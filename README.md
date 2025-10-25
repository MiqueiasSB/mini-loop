# ⚡ Mini Loop  

Um aplicativo de **hábitos atômicos minimalista**, criado com **Ionic Framework** e **Vue 3**, projetado para ajudar você a construir rotinas poderosas por meio de pequenas ações diárias.  
Com foco em simplicidade, leveza e design limpo, o Mini Loop busca tornar o acompanhamento de hábitos uma experiência fluida e intuitiva.  

---

## 🧩 Tecnologias Utilizadas  

- ⚙️ **Ionic Framework** — Interface responsiva e nativa para web e mobile.  
- 🧠 **Vue 3** — Framework progressivo e reativo para construção da interface.  
- ⚡ **Capacitor** — Permite acesso a recursos nativos dos dispositivos móveis.  
- 📦 **Node.js / NPM** — Ambiente e gerenciamento de dependências.  

---

## 🚀 Instalação e Execução  

### 📋 Pré-requisitos  

Certifique-se de ter instalado em seu sistema:  

- [Node.js](https://nodejs.org/) (versão LTS recomendada)  
- [NPM](https://www.npmjs.com/)  
- [Git](https://git-scm.com/)  

---

### 🧰 Passo a passo  

1. **Instale o Ionic CLI e os assets do Capacitor globalmente:**  
   ```bash
   npm install -g @ionic/cli @capacitor/assets
   ```

2. **Clone o repositório:**  
   ```bash
   git clone https://github.com/MiqueiasSB/mini-loop.git mini-loop
   ```

3. **Acesse a pasta do projeto:**  
   ```bash
   cd mini-loop
   ```

4. **Instale as dependências:**  
   ```bash
   npm install
   ```

5. **Inicie o servidor de desenvolvimento:**  
   ```bash
   ionic serve
   ```

   O aplicativo será iniciado e aberto automaticamente no navegador em [http://localhost:8100](http://localhost:8100).  

---

## 📱 Executar no Dispositivo (opcional)

Para rodar o app em um dispositivo Android ou iOS:  

```bash
ionic build
npx cap add android
npx cap open android
```

> 🧩 É necessário ter o **Android Studio** ou o **Xcode** instalado para executar o projeto nativo.  

---

## 🧠 Comandos Úteis  

| Ação | Comando |
|------|----------|
| Atualizar dependências | `npm update` |
| Criar build de produção | `ionic build` |
| Sincronizar Capacitor | `npx cap sync` |
| Iniciar servidor local | `ionic serve` |

