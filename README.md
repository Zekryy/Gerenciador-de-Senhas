# Gerenciador-de-Senhas
Este gerenciador de senhas é apenas um exemplo educacional e pode não ser adequado para uso em ambientes de produção sem ajustes adicionais de segurança.

# Gerenciador de Senhas em Python

Este é um simples gerenciador de senhas em Python que criptografa e armazena senhas de forma segura. Ele utiliza a biblioteca `cryptography` para criptografar e descriptografar as senhas.

## Funcionalidades

- Criptografa e armazena senhas de forma segura.
- Permite salvar e recuperar senhas para diferentes serviços.

## Pré-requisitos

- Python 3.x instalado.

## Instalação

1. Clone ou faça o download deste repositório.

2. Certifique-se de ter o Python 3.x instalado em seu sistema.

3. Instale as dependências executando o seguinte comando no terminal:

   pip install cryptography

   

## Como usar

1. Execute o arquivo `main.py` para iniciar o gerenciador de senhas.

2. O gerenciador de senhas irá solicitar que você insira informações sobre o serviço, como nome de usuário e senha.

3. As senhas serão armazenadas criptografadas de forma segura.

4. Você pode recuperar suas senhas posteriormente fornecendo o nome do serviço.

## Exemplo de Utilização

```python
pm = PasswordManager()
pm.save_password("exemplo_servico", "exemplo_usuario", "exemplo_senha")
usuario, senha = pm.get_password("exemplo_servico")
if usuario and senha:
    print(f"Usuário: {usuario}, Senha: {senha}")
else:
    print("Serviço não encontrado ou senha não definida.")
