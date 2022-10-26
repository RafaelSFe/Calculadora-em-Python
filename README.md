def calculadora():
    operacao = input('''
Escolha o tipo de operção: :
+ Para soma
- Para subtração
* Para Multiplicação
/ Para Divisão
''')
    
    sinalAritimetico = input('Selecione o sinal: ')
    numero1 = int(input('por favor escolha o primeiro numero:  '))
    numero2 = int(input('Por favor escolha o segundo numero:  '))

    if operacao == '+':
        print('{} + {} = '.format(numero1, numero2))
        print(numero1 + numero2)

    elif operacao == '-':
        print('{} - {} = '.format(numero1, numero2))
        print(numero1 - numero2)

    elif operacao == '*':
        print('{} * {} = '.format(numero1, numero2))
        print(numero1 * numero2)

    elif operacao == '/':
        print('{} / {} = '.format(numero1, numero2))
        print(numero1 / numero2)

    else:
        print('Operador de numerico invalido, escolha um corretamente.')

   
    tenteNovamente()

def tenteNovamente():
    calculeNovamente1 = input('''
Você deseja tentar novamente? 
Pressione S para sim ou N para não.

''')

    if calculeNovamente1.upper() == 'S':
        ()
    elif calculeNovamente1() == 'N':
        print('Ate mais!!.')
    else:
        tenteNovamente()

calculadora()
