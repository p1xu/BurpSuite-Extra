## [file-upload-check.bambdas](/file-upload-check.bambdas)
### Bambdas Script to Detect HTML code for file upload in Responses
It is useful to identify a potential file upload from the proxy history.
I used regex to match the `<input>` element with `type="file"` from the HTML response.
```java
// Only applies to in-scope requests. If you want it to apply to all requests, change it to false.
boolean InProxyScopeOnly = true;

// Show only responses that contain an HTML code for file upload.
boolean ShowReponseMatchOnly = true;

// You can choose between this colors (BLUE, CYAN, GRAY, GREEN, MAGENTA, ORANGE, PINK, RED, YELLOW) or NONE for no color.
HighlightColor Color = HighlightColor.CYAN;
```
