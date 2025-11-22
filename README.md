 README – Big Data Fase 4 (Proyecto con datos modificados)
Descripción del proyecto

Este proyecto corresponde a la Fase 4 de Big Data, donde se trabaja con una base de datos en MongoDB, se realizan modificaciones a los datos originales y se ejecutan consultas para el análisis de información.
El repositorio contiene:

Base de datos exportada desde MongoDB Compass con datos modificados.

Archivo con consultas en MongoDB para realizar búsquedas específicas.

Documentación del proceso y estructura del proyecto.

 Archivos del repositorio
1. datos_modificados.json

Archivo exportado desde MongoDB Compass.
Incluye los registros editados según los cambios realizados por el estudiante:

Nuevos municipios

Nuevos departamentos

Entidad modificada

Valores diferentes en GiZScore, PR u otros campos

2. consultas.js

Archivo con las consultas realizadas sobre la colección. Estas son las consultas incluidas:

// 1. Buscar por municipio
db.Homicidios.find({ Municipio: "TuMunicipio" });

// 2. Buscar GiZScore mayor a 2
db.Homicidios.find({ GiZScore: { $gt: 2 } });

// 3. Buscar por departamento
db.Homicidios.find({ Departamento: "TuDepartamento" });

// 4. Buscar por ENTIDAD
db.Homicidios.find({ ENTIDAD: "TuEntidad" });

// 5. Buscar PR mayor o igual que 10
db.Homicidios.find({ PR: { $gte: 10 } });

 Proceso realizado
 1. Modificación de datos

Los datos iniciales fueron editados directamente en MongoDB Compass usando la opción Edit Document.
Se cambiaron campos como:

Municipio

Departamento

ENTIDAD

GiZScore

PR

Luego fueron exportados en formato .json.

 2. Creación de consultas

Se realizaron cinco consultas específicas para analizar los datos de la colección Homicidios, aplicando filtros usando la sintaxis de MongoDB.

 Cómo ejecutar las consultas

Abrir MongoDB Compass o la consola de Mongo Shell.

Seleccionar la base de datos y la colección.

Copiar cualquiera de las consultas del archivo consultas.js.

Pegarlas en la sección Filter o ejecutarlas desde la terminal.

 Tecnologías utilizadas

MongoDB

MongoDB Compass

Git & GitHub

JavaScript (para archivo de consultas)

 Autor del proyecto
 desarrollado por Luis Felipe, estudiante de Ingeniería de Sistemas.
