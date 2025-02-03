document.getElementById('formulario-contacto').addEventListener('submit', function (event) {
    event.preventDefault(); // Evita que el formulario se envíe de inmediato

    // Aquí puedes agregar validaciones adicionales

    // Envía el formulario
    fetch(this.action, {
        method: this.method,
        body: new FormData(this),
        headers: {
            'Accept': 'application/json'
        }
    }).then(response => {
        if (response.ok) {
            alert('Mensaje enviado con éxito. ¡Gracias!');
            this.reset(); // Limpia el formulario
        } else {
            alert('Hubo un error al enviar el mensaje. Inténtalo de nuevo.');
        }
    }).catch(error => {
        alert('Hubo un error al enviar el mensaje. Inténtalo de nuevo.');
    });
});
