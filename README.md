# curso de pug

### enlace del curso https://www.udemy.com/course/pug-desde-cero/learn/lecture/18223606#overview

### pasos de instalación
https://github.com/pugjs/pug-cli
https://www.npmjs.com/package/pug-cli
npm install -g pug-cli
https://www.npmjs.com/package/gulp-cli
npm install -g gulp-cli


escribir
npm install en el proyecto
luego escribir gulp

### Pug es un motor de plantillas
### Pug es un lenguaje de programación

### condicionales
https://pugjs.org/language/conditionals.html
- const persona = {
                name: "Dorian",
                surname: "Designs",
                age: 30
            }
            each value, key in persona 
                p=`valor: ${key}: ${value}`
            
            p=`Persona nombre: ${persona.name}`