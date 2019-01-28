## 1. Start the container
```
docker run -it -p 8888:8888 --env="DISPLAY" -v "$PWD/notebooks:/home/ubuntu/notebooks" sewook/ml-base
```

## 2. Start jupyter notebook 
```
jupyter notebook --allow-root --notebook-dir=/home/ubuntu/notebooks --port=8888 --no-browser
```

Find the token value from the log. The token value changes every time the container starts. 

```
    To access the notebook, open this file in a browser:
        file:///home/ubuntu/.local/share/jupyter/runtime/nbserver-1-open.html
    Or copy and paste one of these URLs:
        http://(00e1dc8c35b6 or 127.0.0.1):8888/?token=39cc883e8ceef0f76acfaee4d19ea5f05c51ff7db0176e76
```

## 3. Open the browser
```
http://localhost:8888/?token=39cc883e8ceef0f76acfaee4d19ea5f05c51ff7db0176e76
```

## 4. Open the xgboost_tutorial notebook and follow instruction. 

For more information, refer to the original blog post: https://www.datacamp.com/community/tutorials/xgboost-in-python

