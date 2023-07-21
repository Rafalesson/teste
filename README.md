## 1° Desenvolva um código Python que lê do teclado nome e a idade atual de uma pessoa. Como saída, imprima o ano em que a pessoa completará 100 anos de idade

    import datetime

    # Solicitar nome e idade
    nome = input("Digite o nome da pessoa: ")
    idade_atual = int(input("Digite a idade atual da pessoa: "))

    # Calcular o ano em que a pessoa completará 100 anos
    ano_atual = datetime.datetime.now().year
    ano_completar_100 = ano_atual + (100 - idade_atual)

    # Imprimir o resultado
    print(ano_completar_100)
---

# 1° Escreva um código Python para verificar se três números digitados na entrada padrão são pares ou ímpares. Para cada número, imprima como saída Par: ou Ímpar: e o número correspondente (um linha para cada número lido).

    # Ler os números da entrada padrão
    numeros = []
    for i in range(3):
        numero = int(input("Digite um número: "))
        numeros.append(numero)

    # Verificar se cada número é par ou ímpar e imprimir o resultado
    for numero in numeros:
        if numero % 2 == 0:
            print("Par:", numero)
        else:
            print("Ímpar:", numero)