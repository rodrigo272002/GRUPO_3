# Grupo 3
-Antonio Benito Jose Manuel
-Carpio Vásquez Joel Dery
-Choquecallata Villca Federico
-Valverde Huarachi Rodrigo Cristian

# Sistema de Gestión de Encomiendas - Proyecto actualizado

Versión mejorada del proyecto `trabajotablas`, ampliada con las tablas faltantes del modelo relacional del proyecto final.

## Incluye

- NestJS + TypeORM + PostgreSQL
- Swagger en `/api/docs`
- CRUD básico para todas las tablas del modelo
- Script SQL completo en `database.sql`
- Configuración por variables de entorno

## Tablas incluidas

- cliente
- sucursal
- contacto_cliente
- cliente_sucursal
- tipo_paquete
- encomienda
- detalle_encomienda
- seguro
- estado_envio
- envio
- seguimiento
- entrega
- usuario
- empleado
- pago
- factura

## Instalación

1. Copiar `.env.example` a `.env`
2. Crear la base de datos en PostgreSQL
3. Ejecutar `database.sql`
4. Instalar dependencias:

```bash
npm install
```

5. Ejecutar el proyecto:

```bash
npm run start:dev
```

## Variables de entorno

```env
DB_HOST=localhost
DB_PORT=5432
DB_USERNAME=postgres
DB_PASSWORD=postgres
DB_NAME=sisenc_test
PORT=3000
```

## Swagger

Una vez iniciado el servidor, abrir:

```text
http://localhost:3000/api/docs
```

## Nota

Esta versión deja `synchronize: false` para respetar la estructura creada desde el script SQL.
