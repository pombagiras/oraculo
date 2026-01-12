# 🔮 Oráculo das 12 Luas

Uma experiência digital mística conectando tecnologia e espiritualidade.

---

## ✨ Sobre o Projeto

O **Oráculo das 12 Luas** é uma aplicação web interativa que combina conhecimento espiritual sobre as Pombagiras da Umbanda com uma experiência de quiz educativa. Através de 12 perguntas místicas, os visitantes descobrem qual das 12 Guardiãs ressoa com sua energia espiritual.

### 🌙 Características Principais

- **Interface Mística**: Design dark com efeitos visuais de chuva de emojis místicos
- **Quiz Interativo**: 12 perguntas sobre as Pombagiras e suas características
- **Sistema de Pontuação**: Feedback visual instantâneo (acertos em verde, erros em vermelho)
- **Barra de Progresso**: Acompanhamento visual da jornada pelo oráculo
- **Resultado Personalizado**: Revelação da Guardiã Regente baseada no desempenho
- **Navegação Integrada**: Links para diversos portais e redes sociais do ecossistema

---

## 🎭 As 12 Guardiãs

| Pombagira | Título | Domínio |
|-----------|--------|---------|
| 👑 Maria Padilha | A Rainha | Comando |
| 🌺 Maria Mulambo | A Curadora | Cura |
| ⚔️ Maria Quitéria | A Guerreira | Proteção |
| 💀 Rosa Caveira | Guardiã dos Ciclos | Justiça |
| 🌙 Dama da Noite | Guardiã dos Segredos | Mistério |
| 💃 Sete Saias | A Dançarina | Alegria |
| 🔮 Pombagira Cigana | A Viajante | Liberdade |
| 🗡️ Maria Navalha | A Malandrina | Rua |
| 🌊 Pombagira da Praia | Guardiã das Águas | Emoção |
| 🧩 Maria Farrapo | A Transformadora | Sanidade |
| 🌸 Pombagira Menina | A Inocente | Renovação |
| 🌳 Pombagira da Figueira | Guardiã das Raízes | Ancestralidade |

---

## 🎨 Elementos Visuais

### Paleta de Cores
```css
--cor-roxo: #4b0082       /* Roxo místico principal */
--cor-lilas: #e0b0ff      /* Lilás para acentos */
--cor-vermelho: #ff0000   /* Vermelho energético */
--cor-preto: #050505      /* Fundo escuro */
--texto-destaque: #ffd700 /* Dourado para títulos */
--cor-acerto: #00ff00     /* Verde para respostas corretas */
--cor-erro: #ff0000       /* Vermelho para erros */
```

### Animações
- **Chuva Mística**: Emojis caindo continuamente (🍷🔱🌹💃🔥🕯️🚬🌙💀🗡️)
- **Efeito Glassmorphism**: Container principal com blur e transparência
- **Botões Pulsantes**: Animações de hover e estados ativos
- **Transições Suaves**: Feedback visual nas respostas do quiz

---

## 🚀 Tecnologias Utilizadas

- **HTML5**: Estrutura semântica
- **CSS3**: Animações, gradientes e efeitos modernos
- **JavaScript Vanilla**: Lógica do quiz e interatividade
- **Design Responsivo**: Adaptável a diferentes dispositivos

---

## 📱 Estrutura de Navegação

O portal integra diversos sites do ecossistema:

- 🌐 **Redes Sociais**: Hub principal de mídias sociais
- 🏠 **Hub Pombagiras**: Central de conteúdo
- 🔮 **Oráculo**: Página atual
- 📖 **Grimório**: Conhecimento místico
- 🎵 **Pontos Cantados**: Músicas rituais
- 🌑 **Dark Melancholy**: Conteúdo sombrio
- 📝 **Blog**: Artigos e reflexões
- 🔗 **Bio Links**: Linktree e Canvas
- 🔥 **Business Card**: Contato de emergência

---

## 🎮 Como Funciona

1. **Início**: Usuário clica em "Abrir o Portal"
2. **Quiz**: Responde 12 perguntas sobre as Pombagiras
3. **Feedback**: Cada resposta mostra se está correta (verde) ou errada (vermelho)
4. **Resultado**: Sistema calcula a Guardiã Regente baseada nos acertos
5. **Revelação**: Exibe nome, título, domínio e mensagem da Guardiã

### Algoritmo de Seleção
```javascript
// A Guardiã é selecionada pelo módulo dos acertos
const guardia = pombagirasDB[acertos % pombagirasDB.length];
```

---

## 💻 Instalação e Uso

### Opção 1: Abrir Diretamente
```bash
# Clone ou baixe o arquivo HTML
# Abra index.html no navegador
```

