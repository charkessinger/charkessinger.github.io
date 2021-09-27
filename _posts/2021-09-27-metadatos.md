---
layout: post
title: "Comentario de un archivo de metadatos en Dublin Core"
author:
- Charlotte Kessinger
date: 2021-09-27
---

# ¿Qué es Dublin Core?

Dublin Core es un estándar web que consta de **15 nombres** estándar para campos de metadatos para resaltar los detalles más importantes de un documento. Es uno de los esquemas de metadatos más simples y más utilizados. El estándar Dublin Core tiene definiciones de cada elemento de metadatos que establecen qué tipo de información se debe registrar, dónde y cómo. Además, muchos de los elementos de datos tienen estándares de valor de datos, como el Vocabulario de tipo DCMI y los códigos de idioma ISO 639, etc. 

## ¿Quién lo utiliza?

Con frecuencia los museos, las bibliotecas, y algunas platformas de publicación como Omeka usan Dublin Core.

## ¿Para qué sirve?

Dublin core ofrece información de catalogación ampliada y documentación de índice mejorada para programas de búsqueda de Web. Los metadatos de Dublin Core se pueden usar para múltiples propósitos, desde la descripción simple de recursos hasta la combinación de vocabularios de metadatos de diferentes estándares de metadatos, hasta más oportunidades e implementaciones avanzadas.

## ¿Quién lo hizo?
El esquema se originó en Dublín, Ohio en 1995 durante un taller de metadatos. 

# Los 15 elementos de código de Dublin Core

    <?xml version="1.0"?>
    <metadata xmlns:dc="http://purl.org/dc/elements/1.1/">
    ...
    </metadata>
    

**El título** se corresponde a...

       <dc:title>Postal a José María Chacón y Calvo</dc:title>
    
El título representa el nombre con el que se reconoce formalmente un recurso. 

**El creador** aparace como...

       <dc:creator>
       Garcia Lorca, Federico
       </dc:creator>
    
Se refiere a la(s) persona(s) u organización(es) principalmente responsables del contenido intelectual del recurso o el autor.

El código del **subjecto** es...

        <dc:subject>
        Madrid
       </dc:subject>
       <dc:subject>
        Correspondencia
       </dc:subject>
       <dc:subject>
        Postales
       </dc:subject>
       <dc:subject>
        Federico Garcia Lorca
       </dc:subject>

Aquí es importante incluir el tema del recurso, palabras clave, frases o descriptores de clasificación que describen el tema o contenido del recurso.

**El description** se corresponde a...

    <dc:description>
    una carta personal de Garcia Lorca desde Lanjaron a un amigo en Madrid. Incluye un dibujo de una flor.
    </dc:description>
    
Esta etiqueta es una descripción textual del contenido del recurso, incluidos resúmenes en el caso de objetos similares a documentos; también puede ser una descripción del contenido en el caso de los recursos visuales.

**El editorial** se pertenece a...

    <dc:publisher>
    Edicin Jos Galvez
    </dc:publisher>
    
Etsa sección se refiere a la entidad responsable de poner a disposición el recurso en su forma actual, como una editorial, departamento universitario o entidad corporativa.

**Los contribuyentes** van siguiente como...

    <dc:contributor>
    Jose María Chacón y Calvo
    </dc:contributor>
    
Aqui incluyua la(s) persona(s) u organización(es) además de las especificadas en el elemento creador, que han realizado contribuciones intelectuales significativas al recurso pero de forma secundaria.

**La fecha** se pertenece a....

    <dc:date>
    1924-09-17
    </dc:date>
    
La fecha en que el recurso estuvo disponible en su forma actual.

El código del **tipo** esta representado como...

    <dc:type>
    Imagen
    </dc:type>
    <dc:type>
    Texto
    </dc:type>

    
El tipo de recurso, como página de web, novela, poema, documento de trabajo, informe técnico, ensayo o diccionario. Tipo se elija de una lista enumerada de tipos.

**El formato** se corresponde a...

    <dc:format>
    jpg
    </dc:format>
    
El formato significa la representación de datos del recurso, como texto / html, archivo, aplicación, o imagen JPG.











