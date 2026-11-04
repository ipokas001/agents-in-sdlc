---
slug: pt-br/real-world-development/cli
title: "CLI do GitHub Copilot"
description: "Crie, valide e entregue duas alterações no Tailspin Toys enquanto aprende sobre modos, personalizações, ferramentas MCP e automação de pull requests no Copilot CLI."
authors:
  - geektrainer
lastUpdated: 2026-09-18
---

O **[GitHub Copilot CLI](https://docs.github.com/copilot/concepts/agents/about-copilot-cli)** coloca o GitHub Copilot no seu terminal como um assistente de programação baseado em agentes. Ele explora bases de código, gera código, executa comandos e se conecta a ferramentas externas — tudo pela linha de comando, para que você mantenha o foco sem trocar para um editor gráfico.

O workshop acompanha um fluxo contínuo de trabalho no Tailspin Toys:

1. Prepare o projeto no GitHub Codespaces, instale o Copilot CLI e conheça seus recursos.
2. Faça uma pequena alteração para exibir avaliações por estrelas, revise-a no navegador e mescle manualmente seu primeiro pull request (PR).
3. Comece pelo issue de filtragem, defina a abordagem no modo Plan, implemente no modo Autopilot e revise no modo Interactive.
4. Atualize as instruções do repositório e aplique-as ao trabalho de filtragem.
5. Personalize a skill `quality-checks` existente e use-a para executar as verificações do projeto.
6. Adicione o servidor Model Context Protocol (MCP) do Playwright e use-o para explorar a filtragem no navegador.
7. Crie um agente personalizado de garantia de qualidade (QA) e use-o para revisar requisitos, cobertura e evidências de verificação.
8. Revise toda a alteração de filtragem e use o Agent Merge no PR correspondente.
9. Explore comandos slash úteis para contexto, modelos, compartilhamento e delegação opcional para o agente na nuvem.

Para manter o workshop focado, você criará dois PRs: um para as avaliações por estrelas e outro para a filtragem, com as atualizações de instruções, da skill, do perfil de QA e dos testes. O fluxo de filtragem e qualidade usa a mesma conversa e branch para que você aproveite o trabalho à medida que explora cada ferramenta.

## Lições

| Lição | Tópico | Descrição |
|----------|-------|-------------|
| [0. Pré-requisitos][ex0] | Configuração | Crie seu repositório e seu codespace |
| [1. Instale o Copilot CLI][ex1] | Instalação | Instale e autentique o Copilot CLI e conheça seus recursos |
| [2. Adicione avaliações por estrelas: uma melhoria rápida][ex2] | Primeira alteração | Exiba as avaliações existentes e a alternativa para valores nulos; depois, mescle seu primeiro PR |
| [3. Modos de agente: Plan e Autopilot][ex3] | Modos de agente | Planeje o recurso a partir do issue, implemente com Autopilot e revise no Interactive |
| [4. Oriente o Copilot com instruções personalizadas][ex4] | Contexto | Explore e atualize as instruções e aplique-as à filtragem |
| [5. Personalize e use uma skill de verificações de qualidade][ex5] | Verificações reutilizáveis | Explore a skill existente, altere o formato do relatório e execute-a |
| [6. Valide a funcionalidade com Playwright MCP][ex6] | Observação no navegador | Configure o MCP na CLI e inspecione o comportamento da filtragem |
| [7. Crie e use um agente de QA][ex7] | Requisitos e cobertura | Crie e selecione um perfil especialista e reúna as evidências finais de verificação |
| [8. Crie e mescle o PR do recurso][ex8] | Revisão e mesclagem | Revise a alteração completa, crie o PR e use o Agent Merge |
| [9. Comandos slash no GitHub Copilot CLI][ex9] | Recursos da CLI | Explore contexto, modelos, compartilhamento e delegação opcional para o agente na nuvem |
| [10. Encerramento e próximos passos][ex10] | Resumo | Revise o fluxo, as personalizações reutilizáveis e outros recursos |
| [Opcional: incorpore o Foundry][foundry] | Agentes hospedados | Prepare um modelo, implante um agente baseado no catálogo e conecte-o ao site |

## Pré-requisitos

Antes de participar deste workshop, verifique se você tem:

- [ ] Uma conta do GitHub com um plano ativo **Copilot Student, Pro, Pro+, Business ou Enterprise**
- [ ] Permissão para criar um repositório e um codespace
- [ ] Familiaridade básica com operações de terminal ou linha de comando

> [!TIP]
> Não tem um plano pago? Estudantes verificados podem obter o GitHub Copilot gratuitamente por meio do [GitHub Education][callout-student-plan-education]. O plano **Copilot Student** inclui os recursos de agente, MCP, revisão de código e Copilot CLI usados neste workshop.

> [!NOTE]
> Se você usa o Copilot Business ou o Copilot Enterprise, verifique se o administrador habilitou o Copilot CLI para uso.

## Começar

**[Comece pelos pré-requisitos →][ex0]**

[ex0]: 0-prerequisites/
[ex1]: 1-install-copilot-cli/
[ex2]: 2-add-star-rating/
[ex3]: 3-agent-modes/
[ex4]: 4-custom-instructions/
[ex5]: 5-agent-skills/
[ex6]: 6-mcp-playwright/
[ex7]: 7-qa-agent/
[ex8]: 8-create-pull-request/
[ex9]: 9-cli-power-tools/
[ex10]: 10-review/
[foundry]: 8-foundry-agent/
[callout-student-plan-education]: https://github.com/education/students
