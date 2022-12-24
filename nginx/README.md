``` bash
# http://localhost/ws/apple

location /ws {
  proxy_pass http://localhost:8000/ws;
  # console.log(req.url) // /ws/apple
}

location /ws/ {
  proxy_pass http://localhost:8000/ws;
  # console.log(req.url) // /wsapple
}

location /ws {
  proxy_pass http://localhost:8000/ws/;
  # console.log(req.url) // /ws//apple
}

location /ws/ {
  proxy_pass http://localhost:8000/ws/;
  # console.log(req.url) // /ws/apple
}
```
