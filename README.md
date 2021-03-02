# up-here
You APPEAR UP HERE

## Back End

```
su
export LD_LIBRARY_PATH=/PATH/TO/mariadb:$LD_LIBRARY_PATH
export PATH=/PATH/TO/uvicorn:$PATH
export PYTHONPATH=script:$PYTHONPATH
uvicorn script.main:app \
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

export HTTPS=true 
export PORT=443 
export SSL_CRT_FILE=/PATH/TO/cert.pem 
export SSL_KEY_FILE=/PATH/TO/privkey.pem 
npm start
```
