# Commands

## Crear un nueva tarea de ejecución

```
POST
https://com-edisonmoreno-ms-commands.herokuapp.com/api/cronjob/create

BODY
{
  "type": "ms-commands.cronjob.create",
  "cronJobId": "{{$guid}}",
  "name": "{{$randomFullName}}",
  "url": "{{$randomUrl}}",
  "cronExpression": "* 5 * * * ?",
  "timeout": "3000",
  "retry": "3",
  "email": "{{$randomEmail}}"
}

```

## Agregar ejecuciones

```
POST
https://com-edisonmoreno-ms-commands.herokuapp.com/api/cronjob/execution

BODY
{
    "type": "ms-commands.cronjob.execution",
    "cronJobId": "ca2c7e3a-cbf1-4970-9074-afa2b9888e14",
    "state": "SUCESSS",
    "duration": "{{$randomInt}}",
    "date": "{{$isoTimestamp}}"
}
```
