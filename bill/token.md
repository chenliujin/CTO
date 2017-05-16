# Token

## notify
```
curl -H "Content-Type: application/json" -d "{topic:'', content:'', ...}" https://www.example.com/message/v1/notify/topic
```


## NSQ Topic
- topic name: token
- format:
 - appId
 - appToken
 - validTime: 过期时间
 - tokenType: Action(create/update/delete)，执行相应的操作
 - updateTime
 - ipAddress
- 对应的处理脚本

## Redis

### Key
```
'token_' + md5({$appId})
```

### Value
```
{
	'appId': 	'',
	'appToken':	'',
	'validTime':	'',
	'updateTime':	'',
	'ipAddress':	'',
}
```
