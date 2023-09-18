# Calculadora criada em Python
from time import sleep

a = '\033[34mCALCULADORA\033[m' # cor azul

print('-=' * 15)
print(a.center(35))
print('-=' * 15)

print('''OPERAÇÕES:
[1] SOMA
[2] SUBTRAÇÃO
[3] MULTIPLICAÇÃO
[4] DIVISÃO''')

operacao = int(input('Escolha a operação: '))

print('Muito bem!')
sleep(1)
print('PROCESSANDO....')
sleep(1)

n1 = int(input('Digite o primeiro número: '))
n2 = int(input('Digite o segundo número: '))
print('CALCULANDO....')
sleep(1)

if operacao == 1:
    resultado = n1 + n2

if operacao == 2:
    resultado = n1 - n2

if operacao == 3:
    resultado = n1 * n2

if operacao == 4:
    resultado = n1 / n2

print(f'O resultado da operação é: \033[31m{resultado}\033[m')
