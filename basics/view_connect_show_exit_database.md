# macOS PostgreSQL Basic Commands on View, Connect, Show, Switch and Exit the Database

## Environment
- macOS 13 Ventura (Intel chip)
- Homebrew
- PostgreSQL 16

## Details

### Start service
`brew services start postgresql@16`

### Open SQL console & Enter PostgreSQL shell
`psql postgres`

### Check database list
`\l`

### Connect to database
`\c [database_name]`

### Show table inside current database
`\dt`

### Switch table (back to postgress in this case)
`\c postgress`

### Exit Postgress
`\q`
