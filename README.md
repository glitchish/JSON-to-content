# JSON-to-content
basically what it sounds like, took 2 minutes to make

snatch the code here:
```html
<!DOCTYPE html>
<html>
<body>

<!-- Basic JSON-to-content code created by @theiocoder (https://github.com/theiocoder)-->

<div id="doc"></p>
<script>
var doc = `{
	"body":[
		{"p":"Hello World!"}
    ]
}
`;
try {
  doc = JSON.parse(doc);
  document.body.innerHTML = "<p>"+doc.body[0].p+"</p>";
} catch(err) {
  document.getElementById("doc").innerHTML = "<span style=\"color: red;\">JSON Error: "+err.message+"</span>";
}

</script>
</body>
</html>
```
_(its messy, i know)_

[originally made at w3school's html editor because y not](https://www.w3schools.com/code/tryit.asp?filename=GR6ML83VFZRG)

its sup~~p~~er basic
