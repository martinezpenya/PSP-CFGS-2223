---
title: EXTRAORDINARIA
language: ES
author: David Martínez Peña [www.martinezpenya.es]
subject: Programación de Servicios y Procesos
keywords: [PSP, 2022, Programacion, servicios, procesos, multihilo, Java]
IES: IES Eduardo Primo Marqués (Carlet) [www.ieseduardoprimo.es]
header: ${title} - ${subject} (ver. ${today}) 
footer:${currentFileName}.pdf - ${author} - ${IES} - ${pageNo}/${pageCount}
typora-root-url:${filename}/../
typora-copy-images-to:${filename}/../assets
imgcover:/media/DADES/NextCloud/DOCENCIA/PSP_2223/PSP-CFGS-2223/UD01/assets/cover.png
---
[toc]

# Introducción

La finalidad de este documento es la de guiar al alumno en el proceso de recuperación del módulo "Programación de servicios y procesos" de 2º de DAM.

El alumno deberá seguir las indicaciones del profesor y asistirá a las sesiones de seguimiento que se convoquen. No servirá realizar el presente proyecto de manera completa pero sin asistir al seguimiento propuesto.

Este proyecto tiene intención de evaluar la parte práctica de la asignatura, mientras que durante el periodo de exámenes de la convocatoria extraordinaria el alumno deberá realizar un examen perteneciente a la parte teórica. La nota final de la asignatura será la nota media entre la nota del proyecto y la nota del examen. Será necesario obtener al menos un 4 en cada una de las partes.

# Estilo

El estilo a utilizar en el documento a entregar seguirá las siguientes indicaciones:

- No contendrá faltas de ortografía.

- En general se redactará con pronombres reflexivos. Ejemplo: "se realizó" en lugar de "realicé".

- En la portada aparecerá:

  - En la parte de arriba los logotipos del instituto, GVA, ministerio y Fondo Social Europeo (proporcionados por el profesor)

  - En la parte de abajo a la derecha el texto siguiente:
    - Nombre del alumno
    - Memoria final Programación de Servicios y procesos
    - IES Eduardo Primo Marqués. Curso 20XX/XX

- En cada página:

- - En el encabezado de página aparecerá el nombre de la asignatura.
  - En el pie de página: nombre del alumno y número de página.

- Tipo de fuente: Helvetica o similar (por ejemplo Arial).

- Tamaño: 11 puntos.

- Alineación: justificado.

- Interlineado: 1,15 líneas.

- Pies de imagen / tabla: tamaño 9.

- En fragmentos de código, salidas de consola, etc.: tipo de fuente monoespaciada, tamaño 10.

- Títulos:

- - Los epígrafes de capítulos, apartados y subapartados tienen que aparecer jerarquizados por la tipografía y con números arábicos subdivididos por puntos (por ejemplo):

    1.CAPÍTULO

    ​	1.1. Apartado

    ​		1.1.1. Subapartado)

  - Tamaño título nivel 1: 16 puntos.

  - Tamaño título nivel 2: 14 puntos.

  - Tamaño título nivel 3: 12 puntos.

- Márgenes:

  - Superior (incluye cabecera) e izquierdo: 3 cm.
  - Inferior y derecho: 2 cm.

- Si se incluyen anexos, estos se identificarán por letras mayúsculas consecutivas. Ejemplo: Anexo A, Anexo B...

# Proyecto

Constará de diferentes fases:

- **FASE1**: Preparación del entorno
  - AWS Academy (Cloud9)
  - Github
  - Servidor de socket simple en AWS - Cliente en local
- **FASE2**: Comenzamos con el `chatBot`. Aplicación multihilo.
  - Preparar el servidor para que admita más de un cliente simultáneo.
  - Los clientes accederán al servidor y podrán enviar mensajes de manera simultanea y también recibirán la información que envíen otros clientes.
- **FASE3**: Asegurando `chatBot` . Certificados de clave pública/privada.
  - El servidor tendrá configurado un certificado de clave asimétrica.
  - Los clientes (seguirán siendo más de uno y podrán actuar simultáneamente) deberán establecer una conexión segura con el servidor.
