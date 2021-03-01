# Create Champion

```
PUT create_champion/{name}/{role}/{origin}
```

## Description

Creates a champion and appends it to the database list.

## Parameters

The following parameters are required:

| Name   | Data Type | Description     |
| ------ | --------- | --------------- |
| name   | string    | Champion name   |
| role   | string    | Champion role   |
| origin | string    | Champion origin |

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
