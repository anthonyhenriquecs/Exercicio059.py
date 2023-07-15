# Exercicio059.py

from  time import sleep
n1 = int(input('Digite o primeiro valor:'))
n2 = int(input('Digite o segundo valor:'))
opcao = 0
while opcao != 5:
    print('''    [ 1 ] somar
    [ 2 ] multiplicar
    [ 3 ] mostar o maior
    [ 4 ] digitar novos numeros
    [ 5 ] sair do programa''')
    opcao = int(input('Qual a sua escolha?'))
    if opcao == 1:
        soma = n1 + n2
        print('A soma de {} e {} é: {}'.format(n1,n2,soma))
    elif opcao == 2:
        mult = n1 * n2
        print('A multiplicação de {} e {} é: {}'.format(n1, n2, mult))
    elif opcao == 3:
        if n1 > n2:
            maior = n1
        else:
            maior = n2
        print('Entre {} e {} o maior é:{}'.format(n1,n2,maior))
    elif opcao == 4:
        print('Informe os numeros novamente:')
        n1 = int(input('Digite um novo numero:'))
        n2 = int(input('Digite outro numero:'))
    elif opcao == 5:
        print('Finalizando...')
    else:
        print('Opção invalida, tente novamente')
    print('=-=' * 10)
    sleep(2)
print('Fim do programa, volte sempre!')
