# Token


## NSQ Topic
- topic name:
- format:
 - appId
 - appToken
 - validTime: 过期时间
 - tokenType: Action(create/update/delete)
 - updateTime
 - ipAddress
- 对应的处理脚本

## Action
- create
- update
- delete


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
