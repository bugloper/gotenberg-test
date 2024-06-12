```bash
curl -X POST "https://localhost:3000/forms/chromium/convert/html" \
  --header 'Content-Type: multipart/form-data' \
  --form 'files=@index.html' \
  --form 'files=@header.html' \
  --form 'files=@footer.html' \
  --form 'files=@style.css' \
  --form 'files=@script.js' \
  --form 'files=@logo.png' \
  --form 'files=@logo.svg' \
  --form 'paperWidth=8.27' \
  --form 'paperHeight=11.7' \
  --form 'marginTop=1cm' \
  --form 'marginBottom=1cm' \
  --form 'marginLeft=1cm' \
  --form 'marginRight=1cm' \
  --form pageRanges='1-3,5' \
  --output html.pdf
```
