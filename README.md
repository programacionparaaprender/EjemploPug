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


### repositorio padre
https://github.com/DorianDesings/pug2019/blob/master/dev/templates/template.pug

### plugins
http://localhost:3001/plugins

### opciones de instalación
https://www.npmjs.com/package/gulp-pug


### leer archivos json
https://github.com/pugjs/pug/issues/3012
npm install --save path fs

mixin something()
  - 
    let path = require('path');
    let fs = require('fs');
    let dataJson = JSON.parse(fs.readFileSync(path.normalize(js/contactos.json")));
    each item in dataJson
        a(target="_blank", class="dropdown-item", href="#")=item.nombre+'-'+item.titulo


li(class="nav-item dropdown")
    a(class="nav-link dropdown-toggle", href="#", id="navbarDropdown", role="button", data-bs-toggle="dropdown", aria-expanded="false") Contactos
    div(class="dropdown-menu", aria-labelledby="navbarDropdown")  
        +something()

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


li(class="nav-item dropdown")
                                a(class="nav-link dropdown-toggle", href="#", id="navbarDropdown", role="button", data-bs-toggle="dropdown", aria-expanded="false") Cursos
          
                                div(class="dropdown-menu", aria-labelledby="navbarDropdown")            
                                    a(target="_blank", class="dropdown-item", href="#") Curso1
                                    a(target="_blank", class="dropdown-item", href="#") Curso2
                                    a(target="_blank", class="dropdown-item", href="#") Curso3

                        form(class="d-flex fst-italic")
                            input(id="iBuscar",name="nBuscar",class="form-control me-2 fst-italic",type="search",placeholder="Buscar",aria-label="Search")
                            button(class="btn btn-outline-secondary fst-italic",type="submit") Buscar