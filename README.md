# Bookmarklets

## Packt

### PDP Fix

Use this when in the View screen with side by side to expand out the comments.

```javascript
javascript:$('tbody.hover tr td').each(function() { $(this).find('p').html($(this).find('a').attr('alt')) });$('.eval_photo').find('img').attr('src','https://d3gnp09177mxuh.cloudfront.net/mapt-skills-images/parrot.gif').attr('width','210').attr('height','150');$('.commentIcon').click(function() { setTimeout(function() { document.getElementById('txtComment').focus(); }, 300) } );
```

### Decode all JWT

```javascript
javascript:;function outputToken(env, token) { console.log("Environment: " + env); var parts = token.split(".");console.log(atob(parts[0]));console.log(atob(parts[1]));console.log("Token expires: " + new Date(JSON.parse(atob(parts[1])).exp*1000)); }; var regex = /access_token_([a-z_]+)=([^;]+)/gi;var tokens = document.cookie.match(regex); console.log(tokens); for(var i = 0; i < tokens.length; i++) { var env = /^access_token_(.*)=.*$/.exec(tokens[i])[1]; var token = /^.*=(.*)$/.exec(tokens[i])[1]; outputToken(env, token); };
```

### Log Datalayer

```javascript
javascript: console.log(dataLayer);
```

### Fix mapt scrollbar (Chrome on Windows)
```javascript
javascript:$('head').append('<style>#sidebar-wrapper::-webkit-scrollbar { width: 5px;} #sidebar-wrapper::-webkit-scrollbar-track { background: #333;} #sidebar-wrapper::-webkit-scrollbar-thumb { background: #999; border-radius: 20px;}</style>');
```
