# Modelo de Organização do Setor de Inovação da Sitelbra no ClickUp

Versão: 1.0  
Responsável: Janaina Rocha  

---

# 1. Objetivo

Este documento define o **modelo organizacional, o fluxo de trabalho e os critérios de padronização** utilizados pelo setor de Inovação da Sitelbra na gestão das atividades da vertical de Software, utilizando a **versão gratuita do ClickUp**.

O objetivo é:

- Garantir clareza no fluxo das tarefas  
- Padronizar entregas entre Desenvolvimento, QA e Gestão  
- Facilitar o acompanhamento das sprints  
- Organizar backlog, revisões técnicas e demandas espontâneas  
- Aumentar rastreabilidade e eficiência do time  

---

# 2. Estrutura Organizacional no ClickUp

## 2.1 Grupo Principal

- **Nome do Grupo:** *Inovação Sitelbra*  
- **Administração:** QA – *Janaina Moraes*

Este grupo centraliza **todos os projetos** vinculados ao setor de Inovação.

---

## 2.2 Espaços de Trabalho por Projeto

Cada projeto possui um **espaço próprio**, estruturado de forma padronizada.

**Exemplos de projetos:**

- Na Fila Não (NFN)  
- Hidden Brasil  
- Procon Digital  
- IPFibra  

Cada espaço de projeto contém listas e fluxos organizados conforme este documento.

---

# 3. Organização das Listas de Tarefas

Dentro de cada espaço de projeto, são criadas listas específicas. As principais são:

---

## 3.1 Lista de Sprint

Criada para **cada ciclo de desenvolvimento**, seguindo o padrão:

- `[Web] Sprint 01`  
- `[Web] Sprint 02`  
- `[App] Sprint 01`  
- `[App] Sprint 02`

Cada lista contém as tarefas aprovadas na **Reunião de Backlog da Sprint**.

---

## 3.2 Lista de Revisão Técnica

Lista destinada a:

- Ajustes emergenciais  
- Demandas paralelas  
- Correções de build  
- Solicitações inesperadas durante a sprint  

Exemplos:

- *Revisão Técnica – Ajustes no Build*  
- *Revisão Técnica – Nova demanda do hardware*  

---

## 3.3 Lista Backlog do Produto

Serve como um repositório central para:

- Ideias  
- Requisitos  
- Demandas futuras  
- Melhorias a serem priorizadas

Durante a **Reunião de Priorização**, os itens são selecionados para compor a próxima sprint.

---

# 4. Fluxo Operacional das Tarefas (Kanban)

O fluxo é composto pelas seguintes etapas:

---

## **1. To Do**
Tarefas recém-movidas para a sprint.  
Aguardam início do desenvolvedor.

---

## **2. In Progress**
Indica que o desenvolvedor iniciou a tarefa.

---

## **3. QA – Deploy Pending**
- Dev finalizou  
- Criou o MR (Merge Request)  
- Aguardando deploy no ambiente de homologação

---

## **4. QA – Deploy Finish**
- Deploy realizado  
- QA já pode iniciar os testes

---

## **5. Testing**
QA testa a tarefa conforme o plano de testes.  

Se:
- **Correto →** mover para *Done*  
- **Erro →** mover para *Bug*  

---

## **6. Bug**
Utilizada quando o QA identifica um desvio.

Deve conter:
- Resultado do teste  
- Prints, vídeos ou logs (quando aplicável)  
- Critério de aceitação violado  

### Fluxo após registrar o Bug

1. QA move a tarefa para **Bug**  
2. Desenvolvedor:  
   - move para **In Progress**  
   - ajusta o problema  
   - atualiza descrição/comentários  
   - envia novo MR (quando aplicável)  
   - move para **QA – Deploy Pending**  
3. Após o deploy → Dev ajusta para **QA – Deploy Finish**  
4. QA retoma na etapa **Testing**

---

## **7. Done**
- Tarefa validada pelo QA  
- Todos os critérios de aceitação atendidos  
- Fluxo encerrado  

---

# 4.1 Fluxograma do Processo

Quando você enviar a imagem, ela será exibida aqui:

```markdown
![Fluxograma do Processo no ClickUp](./imagens/fluxograma-processo-clickup.png)
