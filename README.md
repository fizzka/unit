# unit-example

## Refs:
- https://unit.nginx.org/
- https://github.com/fizzka/php/tree/add-embed

## Example
```
docker build -t unit .

docker run -dit --rm -v $(pwd):/srv -p 8300:8300 -p 8400:8400 unit

#configuration:
curl -X PUT -d @unit.json http://localhost:8400/

curl http://localhost:8300/
```
