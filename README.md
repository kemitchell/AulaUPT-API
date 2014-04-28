# AulaUPT-API -- Sencilla API para interactuar con el Aula Virtual de la Universidad Privada de Tacna

[![NPM](https://nodei.co/npm/request.png)](https://nodei.co/npm/aulaupt-api/)

##Uso

```javascript
var AulaUPT = require('aulaupt-api');

var aula = new AulaUPT({
	usuario: '2013000725',
	password: '467593649',
})

aula.login(function(login) {
	if(login) {
		aula.getCursos(function(cursos) {
			console.log(cursos)
		})
	} else {
		console.log('Login fallido')
	}
})
```
