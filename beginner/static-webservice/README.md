# Sample of static web service

## How to run

Start the service from a terminal

```bash
# builds the binary
go build

# executes the binary on Windows
static-webservice.exe
```

From another terminal

```bash
# sends a plain text request
curl http://localhost:3000/?name=World

# sends a request to receive a json formatted response
curl -H "Accept: application/json" http://localhost:3000/?name=World
```
