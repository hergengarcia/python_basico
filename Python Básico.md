### Python Básico
- Python é uma linguagem de propósito geral, utilizado para aplicações ao ramo do machine learning e da ciência de dados. Estudando os comandos de programação específicos para a área, estará apto a usar essa linguagem no dia a dia.

#### Formatando no Python


```python
fruta = 'limao'
saldo = 100
```


```python
print('Suco de %s é meu favorito!' %fruta)
```

    Suco de limao é meu favorito!
    


```python
print('Valor do saldo é: %d' %saldo)
```

    Valor do saldo é: 100
    


```python
print('Valor do saldo é: %f' %saldo)
```

    Valor do saldo é: 100.000000
    


```python
print('Suco de {} é meu favorito!'.format(fruta))
```

    Suco de limao é meu favorito!
    


```python
print('O Valor {:.2f} é o saldo!'.format(saldo))
```

    O Valor 100.00 é o saldo!
    


```python
valor1 = 21
valor2 = 501
valor3 = 100
```


```python
print('O valor1 é: {0}, o valor2 é: {1} e o valor3 é: {2} '.format(valor1,valor2,valor3))
```

    O valor1 é: 25, o valor2 é: 50 e o valor3 é: 100 
    


```python
conta = valor2 / valor1
print(conta)
```

    23.857142857142858
    


```python
print('Resultado: {:.2f}'.format(conta))
```

    Resultado: 23.86
    

#### Condicionais no Python


```python
alimento = 'pao'
if alimento == 'pizza':
    print('A comida {}'.format(alimento), 'possui muitas calorias')
else:
    print('A comida {}'.format(alimento), 'possui poucas calorias')

```

    A comida pao possui poucas calorias
    


```python
valor = 100
if valor == 100:
    print('Valor igual a 100:', valor)
elif valor < 100:
    print('Valor menor que 100:', valor)
elif valor > 100:
    print('Valor maior que 100:', valor)
else:
    print('Valor desconhecido:', valor)
```

    Valor igual a 100: 100
    

Ex.1 - Calcular se o usuario é adulto.


```python
ano_atual = 2021
ano_nasc = int(input('Qual seu ano de nascimento? '))
idade = (ano_atual - ano_nasc)
if idade >= 18:
    print(f'Você é adulto, você tem {idade} anos')
else:
    print(f'Você não é adulto, você tem {idade} anos')
```

    Qual seu ano de nascimento? 1973
    Você é adulto, você tem 48 anos
    

#### Loops com "for in range" no Python


```python
a = 0
for i in range(5):
    print(i)
    a = a + 1
print('O Valor de i é:', i)
print('O Valor de a é:', a)
```

    0
    1
    2
    3
    4
    O Valor de i é: 4
    O Valor de a é: 5
    


```python
a = 0
b = 10
for i in range(a,b):
    print('Frase')
```

    Frase
    Frase
    Frase
    Frase
    Frase
    Frase
    Frase
    Frase
    Frase
    Frase
    


```python
palavra = 'Familia'
for i in palavra:
    print(i)
```

    F
    a
    m
    i
    l
    i
    a
    


```python
lista = [2,9,11,'py',55,'data']   
for num in lista:
    print(num)
```

    2
    9
    11
    py
    55
    data
    

#### Utilizando os comandos While e Break em Python
- executa comando enquanto tive satifeista a condição


```python
import time
contador = 0
while contador < 10:
    print('Não concluido a condição!')
    print(contador)
    contador = contador + 1
    if contador == 6:
        break
    time.sleep(1)
print('Concluida a condição!')
```

    Não concluido a condição!
    0
    Não concluido a condição!
    1
    Não concluido a condição!
    2
    Não concluido a condição!
    3
    Não concluido a condição!
    4
    Não concluido a condição!
    5
    Concluida a condição!
    

Ex.2 - Calculando o fatorial do numero fornecido pelo usuario.
- 4! = 4*3*2*1


```python
num = int(input('Digite um número inteiro qualquer menor que 10: '))
contador = 1
fat = num
while (num-contador) >= 1:
    fat = fat*(num-contador)
    contador = contador + 1
print('{}! = {}'.format(num, fat))
```

    Digite um número inteiro qualquer menor que 10: 5
    5! = 120
    

##### Usando módulos e bibliotecas


```python
import math
math.factorial(5)
```




    120




```python
import datetime
datetime.date.today() # biblioteca.modulo.função
```




    datetime.date(2021, 5, 5)




```python
from datetime import date
date.isoformat(date.today())
```




    '2021-05-05'



#### Definindo Funções em Python


```python
def texto():
    print('A soma dos valores 2 + 2 = 4:')
```


```python
texto() # chamando a função
```

    A soma dos valores 2 + 2 = 4:
    


```python
def temLetraA():
    frase = input('Digite uma frase: ')
    if 'a' in frase:
        print('A Frase tem a letra a: ')
    else:
        print('A Frase não tem a letra: a')
```


```python
temLetraA()
```

    Digite uma frase: querer é poder
    A Frase não tem a letra: a
    


```python
def somaQadrados(a,b):
    somaQ = a**2 + b**2
    return somaQ
```


```python
somaQadrados(1,2) # chamando a função com parametros
```




    5




```python

```
