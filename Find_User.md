# Find User

```
GET find_user/{username}
```

## Description

Returns a list of user information matching the specificed username.

## Parameters

At least one parameter is required from the following:

| Name     | Data Type | Description |
| -------- | --------- | ----------- |
| username | string    | User name   |

## Returns

**user_info** - List of users with the following values:

| **Name**   | **Data Type** | Description            |
| ---------- | ------------- | ---------------------- |
| username   | string        | User name              |
| email      | string        | User email             |
| accountAge | int           | Age of account in days |

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
