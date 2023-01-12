var alumno = {
    nombre: null,
    apellidos: null,
    fecha_nacimiento: null,
    saluda() {
        return "Hola mi nombre es: " + this.nombre + " " + this.apellidos + " mucho gusto";
    },
    edad() {
        return "mi edad es:" + this.fecha_nacimiento
    }
}

function saveStudent() {
    alumno.nombre = document.getElementById('name').value;
    alumno.apellidos = document.getElementById('lastname').value;
    alumno.fecha_nacimiento = document.getElementById('year').value;
}

function saludar() {
    alert(alumno.saluda());
    alert(alumno.edad());
}
