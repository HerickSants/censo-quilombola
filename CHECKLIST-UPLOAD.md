# ✅ Checklist - Arquivos para Upload no GitHub

## 📁 Estrutura Completa do Projeto

```
CensoQuilombola/
├── 📄 .gitignore                    ✅
├── 📄 build.gradle                  ✅
├── 📄 settings.gradle               ✅
├── 📄 gradlew.bat                   ✅
├── 📄 README.md                     ✅
├── 📄 README-GITHUB.md              ✅
├── 📄 upload-to-github.md           ✅
├── 📄 build-online.md               ✅
├── 📄 CHECKLIST-UPLOAD.md           ✅
├── 📁 .github/
│   └── 📁 workflows/
│       └── 📄 build.yml             ✅
├── 📁 gradle/
│   └── 📁 wrapper/
│       └── 📄 gradle-wrapper.properties ✅
└── 📁 app/
    ├── 📄 build.gradle              ✅
    ├── 📄 google-services.json      ⚠️ (ADICIONAR DEPOIS)
    └── 📁 src/
        └── 📁 main/
            ├── 📄 AndroidManifest.xml ✅
            ├── 📁 java/com/grixo/censoquilombola/
            │   ├── 📄 SplashActivity.kt ✅
            │   ├── 📄 LoginActivity.kt ✅
            │   ├── 📄 MainActivity.kt ✅
            │   ├── 📄 NewSurveyActivity.kt ✅
            │   ├── 📄 ViewDataActivity.kt ✅
            │   ├── 📄 EditSurveyActivity.kt ✅
            │   ├── 📁 api/
            │   │   ├── 📄 GoogleSheetsApi.kt ✅
            │   │   └── 📄 RetrofitClient.kt ✅
            │   └── 📁 data/
            │       └── 📄 SurveyData.kt ✅
            └── 📁 res/
                ├── 📁 layout/
                │   ├── 📄 activity_splash.xml ✅
                │   ├── 📄 activity_login.xml ✅
                │   ├── 📄 activity_main.xml ✅
                │   ├── 📄 activity_new_survey.xml ✅
                │   ├── 📄 activity_view_data.xml ✅
                │   └── 📄 activity_edit_survey.xml ✅
                ├── 📁 values/
                │   └── 📄 strings.xml ✅
                ├── 📁 drawable/       ✅
                └── 📁 layout/         ✅
```

## 🚀 Passos para Upload

### 1. Criar Repositório no GitHub
- [ ] Acessar https://github.com/
- [ ] Criar novo repositório: `censo-quilombola`
- [ ] Configurar como público

### 2. Fazer Upload dos Arquivos
- [ ] Arrastar TODA a pasta `CensoQuilombola` para o GitHub
- [ ] Adicionar mensagem: "Initial commit - Censo Quilombola app"
- [ ] Fazer commit

### 3. Verificar Build Automático
- [ ] Ir para aba "Actions"
- [ ] Aguardar workflow "Build Android APK"
- [ ] Verificar se ficou verde (sucesso)
- [ ] Baixar APK da seção "Artifacts"

### 4. Configurar Firebase (OBRIGATÓRIO)
- [ ] Adicionar `google-services.json` na pasta `app/`
- [ ] Atualizar `strings.xml` com Web Client ID
- [ ] Fazer novo commit para gerar APK funcional

## ⚠️ Arquivos Importantes

### Arquivos que DEVEM ser enviados:
- ✅ Todos os arquivos `.kt` (código fonte)
- ✅ Todos os arquivos `.xml` (layouts)
- ✅ Arquivos de configuração Gradle
- ✅ GitHub Actions workflow
- ✅ README e documentação

### Arquivos que NÃO devem ser enviados:
- ❌ `google-services.json` (contém credenciais)
- ❌ Pasta `build/` (gerada automaticamente)
- ❌ Arquivos `.iml` (Android Studio)

## 📱 Após o Upload

1. **O GitHub Actions compilará automaticamente** o APK
2. **Baixe o APK** da seção Actions
3. **Configure o Firebase** (obrigatório para funcionar)
4. **Teste no dispositivo Android**

## 🔧 Configuração Firebase

**IMPORTANTE:** Sem o Firebase configurado, o app não funcionará!

1. Configure o projeto no Firebase Console
2. Adicione o `google-services.json`
3. Atualize o Web Client ID
4. Faça novo commit

---

**✅ Todos os arquivos estão prontos para upload!**
