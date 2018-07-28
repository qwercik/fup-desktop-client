# FUP desktop client
**F**ile **UP**loader desktop client is simple python app dedicated to uploading, downloading and managing files, that are stored on the FUP server.

## Configuration file
Configuration file is simple INI file. You can declare there several sections, each for another server. Each section contains some values like 'url'.
This is example configuration file:
```
[dev]
url = http://localhost:8000

[production]
url = https://fup.example.com

```

## Usage
```bash
fup.py <server> <action> parameters
```

### Downloading file
```bash
fup.py <server> download <token> [path]
```

### Getting file information
```bash
fup.py <server> info <token>
```

### Uploading file
```bash
fup.py <server> upload <path>
```

### Removing file
```bash
fup.py <server> remove <token>
```
