# View SQL
## 1. Vista cliente-invoice. Vemos las columnas que necesitamos desde sus tablas originales y las unimos con JOIN, lo siguiente es ejecutar:
 - Sentencia:

CREATE VIEW invoice_view AS SELECT i.id, i.code, i.create_at, i.total, c.full_name FROM invoice i JOIN client c  ON c.id = i.client_id;
`
-Captura.
<imag!![Imagen de WhatsApp 2024-06-30 a las 12 00 10_9f782963](https://github.com/micaelabar/TAREA-DEBER-GBD../assets/148156209/0ee46ab0-3020-4ae0-9aef-c16443697515)

## 2. Vista detail-product.
 - Sentencia:

CREATE VIEW detail_view AS SELECT d.id, d.quantity, p.description ,d.price, d.quantity * d.price AS subtotal FROM product p JOIN detail d ON p.id = d.productid;
`
-Captura. 
<imag!![Imagen de WhatsApp 2024-06-30 a las 11 34 02_aeaa4df7](https://github.com/micaelabar/TAREA-DEBER-GBD../assets/148156209/e051b526-b3bd-43ea-a078-575bee9350d5)
