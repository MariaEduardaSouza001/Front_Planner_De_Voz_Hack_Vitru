<div align="center">

# 🎓 SOFIA & EDU — Chat Acadêmico Inteligente

> Assistente conversacional para planejamento de estudos, desenvolvida no **Hackathon Vitru Educação**

[![Status](https://img.shields.io/badge/status-demo-yellow?style=flat-square)](.)
[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](.)
[![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](.)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](.)
[![License](https://img.shields.io/badge/licen%C3%A7a-MIT-green?style=flat-square)](.)

</div>

---

## 📖 Sobre o Projeto

**SOFIA & EDU** é o front-end de uma assistente acadêmica conversacional desenvolvida durante o Hackathon Vitru Educação. A aplicação permite que estudantes interajam com uma IA de planejamento de estudos por meio de chat, comandos de voz e sugestões inteligentes.

A solução contempla duas identidades visuais distintas:

| Marca | Assistente | Tema |
|-------|-----------|------|
| **UNIASSELVI** | Sofia | Amarelo / Preto |
| **UniCesumar** | Edu | Azul |

---

## ✨ Funcionalidades

- 💬 **Chat conversacional** — envio de mensagens com digitação animada e scroll automático
- 🎨 **Multi-brand** — alternância de tema, avatar e nome da assistente por instituição
- 📚 **Plano de Estudos** — card interativo com checklist de tarefas, barra de progresso e reagendamento
- 🏆 **Sistema de Recompensas** — acúmulo de pontos (+50 pts) ao concluir atividades
- 🎤 **Gravação de Voz** — compositor com suporte a `MediaRecorder` para envio de áudio
- 🔊 **Modo "Ouvir"** — animação de fala (integração com TTS preparada)
- 📎 **Anexar Arquivo** — visualização do arquivo no chat (análise via IA planejada)
- ⚡ **Quick Replies** — atalhos de resposta rápida para ações frequentes
- 💾 **Persistência Local** — tema e pontos salvos via `localStorage`
- ♿ **Acessibilidade** — suporte a navegação por teclado, skip link e atributos ARIA

---

## 🗂️ Estrutura do Projeto

```
Front_Planner_De_Voz_Hack_Vitru-main/
├── README.md
└── sofia&Edu-chat/
    ├── index.html          # Entrada principal da aplicação
    ├── css/
    │   └── style.css       # Estilos globais, temas e responsividade
    ├── js/
    │   └── script.js       # Lógica da aplicação (IIFE)
    └── Img/
        ├── sofia.png       # Avatar — Sofia (UNIASSELVI)
        └── edu.png         # Avatar — Edu (UniCesumar)
```

---

## 🛠️ Tech Stack

| Camada | Tecnologia |
|--------|-----------|
| Estrutura | HTML5 semântico |
| Estilização | CSS3 (variáveis, temas, responsivo) |
| Lógica | JavaScript ES6+ (Vanilla, IIFE) |
| Tipografia | Google Fonts — Inter |
| Armazenamento | `localStorage` |
| Áudio | `MediaRecorder` / `getUserMedia` |
| Framework | Nenhum — zero dependências |

---

## 🚀 Como Rodar

### Opção 1 — Abrir direto no navegador

Abra o arquivo `sofia&Edu-chat/index.html` diretamente no seu browser.

> ⚠️ Para usar o microfone, é necessário servir via `localhost` ou HTTPS (restrição do browser).

### Opção 2 — Live Server (recomendado)

Se você usa o **VS Code**:

1. Instale a extensão [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
2. Clique com o botão direito em `index.html`
3. Selecione **"Open with Live Server"**

### Opção 3 — Servidor HTTP local

```bash
# Python 3
python -m http.server 8080

# Node.js (com npx)
npx serve sofia&Edu-chat
```

Acesse: `http://localhost:8080`

---

## 🔌 Integrações Planejadas

O projeto foi estruturado para facilitar a integração futura com serviços de IA e backend:

| Funcionalidade | Hook no código | Status |
|---------------|---------------|--------|
| Respostas da IA | `receiveMessage()` → `fetch("/api/sofia")` | 🔜 Planejado |
| Text-to-Speech | Botão "Ouvir" → stream de áudio | 🔜 Planejado |
| Transcrição de Voz | Envio do blob de áudio | 🔜 Planejado |
| Análise de Arquivo | Upload + processamento | 🔜 Planejado |
| Calendário | Exportação `.ics` / Google Calendar | 🔜 Planejado |

> Atualmente, as respostas são geradas via correspondência de palavras-chave (`DEMO_REPLIES`) para fins de demonstração.

---

## 🎯 Roadmap

- [x] Interface de chat responsiva com dual-brand
- [x] Plano de estudos interativo com checklist
- [x] Sistema de recompensas com pontos
- [x] Gravação e envio de áudio
- [x] Persistência de estado via `localStorage`
- [ ] Integração com API de IA (LLM)
- [ ] Text-to-Speech (TTS) para respostas faladas
- [ ] Transcrição automática de áudio (STT)
- [ ] Backend com autenticação e histórico de conversas
- [ ] Notificações e integração com calendário

---

## 👥 Equipe

Desenvolvido durante o **Hackathon Vitru Educação**.

---

## 📄 Licença

Este projeto está sob a licença [MIT](https://opensource.org/licenses/MIT). Veja o arquivo `LICENSE` para mais detalhes.

---

<div align="center">
  Feito com ❤️ para o Hackathon Vitru Educação
</div>
