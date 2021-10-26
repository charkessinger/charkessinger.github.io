---
layout: post
title: "La Text Encoding Initiative: un ejemplo básico comentado"
date: 2021-10-11
author:
- Charlotte Kessinger 
---

# ¿Qué es un documento XML-TEI?

El iniciativa de codificación de texto (TEI) desarrolla y mantiene un estándar para la representación de textos en forma digital. En esencia, TEI representa directrices que especifican métodos de codificación para textos legibles por máquina, específicamente en los estudios de humanidades, ciencias sociales y lingüística. Desde su creación en 1994, bibliotecas, museos, editoriales y académicos individuales han utilizado las directrices para presentar textos para la investigación, la enseñanza y la preservación en línea.

# Información critical para la creaciòn de un documento de XML-TEI

1. Debe indicar explícitamente o por referencia una especificación de esquema TEI contra la cual se puede validar el documento.

# Directrices para la codificación electrónica de texto

 **La declaración**

        <?xml version="1.0" encoding="UTF-8"?>
        
Indica que se trata de un documento XML, con el tipo de codificación de caracteres: por defecto es siempre UTF-8. Además, nos dice que el documento contiene la versión 1.0 de estándar XML.

 **Asocaiación al esquema .rng**

        <?xml-model href="http://www.tei-c.org/release/xml/tei/custom/schema/relaxng/teilite.rng" 
        schematypens="http://relaxng.org/ns/structure/1.0"?>
        
Este línea indica a qué modelo concreto se sujeta este documento XML. En el campo de TEI el esquema más utilizado es RelaxNG que tiene como extensión .rng. 

3. **El elemento raíz y espacio de nombre**

        <TEI xmlns="http://www.tei-c.org/ns/1.0">

El elemento raíz es el encargado de contener el espacio de nombre. En otras palabras, significa a qué tipo de modelo pertenecer las etiquetas utilizadas.
  
4. **El encabezado**

Uno de lo más importante aspectos de un documento TEI-XML es el encabezado. Aparace en el codígo con la etiqueta *tei header* Pues contiene toda la información de metadatos, normalmente no destinados a la publicación pero imprescinndibles para integrar el documento en un conjunto.

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
    
Los metadatos se identifican con los etiquetas de de *fileDesc*, *titleStmt*, *publicationStmt*, y *sourceDesc*.

*fileDesc* es el elemento obligatorio que incluye  incluye información sobre el fichero XML-TEI así como detalles sobre la fuente primaria.
*titleStmt* inclyue información sobre el nombre del archivo. Aquí, se puede crear una etiqueta de título. En este caso, yo he anadido un título para el             ejercicio.
*publicationStmt* nos da contexto sobre la publicacion digital de fichero del documento. Para nuestra clase, pusé la Universidad de Miami.

5. **El texto**

La otra sección muy importante en un documento XML-TEI es el texto. El texto contiene un subelemento conocido como *body*. En el body se pone el texto actual del documento y es necessario para la fucnción del documento XML-TEI.

     <text>
          <body>
             <p>Un párrafo explicando el trasfondo de TEI. TEI es un marco de trabajo formado en xml y está definido por pautas generales sobre cómo marcar textos digitales para diferentes disciplinas.</p>
          </body>
      </text>

EL ejemplo arribo demonstra una etiqueta de párrafo dentro del elemento del cuerpo.

# Resumen

En conclusión, la formación de un documento XML-TEI está creado por un metódo de reglas y etiquetas estríctas. TEI es independiente de cualquier plataforma o programa, se utiliza para estructurar textos de manera rápida y organizada, y se puede adaptarse para muchos campos de estudio y proyectos y por eso es muy útil en nuestros estudios de las humanidades digitales.







                           
