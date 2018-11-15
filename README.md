### to check the request flow with host header 

```curl http://127.0.0.1:4140/ -H 'Host: red'```

```curl http://127.0.0.1:4140/ -H 'Host: green'```

### Dtab add

```$ export NAMERD_URL=http://localhost:4180```

```curl -v -X PUT -d"/svc/red => /$/inet/red/80" -H "Content-Type: application/dtab" $NAMERD_URL/api/1/dtabs/default```
