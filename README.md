# up-here
You APPEAR UP HERE

## Back End

```
PYTHONPATH=script uvicorn script.main:app \
    --host localhost \
    --port $PORT \
    --reload \
    --ssl-certfile=rsc/cert.pem \
    --ssl-keyfile=rsc/privkey.pem
```
