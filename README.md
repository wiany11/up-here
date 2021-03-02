# up-here
You APPEAR UP HERE

## Back End

```
PYTHONPATH=script uvicorn script.main:app \
    --host 0.0.0.0 \
    --port 44450 \
    --reload \
    --ssl-certfile=rsc/cert.pem \
    --ssl-keyfile=rsc/privkey.pem
```
