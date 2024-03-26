
print("\nBem Vindo Ao Programa Do Mestre")

# Cadastro de Pessoas
# Crie uma lista para armazenar os dados das pessoas
pessoas = []

while True:
    print("\n1 - Cadastrar pessoa")
    print("2 - Listar pessoas cadastradas")
    print("3 - Sair")

    opcao = input("Escolha uma opção: ")

    if opcao == "1":
        # Cadastrar uma nova pessoa
        nome = input("\nDigite o nome da pessoa: ")
        idade = input("Digite a idade da pessoa: ")
        cpf = input("Digite o seu CPF: ")

        # Adicione os dados da pessoa à lista
        pessoas.append({"nome": nome, "idade": idade, "cpf": cpf})
        print(f"\n{nome} foi cadastrado com sucesso!\n")

    elif opcao == "2":
        # Listar pessoas cadastradas
        print("\nPessoas cadastradas:")
        for pessoa in pessoas:
            print(f"Nome: {pessoa['nome']}, Idade: {pessoa['idade']}, Cpf: {pessoa["cpf"]}")

    elif opcao == "3":
        # Sair do programa
        print("\nPrograma encerrando. Até logo!")
        break

    else:
        print("Opção inválida. Tente novamente.\n")
