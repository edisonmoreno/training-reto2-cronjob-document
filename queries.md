# Queries

## Consultar todas las tareas programadas

```
GET
https://com-edisonmoreno-ms-queries.herokuapp.com/api/cronjob/list
```

## Consultar tareas por id

```
GET
https://com-edisonmoreno-ms-queries.herokuapp.com/api/cronjob/by-id?cron-job-id=ca2c7e3a-cbf1-4970-9074-afa2b9888e14
```

**Param**

cron-job-id: Id de la tarea programada

## Consultar las próximas ejecuciones de una tarea

```
GET
https://com-edisonmoreno-ms-queries.herokuapp.com/api/cronjob/list-next?cron-job-id=ca2c7e3a-cbf1-4970-9074-afa2b9888e14&limit=3
```

**Param**

cron-job-id: Id de la tarea programada
limit: cantidad de próximas fechas a ejecutarse, que dea visualizar.
