Punto numero 1: se corrigió esta linea de código para obtener un numero aleatorio.
//let randomNumber = Math.random() * 10;
  let randomNumber = Math.floor(Math.random() * 100) + 1;

Punto numero 2: Se corrigió ETTEMPS a ATTEMPTS, Hacía falta una T
//const ATTEMPS = 5;
  const ATTEMPTS = 10;

Punto numero 3: Se corrigió esta linea, hacía falta un (.) al inicial de lowOrHi, paso de ser lowOrHi a .lowOrHi
 //const lowOrHi = document.querySelector('lowOrHi');
  const lowOrHi = document.querySelector('.lowOrHi');

Punto numero 4: se corriogió esta linea para convertir la variable userGuess a un número antes de realizar la comparación.
 //let userGuess = guessField.value;
    let userGuess = parseInt(guessField.value);

Punto numero 5:
//Hacia falta esta funcion para que no acepte numeros que no este en el rango y asi no incremente
    if (isNaN(userGuess) || userGuess < 1 || userGuess > 100) {
          alert('Por favor, ingresa un número entero válido entre 1 y 100.');
          guessField.value = '';
          return; // No incrementar el contador de intentos
        }
Punto numero 6:
//Aqui va GANASTE con color VERDE, estaba PERDISTE Y EN COLOR NEGRO
      //lastResult.textContent = '!!!Pérdistes!!!';
      lastResult.textContent = 'Felicitaciones! adivinaste el número!';
      //lastResult.style.backgroundColor = 'black';
      lastResult.style.backgroundColor = 'green';

Punto numero 7:
//Faltaba una T en ATTEMPTS, antes estaba como ATTEMPS
else if(guessCount === ATTEMPTS)

Punto numero 8: Aqui va perdiste, el color estaba bien.
      //lastResult.textContent = 'Felicitaciones! adivinaste el número!';
      lastResult.textContent = '!!!Pérdistes!!!';
      lastResult.style.backgroundColor = 'red';

Punto numero 9:
lastResult.textContent = 'Incorrecto! ';
      Aqui debe ser de color NEGRO antes estaba como VERDE
      //lastResult.style.backgroundColor = 'green';
      lastResult.style.backgroundColor = 'black';

Punto numero 10: addeventListener estaba mal escrito, lo correcto es addEventListener
//guessSubmit.addeventListener('click', checkGuess);
  guessSubmit.addEventListener('click', checkGuess);

  Punto numero 11: Aligual que el punto 10, estaba mal escrito addeventListener, lo correcto es addEventListener
  //resetButton.addeventListener('click', resetGame);
    resetButton.addEventListener('click', resetGame);

Punto numero 12: Esta linea estaba mal escrita, se corrigió para obtener un numero aleatorio. 
//randomNumber = Math.floor(Math.random()) + 1;
    randomNumber = Math.floor(Math.random() * 100) + 1;