# macOS PostgreSQL Installation Notes

## Environment
- macOS 13 Ventura (Intel chip)
- Homebrew

## Process
- PostgreSQL 18 and My SQL had startup errors
- Installed PostgreSQL 16 successfully

## Details

### Step 1: Check Homebrew location
```
which brew
brew --prefix
```

### Step 2: Remove broken PostgreSQL
```
brew uninstall postgresql@18
brew cleanup
```

### Step 3: Reinstall stable version
`brew install postgresql@16`

### Step 4: Start service
`brew services start postgresql@16`

### Step 5: Check service status
`brew services list`

(Step 6: Stop service
`brew services stop postgresql@16`)
