# Número primos

A new flutter proyect 


Para este ejercicio se usado una función que nos permita validar que el número sea primo y una función que genere el listado. 

## _checkPrimerNumber()

Esta es una función que comprueba si es un número primo y retorna un valor booleano. 

```javascript
 bool _checkPrimerNumber(int value) {
    bool primo = true;
    for (var i = 2; i < value; i++) {
      if (value % i == 0) {
        primo = false;
        break;
      }
    }
    return primo;
  }
```


## _generateNumbers()

Esta es una función que nos permite mostrar los números primos que se encuentran en entre 1 y 100 se ha usado la función _generateNumbers la cual es una función que realiza un ciclo while, a la vez que va guardando un string con los números primos. 


```javascript
 int _start = 1;
 int _end = 100;
 String _values = "";

 void _generateNumbers() {
    while (_start < _end) {
      if (_checkPrimerNumber(_start)) {
        setState(() {
          _values += _start.toString() + "   ";
        });
      }
      _start++;
    }
  }

```
## Código 

![App Screenshot](https://raw.githubusercontent.com/CarlosMaldonado1998/flutter-prime-number/master/Images/function.png)

## Imágenes 

![App Screenshot](https://raw.githubusercontent.com/CarlosMaldonado1998/flutter-prime-number/master/Images/app.png)
![App Screenshot](https://raw.githubusercontent.com/CarlosMaldonado1998/flutter-prime-number/master/Images/app2.png)

