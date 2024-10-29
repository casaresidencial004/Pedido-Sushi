body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    color: #333;
    margin: 0;
    padding: 0;
}

header {
    background: #007BFF;
    color: #fff;
    padding: 20px 0;
    text-align: center;
}

h1 {
    margin: 0;
}

main {
    max-width: 600px;
    margin: 20px auto;
    padding: 20px;
    background: #fff;
    border-radius: 8px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

form {
    display: flex;
    flex-direction: column;
}

label {
    margin: 10px 0 5px;
    font-weight: bold;
}

input[type="text"],
select,
textarea {
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin-bottom: 15px;
    font-size: 16px;
}

input[type="text"]:focus,
select:focus,
textarea:focus {
    border-color: #007BFF;
    outline: none;
}

textarea {
    resize: vertical; /* Permite redimensionar apenas na vertical */
    height: 100px; /* Altura inicial */
}

button {
    padding: 10px;
    background-color: #28a745;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 16px;
}

button:hover {
    background-color: #218838;
}

#message {
    margin-top: 20px;
    font-size: 16px;
}
