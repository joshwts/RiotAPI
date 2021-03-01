# Create Champion

```
POST create_champion/{name}/{role}/{origin}
```

## Description

Creates a champion and adds it to the database.

## Parameters

The following parameters are required:

| Name   | Data Type | Description     |
| ------ | --------- | --------------- |
| name   | string    | Summoner name   |
| role   | string    | Summoner role   |
| origin | string    | Summoner origin |

## Returns

This method does not return any values.

## Errors

| Code | Description            |
| ---- | ---------------------- |
| 400  | Bad request            |
| 401  | Authorization error    |
| 403  | Forbidden              |
| 409  | Enpoint-specific error |
| 429  | Too many requests      |
| 500  | Internal server error  |

## Examples

##### **Request**

```
POST create_champion/sona/support/ionia
```

##### Return

```
{
   'name': 'sona',
   'role': 'support',
   'origin': 'ionia'
}
```
