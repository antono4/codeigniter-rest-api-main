# codeigniter-rest-api

progress build ...

using Myth/Auth library for authanticate

## Requirement

Framework Codeigniter >= 4.5
PHP >= 8.1


## Featured

- [x] Global access using Api-Key
- [x] Authorization Bearer <token>
- [x] CRUD User, Role, Permission default from Myth/Auth
- [ ] Example postman


# postman

## postman

HEADER
```
#Akses Api
Api-Key: <yor api key>

# Akses data login, token didapat dari login
Authorization: Bearer <token>
```


## postman response default

display single data
```json
{
  "status": 200,
  "success": true,
  "error_code": 0,
  "message": "success",
  "data": {
      "item": {}
  }
}
```

display multiple data
```json
{
  "status": 200,
  "success": true,
  "error_code": 0,
  "message": "success",
  "data": {
      "items": [],
      "pagination" : {}
  }
}
```

## Query Params Doc

DOC
===============

## Filter Query By Field

| Key   | Name               | Result                                                             |
| ----- | ------------------ | ------------------------------------------------------------------ |
| `eq`  | equal              | `field = 'value'`                                                  |
| `neq` | not equal          | `field != 'value'`                                                 |
| `lt`  | lower than         | `field < 'value'`                                                  |
| `gt`  | greater than       | `field > 'value'`                                                  |
| `lte` | lower than equal   | `field <= 'value'`                                                 |
| `gte` | greater than equal | `field >= 'value'`                                                 |
| `le`  | like end           | `field LIKE 'value%'`                                              |
| `ls`  | like start         | `field LIKE '%value'`                                              |
| `lse` | like start end     | `field LIKE '%value%'`                                             |
| `in`  | where IN           | `field IN (value)` value using sparator `,` ex `1,2,3,4` / `1`     |
| `nin` | where NOT IN       | `field NOT IN (value)` value using sparator `,` ex `1,2,3,4` / `1` |

### Avilable Param

1. Sort => `sort=-user_name` => `SORT user_name DESC`
2. Sort => `sort=user_name` => `SORT user_name ASC`
3. Sort => field sort sesuai dengan result
4. limit => default: 10 
5. page => default: 1
6. search => `search=keyword` 


## COFFEE FOR BEST PERFORMANCE

**[COFFEE HERE](https://saidqb.github.io/coffee)** for more inovation

OR

<a href="https://trakteer.id/saidqb/tip" target="_blank"><img id="wse-buttons-preview" src="https://cdn.trakteer.id/images/embed/trbtn-red-1.png?date=18-11-2023" height="40" style="border:0px;height:40px;" alt="Trakteer Saya"></a>
