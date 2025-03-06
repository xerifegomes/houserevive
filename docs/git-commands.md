
# Comandos Git para o projeto House Revive

## Comandos prontos para copiar e colar

Abra o terminal e execute os seguintes comandos:

```bash
# Navegar até a pasta do projeto
cd /Users/isheriffgomes/sites/houserevive/houserevive

# Inicializar o repositório Git
git init

# Criar arquivo .gitignore básico
cat > .gitignore << EOL
.DS_Store
node_modules/
.env
.env.local
*.log
EOL

# Adicionar todos os arquivos ao Git (exceto os ignorados)
git add .

# Fazer o primeiro commit
git commit -m "Versão inicial do site House Revive"

# Criar a branch main (se ainda estiver usando master como padrão)
git branch -M main

# Adicionar o repositório remoto (substitua com seu nome de usuário)
git remote add origin https://github.com/isheriffgomes/house-revive.git

# Enviar o código para o GitHub
git push -u origin main
```

## Verificação

Após executar estes comandos, seu código estará no GitHub. Verifique acessando:
https://github.com/isheriffgomes/house-revive

## Se precisar fazer alterações depois

```bash
# Após fazer alterações nos arquivos
git add .
git commit -m "Descrição das alterações realizadas"
git push
```

## Se tiver problemas com autenticação

```bash
# Configure suas credenciais
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@example.com"

# Se precisar usar token ao invés de senha
git remote set-url origin https://seu-usuario:seu-token@github.com/isheriffgomes/house-revive.git
```
