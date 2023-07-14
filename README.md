# Diagrama-de-clases

          +-----------------+
          |   AmazonApp     |
          +-----------------+
          | - url: String   |
          +-----------------+
          | + search(keyword: String): void |
          | + scrapeResults(): List<Product> |
          +-----------------+

                ^
                |
                |
+----------------------------------+
|            Product               |
+----------------------------------+
| - title: String                  |
| - price: double                  |
+----------------------------------+
| + getTitle(): String             |
| + getPrice(): double             |
+----------------------------------+
Descripción de Clases:

AmazonApp:

Atributos:
url (String): la URL de la página de resultados de Amazon.
Métodos:
search(keyword: String): realiza una búsqueda de productos en Amazon basada en la palabra clave proporcionada.
scrapeResults(): List<Product>: realiza el web scraping de la página de resultados de Amazon y devuelve una lista de productos encontrados.
Product:

Atributos:
title (String): el título del producto.
price (double): el precio del producto.
Métodos:
getTitle(): String: devuelve el título del producto.
getPrice(): double: devuelve el precio del producto.