- **FASE4**: Implementar funciones de Bot.
  - El servidor y el cliente compartirán una Interfaz común de métodos (acciones o comandos del bot).
  - El cliente podrá listar esta lista de funciones, cuando el usuario decide invocar un comando (por ejemplo `!hora` ) se realizará la llamada al servidor.
  - El servidor cuando reciba la solicitud del cliente, realizará la tarea asociada al comando (por ejemplo devolver la hora del sistema) y devolverá la información al cliente que la solicitó o a todos los clientes (según el tipo de comando).
- **FASE5**: Ampliación del alumno.
  - El alumno añadirá al menos dos comandos individuales y dos comandos grupales.
  - Además se valorará cualquier idea que el alumno añada al proyecto.

# Contenido

El proyecto pretende recopilar no solo el contenido de la asignatura, sino el de otras materias que deberían estar asimiladas del curso anterior.

El alumno debe:

- Crear un repositorio en GitHub (o similar), y compartirlo con el profesor para poder hacer seguimiento en cada una de las fases.
- No podrá avanzar a la siguiente fase, si no tiene validada la anterior.
- Deberá documentar en la memoria (se recomienda generar un documento online que permita revisiones y anotaciones) el proceso de resolución de cada fase, así como las partes que le han resultado más fáciles y/o más difíciles.

El profesor por su lado:

- Realizará seguimiento del repositorio de GitHub y de la memoria durante la duración del proyecto
- Sugerirá cambios y modificaciones al alumno a través de anotaciones o correos electrónicos, así como comentarios en persona durante las sesiones presenciales o telemáticas de seguimiento.

# Fechas importantes

El proceso de recuperación comenzará el día 13 de marzo con la primera sesión de seguimiento en la que se explicará este documento, de dará acceso a la academia de AWS y se asesorará al alumnado en la creación del repositorio Git o del documento online para la memoria.

La entrega del documento se realizará al menos 10 días antes de la fecha del examen programado en la convocatoria extraordinaria.

# Fuentes de información

- [Wikipedia](https://en.wikipedia.org)
- [Programación de servicios y procesos - FERNANDO PANIAGUA MARTÍN [Paraninfo]](https://www.paraninfo.es/catalogo/9788413665269/programacion-de-servicios-y-procesos)
- [Programación de Servicios y Procesos - ALBERTO SÁNCHEZ CAMPOS [Ra-ma]](https://www.ra-ma.es/libro/programacion-de-servicios-y-procesos-grado-superior_49240/)
- [Programación de Servicios y Procesos - Mª JESÚS RAMOS MARTÍN - [Garceta] (1ª y 2ª Edición)](https://www.garceta.es)
- [Programación de servicios y procesos - CARLOS ALBERTO CORTIJO BON [Sintesis]](https://www.sintesis.com/desarrollo%20de%20aplicaciones%20multiplataforma-341/programaci%C3%B3n%20de%20servicios%20y%20procesos-ebook-2910.html)
- [Programació de serveis i processos - JOAR ARNEDO MORENO, JOSEP CAÑELLAS BORNAS i JOSÉ ANTONIO LEO MEGÍAS [IOC]](https://ioc.xtec.cat/materials/FP/Recursos/fp_dam_m09_/web/fp_dam_m09_htmlindex/index.html)
-  GitHub repositories:
  - https://github.com/ajcpro/psp
  - https://oscarmaestre.github.io/servicios/index.html
  - https://github.com/juanro49/DAM/tree/master/DAM2/PSP
  - https://github.com/pablohs1986/dam_psp2021
  - https://github.com/Perju/DAM
  - https://github.com/eldiegoch/DAM
  - https://github.com/eldiegoch/2dam-psp-public
  - https://github.com/franlu/DAM-PSP
  - https://github.com/ProgProcesosYServicios
  - https://github.com/joseluisgs
  - https://github.com/oscarnovillo/dam2_2122
  - https://github.com/PacoPortillo/DAM_PSP_Tarea02_La-Cena-de-los-Filosofos
