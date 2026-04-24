# Informe Empresa de Auditoría Fintech

# -- Descripción --
# Este proyecto consiste en un sistema de auditoría diseñado para procesar y almacenar transacciones de pago de una empresa de tecnología financiera (Fintech).
# El desarrollo responde a requisitos regulatorios estrictos, garantizando la total inmutabilidad de los registros y el cumplimiento de transacciones ACID.
# El sistema permite realizar auditorías exactas sobre datos históricos, lo cual es fundamental para la generación de reportes regulatorios fijos que se emiten mensualmente.

# -- Arquitectura seleccionada: Lakehouse --
# ¿Por qué?
# Gracias a su capacidad de manejar transacciones ACID y asegurar inmutabilidad en lo registros, ayuda a evitar datos corruptos durante ka ingesta masiva a traves de metadatos.

# -- Requisitos y Configuración del Entorno Técnico --
# Git: Control de versiones del código.
# Docker: Contenedores para Spark y bases de datos.
# Python: Lenguaje para el procesamiento de datos.
# PySpark / Delta Lake: Librerías para el manejo de la capa de datos.

# -- Instrucciones de Instalación --
# Paso 1: Clonar el repositorio localmente usando Git
# git clone <url repositorio>

# Paso 2: Ir directo a la raiz de la terminal

# Paso 3: Se levantan los servicios y las dependencias requeridas (base de datos) utilizando los contenedores (docker)
# docker-compose up -d

# Paso 4: Se ejecuta el script al iniciar Python para procesar la primera pipeline de ingesta desde la plataforma de pagos ubicada en la capa Bronze.

# -- Estrucutra del repositorio --
# /src:  Contiene el codigo fuente de las pipelanes de datos

# /docs: Carpeta de documentacion tecnica

# /config: Almacenamiento de archivos del entorno, configuracion de segridad ACID y conexion a las bases de datos.
