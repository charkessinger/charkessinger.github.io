---
layout: post
title: "Tarea 3. Comentario de un archivo de metadatos en Dublin Core"
author:
- Charlotte Kessinger
date: 2021-09-27
---

### ¿Qué es Dublin Core?
Dublin Core es un estándar web que consta de **15 nombres** estándar para campos de metadatos para resaltar los detalles más importantes de un documento. Es uno de los esquemas de metadatos más simples y más utilizados. El estándar Dublin Core tiene definiciones para cada elemento de metadatos que establecen qué tipo de información se debe registrar, dónde y cómo. Además, muchos de los elementos de datos tienen estándares de valor de datos, como el Vocabulario de tipo DCMI y los códigos de idioma ISO 639. 

### ¿Quién lo utiliza?
Con frecuencia los museos, las bibliotecas, y algunas platformas de publicación como Omeka usan Dublin Core.

### ¿Para qué sirve?
Dublin core ofrece información de catalogación ampliada y documentación de índice mejorada para programas de búsqueda de Web. Los metadatos de Dublin Core se pueden usar para múltiples propósitos, desde la descripción simple de recursos hasta la combinación de vocabularios de metadatos de diferentes estándares de metadatos, así como más implementaciones avanzadas.

### ¿Quién lo hizo?
El esquema se originó en Dublín (Ohio) en 1995 durante un taller de metadatos. 

### Los **quince elementos de Dublin Core

La etiqueta de apertura del código corresponde a un simple prólogo XML y un elemento raíz llamado `metada`:

```
<?xml version="1.0"?>
<metadata xmlns:dc="http://purl.org/dc/elements/1.1/">
    ...
</metadata>
```

El **título** aparecen en el siguiente elemento y representa el nombre con el que se reconoce formalmente un recurso:

```
<dc:title>Postal a José María Chacón y Calvo</dc:title>
```

El **creador** re refiere a la(s) persona(s) u organización(es) principalmente responsables del contenido intelectual del recurso o el autor

```
<dc:creator>
    Garcia Lorca, Federico
</dc:creator>
```

En el elemento **subject** es importante incluir el tema del recurso, palabras clave, frases o descriptores de clasificación que describen el tema o contenido del recurso

```
<dc:subject>Madrid</dc:subject>
<dc:subject>Correspondencia</dc:subject>
<dc:subject>Postales</dc:subject>
<dc:subject>Federico Garcia Lorca</dc:subject>
```

En **description** aparece una descripción textual del contenido del recurso, incluidos resúmenes en el caso de objetos similares a documentos; también puede ser una descripción del contenido en el caso de los recursos visuales.

```
<dc:description>
    una carta personal de Garcia Lorca desde Lanjaron a un amigo en Madrid. Incluye un dibujo de una flor.
</dc:description>
```  

La **editorial** del objeto digital se refiere a la entidad responsable de poner a disposición el recurso en su forma actual, como una editorial, departamento universitario o entidad corporativa.

```  
<dc:publisher>
    Edición José Galvez
</dc:publisher>
 ``` 
 
Los **contribuyentes** se incluyen la(s) persona(s) u organización(es) además de las especificadas en el elemento `creator`, que han realizado contribuciones intelectuales significativas al recurso pero de forma secundaria.

 ``` 
<dc:contributor>
    Jose María Chacón y Calvo
</dc:contributor>
 ```     

La **fecha** corresponde a la creación del recurso digital disponible en su forma actual:

```
<dc:date>1924-09-17</dc:date>
```

El tipo de recurso, como página de web, novela, poema, documento de trabajo, informe técnico, ensayo o diccionario, se elige de entre una lista de opciones:

```
<dc:type>Imagen</dc:type>
<dc:type>Texto</dc:type>
```
   
El **formato** significa la representación de datos del recurso, como texto / html, archivo, aplicación, o imagen JPG.

```
<dc:format>jpg</dc:format>
```

El **identificador** corresponde a una cadena o número que se utiliza para identificar de forma exclusiva el recurso digital:

```
<dc:identifier>
    https://merrick.library.miami.edu/cdm/compoundobject/collection/chc5324/id/31/rec/19
</dc:identifier>
```
    
El código del **fuente** representa la procedencia del trabajo, ya sea impreso o electrónico:

```    
<dc:source>University of Miami</dc:source>
```

La etiqueta del **idioma** indica el (los) idioma(s) del contenido intelectual del recurso:

```
<dc:language>SPA</dc:language>
```

La **cobretura** significa el contexto y las caracteristicas espaciales y temporales del recurso:

```
<dc:coverage>1898-1936 Spain</dc:coverage>
```
 
Los **Los derechos** incluyen la información sobre los derechos sobre el recurso:

```
<dc:rights>Domino público</dc:rights>
```

### Conclusión

Los metadatos ayudan a la precisión de la búsqueda en la web. De manera parecida a como añadimos una serie de metadatos en el área del `<head>` de una página web, así sirven algunos tipos específicos de estándares de metadatos. Dublin Core se utiliza para la creación de registros para objetos digitales y su catalogación, recuperación o archivo de documentos electrónicos.


















