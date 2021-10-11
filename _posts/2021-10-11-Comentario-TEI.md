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

1. **La declaración**

        <?xml version="1.0" encoding="UTF-8"?>
        
Indica que se trata de un documento XML, con el tipo de codificación de caracteres: por defecto es siempre UTF-8

2. **El esquema**

        <?xml-model href="http://www.tei-c.org/release/xml/tei/custom/schema/relaxng/teilite.rng" 
        schematypens="http://relaxng.org/ns/structure/1.0"?>
        
Este línea indica a qué modelo concreto se sujeta este documento XML. En el campo de TEI el esquema más utilizado es RelaxNG que tiene como extensión .rng. 

3. **El elemento raíz**

        <TEI xmlns="http://www.tei-c.org/ns/1.0">

El elemento raíz es el encargado de contener el espacio de nombre. En otras palabras, significa a qué tipo de modelo pertenecer las etiquetas utilizadas.
  
4. **El encabezado**

       <teiHeader>
        <fileDesc>
        <titleStmt>
        <title>
        <!-- title of the resource -->
        </title>
        </titleStmt>
        <publicationStmt>
        <p>
        <!-- Information about distribution of the resource -->
        </p>
        </publicationStmt>
        <sourceDesc>
        <p>
        <!-- Information about source from which the resource derives -->
        </p>
        </sourceDesc>
        </fileDesc>
        </teiHeader>
        
Es una de las partes más importantes, pues contiene toda la información de metadatos, normalmente no destinados a la publicación pero imprescinndibles para integrar el documento en un conjunto. 

5. **El cuerpo del documento**

        <text>
            <body>
              <p>El texto </p>
             <figure>
              <!--Este elemento <figure> puede eliminarse pues es solo el logo de TEI -->
                <graphic url="http://www.tei-c.org/logos/TEI-glow.png"/>
              </figure>
           </body>
          </text>
  
        </TEI>
                           
