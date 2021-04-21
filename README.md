# TugasBesarACP7
Kelompok 2 : Febri Arianto dan Mohammad Haikal Hasnain

## CREATE PRODUCT
Request : 
- Method : POST
- EndPoint : '/products'
- Header :
  - Content-Type : application/json
  - Accept : application/json
- Body :
```json
{
  "id" : "int, Primary Key",
  "id_kategori" : "int, Foreign Key To Category Table",
  "name" : "varchar",
  "desc" : "varchar",
  "stock" : "int",
  "harga" : "int",

}
```

-Response :
```json
{
    "code" : "number",
    "status" : "string",
    "data" : {
        "id" : "string, Primary Key",
        "id_kategori" : "int, Foreign Key To Category Table",
        "name" : "varchar",
        "desc" : "varchar",
        "harga" : "int",
        "stock" : "int",
        "createdAt" : "date"
     }
}
```


## GET PRODUCT
Request : 
- Method : GET
- EndPoint : '/products/{id}'
- Header :
  - Accept : application/json

-Response :
```json
{
    "code" : "number",
    "status" : "string",
    "data" : {
        "id" : "string, Primary Key",
        "id_kategori" : "int, Foreign Key To Category Table",
        "name" : "varchar",
        "desc" : "varchar",
        "harga" : "int",
        "stock" : "int",
        "createdAt" : "date"
     }
}
```

## LIST PRODUCT 
Request : 
- Method : GET
- EndPoint : '/products'
- Header :
  - Accept : application/json
-Response :
```json
{
    "code" : "number",
    "status" : "string",
    "data" : {
        "id" : "string, Primary Key",
        "id_kategori" : "int, Foreign Key To Category Table",
        "name" : "varchar",
        "desc" : "varchar",
        "harga" : "int",
        "stock" : "int",
        "createdAt" : "date"
     },
     {
        "id" : "string, Primary Key",
        "id_kategori" : "int, Foreign Key To Category Table",
        "name" : "varchar",
        "desc" : "varchar",
        "harga" : "int",
        "stock" : "int",
        "createdAt" : "date"
     }
}
```

## DELETE PRODUCT 
Request : 
- Method : DELETE
- EndPoint : '/products/{id}'
- Header :
  - Accept : application/json
-Response :
```json
{
    "code" : "number",
    "status" : "string"
}
```

## GET USER
Request : 
- Method : GET
- EndPoint : '/users/{id}'
- Header :
  - Content-Type : application/json
  - Accept : application/json
- Body :
```json
{
  "id" : "int, Primary Key",
  "email" : "varchar",
  "name" : "varchar",
  "address" : "varchar",
  "createdAt" : "date"

}
```

-Response :
```json
{
    "code" : "number",
    "status" : "string",
    "data" : {
      "id" : "int, Primary Key",
  "email" : "varchar",
  "name" : "varchar",
  "address" : "varchar",
  "createdAt" : "date"
     }
}
```

## CREATE TRANSACTION
Request : 
- Method : POST
- EndPoint : '/transaction'
- Header :
  - Content-Type : application/json
  - Accept : application/json
- Body :
```json
{
  "id" : "int, Primary Key",
  "id_user" : "int, Foreign key to user table",
  "date" : "datetime",
  "status" : "int",
  "createdAt" : "date"

}
```

-Response :
```json
{
    "code" : "number",
    "status" : "string",
    "data" : {
   "id" : "int, Primary Key",
  "id_user" : "int, Foreign key to user table",
  "date" : "datetime",
  "status" : "int",
  "createdAt" : "date"
     }
}

