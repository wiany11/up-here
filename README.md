# up-here
You APPEAR UP HERE

## Back End

```
sudo \
    LD_LIBRARY_PATH=/PATH/TO/mariadb:$LD_LIBRARY_PATH \
    PYTHONPATH=script:$PYTHONPATH \
    /PATH/TO/uvicorn script.main:app \
        --host localhost \
        --port $PORT \
        --reload \
        --ssl-certfile=/PATH/TO/cert.pem \
        --ssl-keyfile=/PATH/TO/privkey.pem
```

## Front End

```
su
export PATH=/PATH/TO/npx:$PATH

mv -f front front.0
npx create-react-app front
cd front
```

```
```
