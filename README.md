# Projeto Banco Simples

## Descrição

Este é um projeto simples de um sistema bancário implementado em Python. O objetivo principal é oferecer funcionalidades básicas de um banco, como criação de usuários, criação de contas, saques, depósitos e exibição de extratos. O sistema é baseado em um menu de texto interativo que permite ao usuário navegar entre as opções disponíveis.

## Funcionalidades

1. **Sacar**: Permite ao usuário realizar saques, respeitando o limite diário de saques e o saldo disponível.
2. **Depósito**: Permite ao usuário realizar depósitos em sua conta.
3. **Extrato**: Exibe o extrato com as movimentações da conta.
4. **Criar Usuário**: Permite criar um novo usuário fornecendo CPF, nome, data de nascimento, endereço e senha.
5. **Criar Conta**: Permite criar uma nova conta associada a um usuário existente.
6. **Listar Contas**: Exibe todas as contas criadas, com a opção de buscar por nome ou CPF.
7. **Sair**: Encerra o programa.

## Estrutura do Código

O código está organizado em diversas funções para facilitar a manutenção e o entendimento:

- `menuBanco()`: Exibe o menu principal.
- `criar_usuario(usuarios)`: Cria um novo usuário e adiciona à lista de usuários.
- `verificar_usuario(cpf, senha, usuarios)`: Verifica se um usuário existe com base no CPF e senha fornecidos.
- `verificar_cpf(cpf, usuarios)`: Verifica se um CPF já está cadastrado.
- `criar_conta(usuarios, agencia, numero_conta, contas)`: Cria uma nova conta para um usuário existente.
- `listar_contas(contas)`: Lista todas as contas ou busca por um CPF ou nome específico.
- `sacar(*, limite, extrato, numeroSaques, limiteSaque, saldo, valor)`: Realiza um saque, respeitando os limites de saque e saldo.
- `depositar(saldo, extrato, valor, /)`: Realiza um depósito.
- `exbExtrato(saldo, /, *, extrato)`: Exibe o extrato das movimentações.
- `limparTela()`: Limpa a tela do terminal.
- `main()`: Função principal que gerencia o loop do menu e chama as demais funções conforme a opção selecionada.

## Como Executar

1. Certifique-se de ter o Python instalado em sua máquina.
2. Clone este repositório.
3. Navegue até o diretório do projeto.
4. Execute o script `main.py`:
   ```bash
   python main.py
   ```

## Observações

- O sistema não utiliza um banco de dados real; todos os dados são armazenados em listas na memória enquanto o programa está em execução.
- Para fins de simplicidade, a verificação do CPF e da senha é feita de forma básica e não há criptografia de senha.

## Melhorias Futuras

- Implementar um banco de dados para persistência dos dados.
- Adicionar validações mais robustas para CPF, datas e outros campos.
- Implementar criptografia para as senhas.
- Melhorar a interface do usuário.
- Adicionar testes unitários para garantir a integridade do sistema.

## Curso

Este projeto faz parte do curso Python AI Backend Developer da DIO.io.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests com melhorias e correções.

## Licença

Este projeto está licenciado sob a Licença MIT. Veja o arquivo LICENSE para mais detalhes.

---

Este projeto foi desenvolvido como um exercício de programação para aprender e praticar conceitos básicos de Python e lógica de programação. Espero que seja útil e que sirva como uma base para projetos mais complexos no futuro.
