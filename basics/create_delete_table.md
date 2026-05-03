# macOS PostgreSQL Basic Commands on Create and Delete a Table

## Environment
- macOS 13 Ventura (Intel chip)
- Homebrew
- PostgreSQL 16

## Details

### 1) Create database inside SQL console
```ruby
CREATE DATABASE [database_name];
```

> [!TIP]
if the table needs specific setting, in this case, the setting is "to be able to insert Vietnamese data" into the table:<br/>
```ruby
CREATE DATABASE [database_name] character set [CHAR_SET] collate [COLLATION];
```
E.g.:<br/>
```ruby
CREATE DATABASE database_1 character set UTF8 collate utf8_vietnamese_ci;
```

### 2) Connect to the database
```ruby
\c [database_name]
```
As you are connected to the database_1, you should be able to see:</br>
`database_1=#`</br> 
in the terminal

### 3) Delete a database
It is recommended to switch out of the database before deleting the table</br>
`\c postgress`

Delete a database:
```ruby
DROP DATABASE [database_name];
```

> [!TIP]
To confirm whether the database was deleted successfully, check the list of database with</br>
`\l`
