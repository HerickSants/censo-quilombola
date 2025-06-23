# 📤 Como Fazer Upload para o GitHub

## Passo 1: Criar Repositório no GitHub

1. **Acesse:** https://github.com/
2. **Faça login ou crie conta**
3. **Clique em "New repository"**
4. **Configure:**
   - **Repository name:** `censo-quilombola`
   - **Description:** `Aplicativo Android para censo quilombola`
   - **Public** ✅
   - **Não marque** "Add a README file"
5. **Clique em "Create repository"**

## Passo 2: Fazer Upload dos Arquivos

### Opção A: Upload pelo Navegador (Mais Fácil)

1. **No repositório criado, clique em "uploading an existing file"**
2. **Arraste TODOS os arquivos** da pasta `Projetos/CensoQuilombola/` para o GitHub
3. **Adicione uma mensagem:** "Initial commit - Censo Quilombola app"
4. **Clique em "Commit changes"**

### Opção B: Usando Git (Para Desenvolvedores)

```bash
# No terminal, na pasta do projeto:
git init
git add .
git commit -m "Initial commit - Censo Quilombola app"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/censo-quilombola.git
git push -u origin main
```

## Passo 3: Verificar o Build

1. **Vá para a aba "Actions"** no seu repositório
2. **Você verá um workflow rodando** (Build Android APK)
3. **Aguarde alguns minutos** para completar
4. **Clique no workflow** quando ficar verde
5. **Role para baixo** até "Artifacts"
6. **Clique em "app-debug"** para baixar o APK

## Passo 4: Configurar Firebase (Obrigatório)

**IMPORTANTE:** O APK não funcionará sem configurar o Firebase!

1. **Siga as instruções** no README-GITHUB.md
2. **Configure o Firebase** e Google Sheets
3. **Substitua os arquivos** `google-services.json` e `strings.xml`
4. **Faça novo commit** para gerar novo APK

## 🎯 Resultado

Após seguir estes passos, você terá:
- ✅ Repositório no GitHub
- ✅ Build automático do APK
- ✅ APK pronto para download
- ✅ Código fonte versionado

## 📱 Próximos Passos

1. **Baixe o APK** da seção Actions
2. **Configure o Firebase** (obrigatório)
3. **Teste no dispositivo Android**
4. **Compartilhe o repositório** com outros desenvolvedores

---

**Dúvidas? Abra uma issue no repositório!**
