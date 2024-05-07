### Postman Scripts

Below script will automate to add environment variable into Postman. In this case is TOKEN and IDENTITY.
So we can use as {{TOKEN}} and {{IDENTITY}}

```
if (pm.response.code === 200) {
    var res = pm.response.json();
    if (res.status && res.code===200) {
        postman.setEnvironmentVariable("TOKEN", res.data.token);
        postman.setEnvironmentVariable("IDENTITY", res.data.identity);
    }
}
```

screenshot as below :

![Sample postman](https://github.com/nunahsan/my-note/blob/main/postman.png)
