# Java Plain Native Image Sample Application

## Building

### With `pack`
```bash
pack build applications/plain-native-image \
  --builder paketobuildpacks/builder:tiny \
  --env BP_NATIVE_IMAGE=true
```

## Running
```bash
docker run --rm -it -p8080:8080 applications/plain-native-image
```

## Viewing

```bash
curl -s http://localhost:8080
```
