1) El primer error que se muestra es, de que .addEventListener no es una function, y eso es porque lleva una mayúscula en Event, y se debe escribir como guessSubmit.addeventListener('click', checkGuess);

2) No existe una validación para numero enteros, en el formulario, primero está declarado como tipo text, se cambia a number, y se valida dentro de un if si es el userGuess es un dato entero.

3) El resetButton tambien tiene un error a la hora que se ejecuta la funcion setGameOver(), al igual que el primer error se debe cambiar el .addEventListener a resetButton.addeventListener('click', resetGame);

4) Los estilos de los backgroudColor estaban mal, en el caso de que Gane se setea
lastResult.style.backgroundColor = 'green';
En el caso de que Pierda se setea
lastResult.style.backgroundColor = 'red';
Y en el caso de que sea incorrecto y muestre el mensaje de Número es mayo o Número menor setear
lastResult.style.backgroundColor = 'black';