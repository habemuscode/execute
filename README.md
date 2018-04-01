# execute

Versión ES7(async-await) de `child_process.exec` de NodeJS

## Como usarlo
```js

const exec = require('execute')

async function test (mensaje) {
	try {
		await exec(`echo ${mensaje}`)
		console.log('Acierto')
	} catch (error) {
		console.error('Error: ', error)
	}
}

test('Funciona correctamente')
```
Opcionalmente se le puede pasar un objeto con opciones que son las mismas que `child_process.exec`

Documentación oficial -> (https://nodejs.org/api/child_process.html#child_process_child_process_exec_command_options_callback)

[¿Preguntas? ¿Opiniones?](https://github.com/habemuscode/execute/issues/new)

## License (AGPLv3)
