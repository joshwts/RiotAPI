# Find Champion

```
GET find_champion
```

## Description

Returns a list of champions matching the specified name, role, or origin.

## Parameters

At least one parameter is required from the following:

| Name   | Data Type | Description     |
| ------ | --------- | --------------- |
| name   | string    | Champion name   |
| role   | string    | Champion role   |
| origin | string    | Champion origin |

## Returns

**champion_suggestions** - List of champions with the following values:

| **Name** | **Data Type** | Description     |
| -------- | ------------- | --------------- |
| name     | string        | Champion name   |
| role     | string        | Champion role   |
| origin   | string        | Champion origin |

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
GET find_champion?name=sona
```

##### Return

```
{
   'name': 'sona',
   'role': 'support',
   'origin': 'ionia'
}
```

##### Request

```
GET find_champion?role=top+lane
```

##### Return

```
{
   'name': 'teemo',
   'role': 'top lane',
   'origin': 'bandle city'
},
{
   'name':'gangplank',
   'role': 'top lane',
   'origin': 'bilgewater'
}
```

