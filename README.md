# Calculadora2.0
def calculadora():
    while True:
        print("Operações disponíveis:")
        print("1: Soma")
        print("2: Subtração")
        print("3: Multiplicação")
        print("4: Divisão")
        print("0: Sair")
        
        escolha = input("Digite o número para a operação correspondente: ")

        if escolha == '0':
            print("Saindo da calculadora.")
            break
        
        if escolha not in ['1', '2', '3', '4']:
            print("Essa opção não existe.")
            continue

        num1 = float(input("Digite o primeiro valor: "))
        num2 = float(input("Digite o segundo valor: "))

        if escolha == '1':
            print("Resultado da soma:", num1 + num2)
        elif escolha == '2':
            print("Resultado da subtração:", num1 - num2)
        elif escolha == '3':
            print("Resultado da multiplicação:", num1 * num2)
        elif escolha == '4':
            if num2 != 0:
                print("Resultado da divisão:", num1 / num2)
            else:
                print("Erro: Divisão por zero!")
        print()  # Adiciona uma linha em branco para melhorar a legibilidade


