# Configuração do Cloudflare Pages para HouseRevive

## 🚀 Hospedar o Site Diretamente no Domínio do Cloudflare

### Passo 1: Criar o Projeto no Cloudflare Pages
- Acesse o painel do Cloudflare.
- No menu lateral esquerdo, clique em **Pages**.
- Clique em **Criar um projeto** (Create a project).

### Passo 2: Conectar seu Repositório Git
- Escolha **GitHub** ou **GitLab** (onde você armazenou o código HTML do site).
- Conecte sua conta ao Cloudflare e escolha o repositório criado para a House Revive.

### Passo 3: Definir Branch e Diretório
- Em **Ramificação de produção** (Production Branch), escolha a branch principal (ex: main ou master).
- Em **Diretório de build** (Build output directory), deixe em branco se o arquivo index.html estiver na raiz.

### Passo 4: Realizar o Deploy
- Clique no botão **Deploy**.
- Aguarde alguns segundos até aparecer "Success".

## 🌐 Conectar o Domínio existente ao Cloudflare Pages

### Passo 1:
- Após o deploy, clique em **Custom Domains** dentro do seu projeto no Cloudflare Pages.

### Passo 2:
- Clique em **Set up a custom domain** e insira o domínio que você já tem (ex: houserevive.pt).

### Passo 3 (DNS automático):
- Como seu domínio já está no Cloudflare, ele configurará automaticamente o DNS.
- Clique em **Confirmar**. Em poucos minutos, estará pronto.

## 🔒 SSL Automático
- O Cloudflare oferece automaticamente SSL (HTTPS) gratuito, seguro e ativado automaticamente após a conexão do domínio.

## Configuração Adicional (Opcional)

1. **Configuração SSL/TLS**
   - No dashboard do domínio, vá para a seção "SSL/TLS"
   - Recomendado: Use a opção "Full" ou "Full (strict)"
   - Verifique se o certificado SSL foi provisionado automaticamente

2. **Configurações adicionais recomendadas**
   - Ative o "Always Use HTTPS"
   - Configure regras de Page Rules conforme necessário
   - Ative o cache de borda para melhor performance
