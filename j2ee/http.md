# The format of the HTTP request and HTTP response messages are similar and will have following structure −

- An initial status line + CRLF ( Carriage Return + Line Feed i.e. New Line )
- Zero or more header lines + CRLF
- A blank line, i.e., a CRLF
- An optional message body like file, query data or query output.

```code
HTTP/1.1 200 OK
Content-Type: text/html
Header2: ...
...
HeaderN: ...
   (Blank Line)
<!doctype ...>

<html>
   <head>...</head>
   
   <body>
      ...
   </body>
</html>
```
