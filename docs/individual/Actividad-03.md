<div style="display: table;">
    <div style="width: 75%;float: left;margin: auto;padding: 50px 0px 50px 10px; float: left;">
        <span style="color: black;font-size: 25px;font-weight: bold;"> JSON & XML</span></br></br>
    </div>
    <img src="/archivos/index/vs.jpg" alt="drawing" width="200" style="width: 25%;"/>
</div>
&nbsp;

# ¿Qué es Json?

JSON, cuyo nombre corresponde a las siglas JavaScript Object Notation o Notación de Objetos de JavaScript, es un formato ligero de intercambio de datos, que resulta sencillo de leer y escribir para los programadores y simple de interpretar y generar para las máquinas.

JSON es un formato de texto completamente independiente de lenguaje, pero utiliza convenciones que son ampliamente conocidos por los programadores, entre ellos:

+ C
+ C++
+ C#
+ JavaScripts
+ Java 
+ Perl
+ Python

Dichas propiedades hacen de JSON un formato de intercambio de datos ideal para usar con API REST o AJAX. 

# Caracteristicas de Json

Al ser un formato que es independiente de cualquier lenguaje de programación, es que los servicios que comparten información por este método no necesitan hablar el mismo idioma, es decir, el emisor puede ser Java y el receptor Python, pues cada uno tiene su propia librería para codificar y decodificar cadenas en este formato. 

Podemos concluir entonces en que JSON es un formato común para ‘serializar’ y ‘deserializar’ objetos en la mayoría de los idiomas.

* JSON es solo un formato de datos.
* Requiere usar comillas dobles para las cadenas y los nombres de propiedades. Las comillas simples no son válidas.
* Una coma o dos puntos mal ubicados pueden producir que un archivo JSON no funcione. 
* Puede tomar la forma de cualquier tipo de datos que sea válido para ser incluido en un JSON, no solo arreglos u objetos. Así, por ejemplo, una cadena o un número único podrían ser objetos JSON válidos.
* A diferencia del código JavaScript, en el que las propiedades del objeto pueden no estar entre comillas, en JSON solo las cadenas entre comillas pueden ser utilizadas como propiedades.

# Ventajas y Desventajas de Json

|   Ventajas                                | Desventajas|
| :----------------------------------:      | :---------: |
|Es autodescriptivo y fácil de entender.    | Algunos desarrolladores encuentran su escueta notación algo confusa.    |
| Su sencillez le ha permitido posicionarse como alternativa a XML.  | No cuenta con una característica que posee XML: extensibilidad.    |
|   Es más rápido en cualquier navegador.                                | No soporta grandes cargas, solo datos comunes.  |
|Es más fácil de leer que XML.| |Para la seguridad requiere de mecanismos externos como expresiones regulares.|
|Es más ligero (bytes) en las transmisiones.|||
|Se parsea más rápido.|||
|Velocidad de procesamiento alta.|||
|Puede ser entendido de forma nativa por los analizadores de JavaScript.|||

# Ejemplo Json

+ { "name"   : "John Smith",
  "sku"    : "20223",
  "price"  : 23.95,
  "shipTo" : { "name" : "Jane Smith",
               "address" : "123 Maple Street",
               "city" : "Pretendville",
               "state" : "NY",
               "zip"   : "12345" },
  "billTo" : { "name" : "John Smith",
               "address" : "123 Maple Street",
               "city" : "Pretendville",
               "state" : "NY",
               "zip"   : "12345" }
}

+ {
  "billTo":{
    "zip":"12345",
    "city":"Pretendville",
    "name":"John Smith",
    "state":"NY",
    "address":"123 Maple Street"
  },
  "sku":"20223",
  "shipTo":{
    "zip":"12345",
    "city":"Pretendville",
    "name":"Jane Smith",
    "state":"NY",
    "address":"123 Maple Street"
  },
  "name":"John Smith",
  "price":23.95
}

# ¿Qué es XML?

XML proviene del estándar SGML, que es utilizado para definir lenguajes de marcado generalizados para documentos.

 La sigla XML es la abreviación de la expresión "Extensible Markup Language", lo que podría traducirse como “Lenguaje de Marcas Extensible”. Se trata de un lenguaje utilizado para estructurar la información en cualquier documento que contenga texto como por ejemplo los archivos de configuración de una aplicación específica o una base de datos.

# Caracteristicas de XML

+ XML es un subconjunto de SGML que incorpora las tres características más importantes de este:
     + Extensibilidad
     + Estructura
     + Validación
+ Basado en texto.
+ Orientado a los contenidos no presentación.
+ Las etiquetas se definen para crear los documentos, no tienen un significado preestablecido.
+ No es sustituto de HTML.
+ No existe un visor genérico de XML.

# Ventajas y Desventajas de XML 

|   Ventajas                                | Desventajas|
| :----------------------------------:      | :---------: |
|Tiene un formato estructurado y fácil de comprender. | El formato es sumamente estricto. |
|  Separa radicalmente la información o el contenido de su presentación o formato. |  Lleva más tiempo procesarlo.   |
| Está diseñado para ser utilizado en cualquier lenguaje o alfabeto. |  Complejidad de analizador (parser). |
|Su análisis sintáctico es fácil debido a las estrictas reglas que rigen la composición de un documento.| |Un error en cualquier parte del formato puede hacer que todo el documento sea inválido.|
|Tiene soporte a cualquier tipo de datos.|
|Se pueden definir estructuras complejas y reutilizables.|||

# Ejemplo XML

+ <?xml version="1.0" encoding="UTF-8"?>
<json>
  <name>John Smith</name>
  <sku>20223</sku>
  <price>23.95</price>
  <shipTo>
    <name>Jane Smith</name>
    <address>123 Maple Street</address>
    <city>Pretendville</city>
    <state>NY</state>
    <zip>12345</zip>
  </shipTo>
  <billTo>
    <name>John Smith</name>
    <address>123 Maple Street</address>
    <city>Pretendville</city>
    <state>NY</state>
    <zip>12345</zip>
  </billTo>
</json>

+ <?xml version="1.0" encoding="UTF-8"?>
<json>
  <billTo>
    <zip>12345</zip>
    <city>Pretendville</city>
    <name>John Smith</name>
    <state>NY</state>
    <address>123 Maple Street</address>
  </billTo>
  <sku>20223</sku>
  <shipTo>
    <zip>12345</zip>
    <city>Pretendville</city>
    <name>Jane Smith</name>
    <state>NY</state>
    <address>123 Maple Street</address>
  </shipTo>
  <name>John Smith</name>
  <price>23.95</price>
</json>


# Diferencias y Similitudes

XML puede ser usado como un formato de intercambio para que los usuarios muevan datos entre aplicaciones similares, tal y como JSON. XML se procesa facilmente debido a que la estructura de los datos es simple y estándar, sin embargo, JSON se procesa mas facilmente. Hay una amplia gama de softwares reutilizables disponibles para los programadores para manejar XML por lo que no tienen que reinventar codigo.
JSON, siendo una notación más simple, necesita mucho menos software especializado. En los lenguajes JavaScript y Phyton, la notación JSON está integrada en el lenguaje de programación, sin necesidad de software adicional.


# Referencias

https://www.nextu.com/blog/que-es-json/

https://tecnologia-facil.com/que-es/que-es-xml-para-que-sirve-caracteristicas-y-ventajas/#%C2%BFQue_es_XML?

https://www.ibm.com/docs/en/datapower-gateways
