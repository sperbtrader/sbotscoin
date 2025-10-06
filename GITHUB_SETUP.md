# 📦 Guia de Setup no GitHub

Este guia explica como configurar o repositório no GitHub e fazer deploy do site.

---

## 🚀 Passo 1: Criar Repositório no GitHub

1. Acesse [GitHub](https://github.com) e faça login
2. Clique em **"New repository"** (ou acesse https://github.com/new)
3. Configure o repositório:
   - **Repository name:** `sbotscoin-website` (ou o nome que preferir)
   - **Description:** `🤖 SBOTS - Token $SBOTS Liquidez Alimentada por Performance | Site Oficial`
   - **Visibility:** Public
   - **NÃO** marque "Initialize this repository with a README" (já temos um)
4. Clique em **"Create repository"**

---

## 📁 Passo 2: Upload dos Arquivos

### Opção A: Via Interface Web (Mais Fácil)

1. Na página do repositório recém-criado, clique em **"uploading an existing file"**
2. Arraste e solte todos os arquivos:
   - `index.html`
   - `logo-token.png`
   - `README.md`
   - `LICENSE`
   - `.gitignore`
3. Adicione uma mensagem de commit: `🚀 Initial commit - SBOTS Website`
4. Clique em **"Commit changes"**

### Opção B: Via Git CLI (Linha de Comando)

```bash
# Navegue até a pasta do projeto
cd sbotscoin-website

# Inicialize o repositório Git
git init

# Adicione todos os arquivos
git add .

# Faça o primeiro commit
git commit -m "🚀 Initial commit - SBOTS Website"

# Adicione o repositório remoto (substitua SEU_USUARIO pelo seu username)
git remote add origin https://github.com/SEU_USUARIO/sbotscoin-website.git

# Renomeie a branch para main (se necessário)
git branch -M main

# Envie os arquivos para o GitHub
git push -u origin main
```

---

## 🌐 Passo 3: Ativar GitHub Pages (Deploy Gratuito)

1. No repositório, vá em **Settings** (Configurações)
2. No menu lateral, clique em **Pages**
3. Em **Source**, selecione:
   - Branch: `main`
   - Folder: `/ (root)`
4. Clique em **Save**
5. Aguarde alguns minutos e seu site estará disponível em:
   ```
   https://SEU_USUARIO.github.io/sbotscoin-website/
   ```

---

## 🎨 Estrutura dos Arquivos

```
sbotscoin-website/
│
├── index.html          # ⭐ Site principal (arquivo único com tudo)
├── logo-token.png      # 🖼️ Logo oficial do token (705KB)
├── README.md           # 📖 Documentação do projeto
├── LICENSE             # ⚖️ Licença MIT
├── .gitignore          # 🚫 Arquivos ignorados pelo Git
└── GITHUB_SETUP.md     # 📋 Este guia
```

---

## 📝 Informações Importantes

### Nome da Logo
**Salve a imagem como:** `logo-token.png`

Este é o nome usado no README.md para exibir a logo no topo do repositório.

### Arquivo HTML
O arquivo `index.html` contém:
- ✅ Todo o HTML, CSS e JavaScript
- ✅ Logo do token incorporada em base64
- ✅ Todas as animações SVG
- ✅ Integração com API do Pump.fun
- ✅ Totalmente funcional sem dependências externas

### Tamanho dos Arquivos
- `index.html`: 996KB (logo incorporada em base64)
- `logo-token.png`: 705KB (imagem original para o README)

---

## 🔧 Atualizações Futuras

Para atualizar o site no futuro:

### Via Interface Web:
1. Acesse o arquivo no GitHub
2. Clique no ícone de lápis (Edit)
3. Faça as alterações
4. Commit changes

### Via Git CLI:
```bash
# Faça as alterações nos arquivos localmente

# Adicione as mudanças
git add .

# Faça o commit
git commit -m "Descrição das mudanças"

# Envie para o GitHub
git push origin main
```

---

## 🌟 Dicas Extras

### Domínio Personalizado
Se quiser usar um domínio próprio (ex: `sbots.io`):
1. Vá em **Settings > Pages**
2. Em **Custom domain**, adicione seu domínio
3. Configure o DNS do seu domínio apontando para o GitHub Pages

### Badges no README
O README já inclui badges bonitas. Para personalizar:
- Acesse [shields.io](https://shields.io) para criar badges customizadas

### Analytics
Para adicionar Google Analytics ou similar:
1. Edite o `index.html`
2. Adicione o código de tracking antes do `</head>`

---

## ❓ Problemas Comuns

### Site não carrega após deploy
- Aguarde 5-10 minutos após ativar o GitHub Pages
- Limpe o cache do navegador (Ctrl+Shift+R)
- Verifique se o arquivo se chama exatamente `index.html`

### Logo não aparece no README
- Certifique-se que o arquivo se chama `logo-token.png`
- Verifique se está na raiz do repositório
- Aguarde alguns minutos para o GitHub processar

### Erro ao fazer push
- Verifique se você tem permissão no repositório
- Confirme que adicionou o remote correto
- Tente fazer login novamente: `git config --global user.name "Seu Nome"`

---

## 📞 Suporte

Se tiver dúvidas:
- 📖 [Documentação do GitHub Pages](https://docs.github.com/pages)
- 💬 [GitHub Community](https://github.community)
- 🐦 Twitter: [@sbots](https://twitter.com/sbots)

---

<div align="center">

**Boa sorte com o projeto SBOTS! 🚀**

</div>
