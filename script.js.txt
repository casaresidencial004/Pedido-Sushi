document.getElementById('orderForm').addEventListener('submit', function(event) {
    event.preventDefault(); // Impede o envio do formulário padrão

    const fullName = document.getElementById('fullName').value;
    const address = document.getElementById('address').value;
    const whatsapp = document.getElementById('whatsapp').value;
    const combo = document.getElementById('combo').value;
    const observations = document.getElementById('observations').value;

    const orderData = {
        fullName,
        address,
        whatsapp,
        combo,
        observations
    };

    // Envia o pedido para o seu email
    emailjs.send("casaresidencial004@gmail", "template_xcg1vha", orderData)
        .then((response) => {
            document.getElementById('message').innerText = 'Pedido enviado com sucesso!';
            event.target.reset(); // Limpa o formulário
        })
        .catch((error) => {
            document.getElementById('message').innerText = 'Erro ao enviar o pedido: ' + error.text;
        });
});
