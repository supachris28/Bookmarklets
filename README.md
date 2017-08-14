# Bookmarklets

## Packt

### PDP Fix

Use this when in the View screen with side by side to expand out the comments.

```javascript
javascript:$('tbody.hover tr td').each(function() { $(this).find('p').html($(this).find('a').attr('alt')) });$('.eval_photo').find('img').attr('src','https://d3gnp09177mxuh.cloudfront.net/mapt-skills-images/parrot.gif').attr('width','210').attr('height','150');$('.commentIcon').click(function() { setTimeout(function() { document.getElementById('txtComment').focus(); }, 300) } );
```