### Opção 2: Servidor Local
```bash
# Python 3
python -m http.server 8000

# Node.js
npx http-server

# Acesse: http://localhost:8000
```

### Opção 3: Deploy
- **GitHub Pages**: Faça upload e ative nas configurações
- **Netlify**: Arraste e solte o arquivo
- **Vercel**: Deploy via CLI ou interface

---

## 🎯 Funcionalidades Detalhadas

### Sistema de Quiz
- ✅ 12 perguntas pré-definidas
- ✅ 4 opções de resposta por pergunta
- ✅ Validação automática
- ✅ Desabilitação dos botões após resposta
- ✅ Highlight da resposta correta
- ✅ Delay de 1.5s antes da próxima pergunta

### Interface
- ✅ Design glassmorphism
- ✅ Animação de chuva contínua
- ✅ Barra de progresso dinâmica
- ✅ Navegação por botões estilizados
- ✅ Responsividade mobile-first

### Resultado Final
- ✅ Card personalizado da Guardiã
- ✅ Placar de acertos
- ✅ Mensagem inspiradora
- ✅ Botão para reiniciar

---

## 🎨 Customização

### Adicionar Novas Perguntas
```javascript
const perguntasBase = [
    {
        t: "Texto da pergunta?",
        r: "Resposta Correta",
        o: ["Opção 1", "Opção 2", "Opção 3", "Resposta Correta"]
    }
];
```

### Adicionar Nova Guardiã
```javascript
const pombagirasDB = [
    {
        nome: "Nome da Pombagira",
        titulo: "Título Místico",
        dominio: "Domínio",
        msg: "Mensagem inspiradora completa"
    }
];
```

### Modificar Cores
Edite as variáveis CSS em `:root` no topo do arquivo.

---

## 📊 Estrutura de Arquivos
```
oraculo-12-luas/
│
├── index.html          # Arquivo principal (único necessário)
├── README.md           # Este arquivo
└── LICENSE             # Licença do projeto (opcional)
```

---

## 🌟 Diferenciais

- ✨ **Zero Dependências**: Não requer bibliotecas externas
- ✨ **Single File**: Toda aplicação em um único HTML
- ✨ **Performance**: Carregamento instantâneo
- ✨ **Acessibilidade**: Estrutura semântica e contrastes adequados
- ✨ **Mobile First**: Totalmente responsivo
- ✨ **Experiência Imersiva**: Animações e efeitos envolventes

---

## 🔒 Privacidade

Este projeto:
- ❌ Não coleta dados pessoais
- ❌ Não usa cookies
- ❌ Não rastreia usuários
- ✅ 100% client-side
- ✅ Funciona offline (após carregamento inicial)

---

## 🤝 Contribuindo

Contribuições são bem-vindas! Para contribuir:

1. Fork o projeto
2. Crie uma branch (`git checkout -b feature/NovaGuardia`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova Guardiã'`)
4. Push para a branch (`git push origin feature/NovaGuardia`)
5. Abra um Pull Request

---

## 📜 Licença

Este projeto é livre para uso pessoal e educacional. Para uso comercial, entre em contato.

---

## 🔗 Links Relacionados

- 🌐 [Redes Sociais](https://alexialuzdeferro.github.io/redes_sociais/)
- 🏠 [Hub Pombagiras](https://alexialuzdeferro.github.io/Hub-Pombagiras/)
- 📖 [Grimório](https://alexialuzdeferro.github.io/grimorio-das-pombagiras/)
- 🎵 [Pontos Cantados](https://alexialuzdeferro.github.io/PONTOS-CANTADOS/)
- 🌑 [Dark Melancholy](https://alexialuzdeferro.github.io/dark-melancholy/)
- 📝 [Blog](https://alexialuzdeferro.github.io/Pombagiras/)
- 🔗 [Linktree](https://linktr.ee/alexiarosadefogo)
- 🎨 [Canvas](https://pombagiras.my.canva.site/)
- 🌟 [Portal](https://bio.site/AlmasdePombagira)
- 🔥 [Business Card](https://alexialuzdeferro.github.io/Business-Card/)

---

## 💬 Contato

Para dúvidas, sugestões ou colaborações:
- 🔗 [Portal Principal](https://bio.site/AlmasdePombagira)
- 🔥 [Business Card](https://alexialuzdeferro.github.io/Business-Card/)

---

## 🙏 Agradecimentos

Gratidão às forças espirituais que inspiram este trabalho e a todos que buscam conhecimento através da tecnologia e da espiritualidade.

---

<div align="center">

**🔮 Que as Guardiãs iluminem seu caminho 🔮**

⭐ Se este projeto foi útil, considere dar uma estrela!

</div>
