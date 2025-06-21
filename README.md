# 📱 Censo Quilombola - App Android

Aplicativo Android para coleta e análise de dados de censo em comunidades quilombolas.

## 🚀 Download do APK

O APK é compilado automaticamente pelo GitHub Actions. Para baixar:

1. **Vá para a aba "Actions"** neste repositório
2. **Clique no último workflow executado** (verde)
3. **Role para baixo** até "Artifacts"
4. **Clique em "app-debug"** para baixar o APK

## 📋 Funcionalidades

- 🔐 **Login com Google** - Autenticação via Firebase
- 📝 **Nova Pesquisa** - Formulário para coleta de dados
- 📊 **Visualização de Dados** - Gráficos e estatísticas
- ✏️ **Edição de Pesquisa** - Personalização das perguntas
- 📤 **Compartilhamento** - Envio via Email e WhatsApp
- 📄 **Exportação PDF** - Relatórios em PDF

## 🛠️ Tecnologias

- **Kotlin** + **Android**
- **Firebase Authentication** (Google Sign-in)
- **Google Sheets** + **Apps Script** (Backend)
- **Retrofit** (Chamadas HTTP)
- **MPAndroidChart** (Gráficos)
- **ViewBinding** (Interface)

## 📱 Como Instalar

1. **Baixe o APK** da seção Actions
2. **Ative "Fontes desconhecidas"** nas configurações do Android
3. **Instale o APK** no seu dispositivo
4. **Configure o Firebase** (veja instruções abaixo)

## ⚙️ Configuração Necessária

### Firebase Setup
1. Crie um projeto no [Firebase Console](https://console.firebase.google.com/)
2. Adicione um app Android com package: `com.grixo.censoquilombola`
3. Baixe `google-services.json` e coloque na pasta `app/`
4. Ative Google Sign-in na seção Authentication
5. Crie um app Web e copie o Web Client ID
6. Substitua o Web Client ID em `app/src/main/res/values/strings.xml`

### Google Sheets Setup
1. Crie uma planilha no Google Sheets
2. Adicione cabeçalhos: `Sexo`, `Idade`, `Escolaridade`, `Data`
3. Vá em Extensões > Apps Script
4. Cole o código do Apps Script fornecido
5. Publique como Web App
6. Copie a URL e substitua em `RetrofitClient.kt`

## 🔄 Build Automático

Este repositório usa GitHub Actions para compilar automaticamente o APK sempre que houver mudanças no código.

## 📞 Suporte

Para dúvidas ou problemas, abra uma issue neste repositório.

---

**Desenvolvido com ❤️ para comunidades quilombolas**
