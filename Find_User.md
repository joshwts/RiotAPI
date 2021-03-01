# Find Champion

```
GET find_user/{username}
```

## Description

Returns a list of users matching the specificed username.

## Parameters

At least one parameter is required from the following:

| Name     | Data Type | Description |
| -------- | --------- | ----------- |
| username | string    | User name   |

## Returns

**user_suggestions** - List of users with the following values:

| **Name**   | **Data Type** | Description            |
| ---------- | ------------- | ---------------------- |
| username   | string        | User name              |
| email      | string        | User email             |
| accountAge | int           | Age of account in days |

## Errors

| Code | Description         |
| ---- | ------------------- |
| 400  | Bad request         |
| 401  | Authorization error |
| 403  | Forbidden           |

## Examples

##### **Request**

```
GET find_user/riotuser
```

##### Return

```
{
   'name': 'riotuser',
   'email': 'user@riot.com',
   'accountAge': 327
}
```
