---
layout: post
title: "Tarea 4. La Text Encoding Initiative: un ejemplo básico comentado"
date: 2021-10-11
author:
- Charlotte Kessinger 
---

<img src="/assets/images/download.png" alt="TEI" width="400" height="400">

La iniciativa de codificación de texto (TEI) desarrolla y mantiene un estándar para la representación de textos en formato digital. En esencia, TEI elabora una serie de directrices que especifican métodos de codificación para textos legibles por ordenador, específicamente en los estudios de humanidades, ciencias sociales y lingüística. Desde su creación en 1994, bibliotecas, museos, editoriales y académicos individuales han utilizado las directrices para presentar textos para la investigación, la enseñanza y la preservación en línea. 

Veamos a continuación los elementos básicos que debe contener un documento XML-TEI. 

 **La declaración del lenguaje XML**: Indica que se trata de un documento XML, con el tipo de codificación de caracteres: por defecto es siempre UTF-8. Además, nos dice que el documento contiene la versión 1.0 de estándar XML.

        <?xml version="1.0" encoding="UTF-8"?>
        
 **Asocaiación al esquema .rng**: Esta línea indica a qué modelo concreto al que se adapta este documento XML y contra la cual se puede validar el documento. En el caso de TEI, el esquema más utilizado es RelaxNG que tiene como extensión `.rng`:

        <?xml-model href="http://www.tei-c.org/release/xml/tei/custom/schema/relaxng/teilite.rng" 
        schematypens="http://relaxng.org/ns/structure/1.0"?>
        
**El elemento raíz y espacio de nombre**: El elemento raíz es el encargado de contener el espacio de nombre. En otras palabras, significa a qué tipo de modelo pertenecer las etiquetas utilizadas:

        <TEI xmlns="http://www.tei-c.org/ns/1.0">

**El encabezado** es uno de lo elementos más importante de un documento TEI-XML y contiene toda la información de metadatos, normalmente no destinados a la publicación pero imprescinndibles para integrar el documento en un conjunto:

    <teiHeader>
      <fileDesc>
         <titleStmt>
            <title>Ejercicio para el curso de SPA 410</title>
         </titleStmt>
         <publicationStmt>
            <p>University of Miami</p>        
         </publicationStmt>
         <sourceDesc>
            <p>Archivo creado digitalmente para nuestro curso SPA410.</p>
         </sourceDesc>
      </fileDesc>
    </teiHeader>
    
Los metadatos se identifican con los etiquetas de de `fileDesc`, `titleStmt`, `publicationStmt`, y `sourceDesc`:

- *fileDesc* es el elemento obligatorio que incluye información sobre el fichero XML-TEI así como detalles sobre la fuente primaria.
- *titleStmt* inclyue información sobre el nombre del archivo. Aquí, se puede crear una etiqueta de título. En este caso, yo he anadido un título para el             ejercicio.
- *publicationStmt* nos da contexto sobre la publicacion digital del documento. Para nuestra clase, puse la Universidad de Miami.

**El texto**: La otra sección muy importante en un documento XML-TEI es el texto que contiene un subelemento conocido como `body` donde se pone el texto del documento y es necessario para la fucnción del documento XML-TEI. El siguiente ejemplo muestra una etiqueta de párrafo dentro del elemento del cuerpo.

     <text>
          <body>
             <p>Un párrafo explicando el trasfondo de TEI. TEI es un marco de trabajo formado en xml y está definido por pautas generales sobre cómo marcar textos digitales para diferentes disciplinas.</p>
          </body>
      </text>


En conclusión, la formación de un documento XML-TEI está creado por un metódo de reglas y etiquetas estríctas. TEI es independiente de cualquier plataforma o programa, se utiliza para estructurar textos de manera rápida y organizada, y puede adaptarse para muchos campos de estudio y proyectos, con lo cual es muy útil en nuestros trabajos de humanidades digitales.







                           
