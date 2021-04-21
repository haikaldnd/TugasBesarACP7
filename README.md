# TugasBesarACP7
Kelompok 2 : Febri Arianto dan Mohammad Haikal Hasnain

## CREATE PRODUCT
Request : 
- Method : POST
- EndPoint : '/product'
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
