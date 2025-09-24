# Copilot Agents Collection 🤖

> Uma coleção personalizada de agentes especializados para GitHub Copilot, otimizados para diferentes aspectos do desenvolvimento de software.

[![GitHub](https://img.shields.io/badge/GitHub-Copilot_Agents-blue?logo=github)](https://github.com/Crown32/copilot_agents)
[![VS Code](https://img.shields.io/badge/VS_Code-Extension-007ACC?logo=visualstudiocode)](https://code.visualstudio.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 📋 Sobre este Repositório

Este repositório contém uma **coleção de agentes personalizados do GitHub Copilot** (arquivos `.chatmode.md`) que podem ser adicionados ao contexto do usuário no VS Code. Cada agente é especializado em uma área específica do desenvolvimento, oferecendo assistência focada e expertise direcionada.

### 🎯 Agentes Disponíveis

| 🔧 Agente | 📝 Descrição | ⚡ Especialização | 📋 To-Dos |
|-----------|--------------|------------------|-----------|
| **Coding Agent** | Desenvolvimento e implementação | Features, debugging, arquitetura | ✅ Step-by-step |
| **Documentation Agent** | Criação de documentação | READMEs, APIs, tutoriais | ✅ Planejamento |
| **Review Agent** | Análise e revisão de código | Code review, qualidade, segurança | ✅ Revisão sistemática |
| **Refinement Agent** | Refinamento de tarefas | Histórias de usuário, análise | ✅ Gera to-dos |
| **Commit Agent** | Gestão de commits e versionamento | Conventional commits, changelogs | ✅ Commits organizados |

### 📋 **NOVO**: Sistema de To-Dos Integrado

Todos os agentes agora trabalham com **metodologia step-by-step** usando to-dos para máxima transparência:

✅ **Planejamento Claro**: Cada tarefa é quebrada em steps organizados  
✅ **Progresso Visível**: Acompanhe cada etapa em tempo real  
✅ **Integração entre Agentes**: @refinement-agent → @coding-agent com to-dos estruturados  
✅ **Transparência Total**: Veja exatamente o que está sendo feito e o que vem a seguir

---

## 🚀 Como Usar

### 1️⃣ Localizar a Pasta de Contexto do VS Code

A pasta de contexto do usuário do VS Code está localizada em:

**🪟 Windows:**

```powershell
%APPDATA%\Code\User\prompts\
```

**🍎 macOS:**

```bash
~/Library/Application Support/Code/User/globalStorage/github.copilot-chat/
```

**🐧 Linux:**

```bash
~/.config/Code/User/globalStorage/github.copilot-chat/
```

### 2️⃣ Instalar os Agentes

1. **Clone** este repositório ou **baixe** os arquivos `.chatmode.md`
2. **Copie** os arquivos desejados para a pasta de contexto do VS Code
3. **Reinicie** o VS Code para carregar os novos agentes

### 3️⃣ Ativar um Agente

No VS Code, abra o **GitHub Copilot Chat** e digite:

```text
@coding-agent Preciso implementar uma nova feature de autenticação
```

```text
@review-agent Revise este código para identificar possíveis problemas
```

```text
@documentation-agent Crie documentação para esta API
```

### 🎯 **NOVO**: Fluxo Integrado com To-Dos

```text
@refinement-agent Refine esta ideia: sistema de gestão de produtos
↓ (Gera história + to-dos estruturados)
@coding-agent Implemente a história que o @refinement-agent criou
↓ (Trabalha step-by-step com progresso visível)
@review-agent Revise o código implementado pelo @coding-agent
```

---

## 📁 Estrutura dos Agentes

Cada agente segue o padrão de arquivo `.chatmode.md`:

```yaml
---
description: 'Descrição breve do agente'
tools: ['edit', 'search', 'runCommands', ...]
---

# Nome do Agente

Conteúdo do prompt do agente...
```

### 🏗️ Seções Principais

- **📋 Frontmatter YAML**: Metadados do agente (descrição, ferramentas)
- **🎯 Identidade**: O que o agente é e seu foco principal  
- **⚡ Capacidades**: Lista específica do que pode fazer
- **🔧 Especialização**: Tecnologias e áreas de expertise
- **💡 Exemplos**: Casos de uso práticos
- **📖 Diretrizes**: Instruções específicas de comportamento

---

## ✨ Criando Novos Agentes

### 📝 Template Base

```markdown
---
description: 'Sua descrição aqui'
tools: ['edit', 'search', 'runCommands']
---

# Seu Agente

Sou um especialista em [área de expertise]...

## Como posso ajudar:

### 🎯 Área Principal
- Funcionalidade 1
- Funcionalidade 2

### 🔧 Área Secundária
- Funcionalidade 3
- Funcionalidade 4
```

### 💡 Dicas para Criação

| Dica | Descrição |
|------|-----------|
| **🎯 Seja Específico** | Defina claramente o escopo e especialização |
| **😊 Use Emojis** | Facilita a identificação visual |
| **🛠️ Liste Ferramentas** | Inclua apenas as tools necessárias (adicione 'todos' se precisar de planejamento) |
| **📚 Exemplos Práticos** | Mostre casos de uso reais |
| **📖 Instruções Claras** | Defina comportamentos esperados |
| **📋 Metodologia To-Dos** | Para tarefas complexas, inclua sistema de to-dos step-by-step |

---

## 🔄 Roadmap e Atualizações

Este repositório será atualizado incrementalmente com:

- ✅ Novos agentes especializados
- ✅ Melhorias nos agentes existentes  
- ✅ Templates para casos de uso específicos
- ✅ Documentação expandida
- 🔄 Integração com mais ferramentas
- 🔄 Exemplos de uso avançados

---

## 📚 Recursos Úteis

| Recurso | Link |
|---------|------|
| **GitHub Copilot Docs** | [docs.github.com/copilot](https://docs.github.com/en/copilot) |
| **VS Code Extension** | [marketplace.visualstudio.com](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot-chat) |
| **Best Practices** | [copilot best practices](https://docs.github.com/en/copilot/using-github-copilot/best-practices-for-using-github-copilot-chat) |

---

## 🤝 Contribuindo

Sua contribuição é bem-vinda! Sinta-se à vontade para:

- 🔧 Sugerir melhorias nos agentes existentes
- 🆕 Propor novos agentes especializados
- 🐛 Reportar problemas ou bugs
- 💡 Compartilhar casos de uso interessantes

### Como Contribuir

1. **Fork** este repositório
2. **Crie** uma branch para sua feature (`git checkout -b feature/novo-agente`)
3. **Commit** suas mudanças (`git commit -am 'Add: novo agente para testes'`)
4. **Push** para a branch (`git push origin feature/novo-agente`)
5. **Abra** um Pull Request

---

## 📄 Licença

Este projeto está sob a licença **MIT**. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## 🙏 Agradecimentos

- **GitHub Copilot Team** - Por tornar possível a criação de agentes personalizados
- **VS Code Team** - Pela plataforma extensível
- **Comunidade** - Por feedback e contribuições

---

---

**💡 Dica**: Para melhor experiência, mantenha os agentes atualizados e personalize-os conforme suas necessidades específicas de desenvolvimento!

**⭐ Se este projeto foi útil para você, considere dar uma estrela!**
