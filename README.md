# 💸 Assistente Financeiro Conversacional

> App de finanças pessoais em **Design Universal**, criado com **Vibe Coding** no Lovable.

![Lovable](https://img.shields.io/badge/Criado%20com-Lovable-ff4d8d)
![Bootcamp DIO](https://img.shields.io/badge/Bootcamp-DIO-0b3d91)
![Status](https://img.shields.io/badge/Status-MVP%20funcional-2e9e6b)
![Acessibilidade](https://img.shields.io/badge/Acessibilidade-WCAG%20AA-1f6feb)

Um aplicativo focado em **simplicidade e acessibilidade**. Por meio de uma interface conversacional, a pessoa usuária registra receitas, despesas e metas financeiras em linguagem natural, sem planilhas complexas nem formulários manuais.

👉 **[Acesse o protótipo funcional](https://exact-capture-frame-39.lovable.app)**

---

## 📑 Sumário

- [Sobre o projeto](#-sobre-o-projeto)
- [Principais funcionalidades](#-principais-funcionalidades)
- [Como testar](#-como-testar)
- [Processo de criação (Vibe Coding)](#️-processo-de-criação-vibe-coding)
- [Resultado final](#-resultado-final)
- [Reflexão](#-reflexão)
- [Conclusão](#-conclusão)

---

## 🎓 Sobre o projeto

Projeto desenvolvido como desafio do **bootcamp de Empreendedorismo com IA da DIO**, com o objetivo de colocar a mão na massa e transformar uma ideia em um **MVP funcional** usando IA, no-code e Vibe Coding.

**Problema que o app resolve:** muita gente abandona o controle financeiro por causa do atrito de inserir dados manualmente e da falta de visibilidade sobre o impacto das compras parceladas no orçamento.

**Público-alvo:** pessoas que querem organizar as finanças de forma prática, principalmente iniciantes com dificuldade de enxergar o comprometimento futuro da renda e de gerenciar metas e investimentos simples.

**Ferramentas utilizadas:**

| Etapa | Ferramenta |
|---|---|
| Refinamento do PRD | Gemini |
| Geração e evolução do app | Lovable |
| Respostas e sugestões personalizadas | AI Gateway |

---

## 🎯 Principais funcionalidades

| Funcionalidade | Descrição |
|---|---|
| 💬 **Registro via chat** | Inserção contínua de gastos, receitas e metas conversando de forma natural. |
| 🧾 **Inteligência de parcelamentos** | Reconhece compras a prazo, divide as parcelas e projeta o comprometimento da renda nos meses futuros. |
| 📊 **Dashboard e relatórios** | Painel visual com distribuição de despesas, visão do mês atual e indicador de comprometimento futuro. |
| 🏦 **Conciliação e investimentos** | Extrato detalhado para conciliação bancária, saldos iniciais e acompanhamento de rendimentos de aplicações prévias. |
| 🔔 **Alertas proativos** | Dicas e avisos do agente sobre impactos no orçamento e evolução dos objetivos. |
| 🎯 **Metas com prazo** | Define um prazo para cada meta e mostra no painel o valor mensal necessário para alcançá-la. |
| 🤖 **Perguntas em linguagem natural** | A pessoa pergunta sobre gastos, categorias e metas e recebe respostas e sugestões personalizadas. |
| ♿ **Design Universal** | Interface mobile-first, com alto contraste, tolerância a erros e navegação adaptada para ser inclusiva. |

### ♿ Princípios de acessibilidade aplicados

- Paleta de cores com **alto contraste** (WCAG AA).
- Cores nunca são o único indicador: sempre acompanhadas de **ícones** (setas e sinais de + e −).
- Fontes legíveis (Inter ou Roboto) e tamanhos adequados.
- Botões e áreas de clique com no mínimo **44x44 px**.
- Ações destrutivas fáceis de reverter e confirmações visuais claras.

---

## 🧪 Como testar

Acesse o [protótipo](https://exact-capture-frame-39.lovable.app) e experimente digitar no chat:

```text
Gastei R$ 50 no iFood hoje
Comprei uma TV de 2000 em 10 vezes
Quero guardar R$ 1000 para viajar
```

Cada frase gera um card diferente: confirmação de gasto, alerta de comprometimento com a divisão das parcelas e meta financeira.

---

## 🛠️ Processo de criação (Vibe Coding)

### 1. Prompt inicial e PRD

O ponto de partida foi um prompt detalhado, acompanhado de um **PRD (Product Requirements Document)**, para instruir a IA na criação da arquitetura e do design do app.

<details>
<summary><b>📝 Ver o prompt inicial</b></summary>

```text
Aja como um Desenvolvedor Front-end Senior e Especialista em UX/UI com foco em Design Universal e Acessibilidade.

Abaixo, fornecerei o PRD (Product Requirements Document) de um novo aplicativo de financas pessoais chamado "Assistente Financeiro
Conversacional".

Por favor, leia as especificacoes e inicie o desenvolvimento do MVP seguindo estas diretrizes rigorosas:

1. DESIGN SYSTEM E ACESSIBILIDADE (DESIGN UNIVERSAL):
- Crie uma interface "mobile-first" (pode ser renderizada na web, mas com proporcoes de celular).
- Use uma paleta de cores limpa, com alto contraste (aderente ao WCAG AA). Nao dependa apenas de verde/vermelho para indicar valores; use
sempre icones (setas para cima/baixo, sinais de + e -).
- Fontes legiveis (ex: Inter ou Roboto) com tamanhos adequados.
- Botoes e areas de clique devem ter no minimo 44x44 pixels.
- Utilize componentes modernos, minimalistas e com cantos arredondados (estilo Shadcn UI ou similar).

2. O QUE CONSTRUIR NESTA PRIMEIRA ETAPA:
Nao crie todas as telas de uma vez. Para esta interacao inicial, construa a estrutura principal do app (um menu de navegacao inferior
simples) e as duas primeiras telas descritas no PRD:
- TELA DE ONBOARDING: Uma tela simples para coletar o nome do usuario e um formulario claro para inserir o "Saldo Inicial em Conta" e
"Investimentos Previos".
- TELA PRINCIPAL (CHAT): A interface core do app. Uma area de rolagem de mensagens e um input de texto fixo na base (estilo WhatsApp).

3. COMPORTAMENTO E MOCK DATA (VIBE CODING):
- Implemente uma logica simulada (mock) no Chat.
- Se eu digitar "Gastei 50 reais no Ifood hoje", faça o sistema responder com um "Card UI" confirmando a transacao imediata.
- Se eu digitar "Comprei uma TV de 2000 em 10 vezes", faça o sistema responder com um "Card UI de Alerta de Comprometimento", mostrando a
divisao das parcelas.
- Se eu digitar "Quero guardar 1000 reais para viajar", crie um Card de Meta Financeira.

Aqui esta o PRD com todas as regras de negocio que voce deve seguir:
```

</details>

<details>
<summary><b>📄 Ver o PRD completo</b></summary>

#### PRD: App Assistente Financeiro Conversacional

**1. Visão geral do produto (contexto)**

Um aplicativo Web/Mobile PWA de organização de finanças pessoais cuja principal interface é conversacional (estilo chat). O objetivo é eliminar o atrito do controle financeiro manual, permitindo que o usuário registre receitas, gastos imediatos, compromissos futuros e acompanhe investimentos, através de interações em linguagem natural de forma simples, fluida e amigável.

**2. Problema e público-alvo**

- **Problema:** alta taxa de abandono no controle financeiro devido à fricção de inserir dados manuais, à falta de visibilidade do impacto das compras a prazo no orçamento, à dificuldade de manter saldos reais sincronizados com o app e de acompanhar rendimentos.
- **Público-alvo:** pessoas que desejam organizar as finanças de forma prática, com foco em iniciantes que têm dificuldade em visualizar o comprometimento futuro de sua renda e precisam de ajuda para gerenciar metas e investimentos simples.

**3. Princípios de Design Universal (regras de UI/UX para a IA)**

A interface deve ser gerada respeitando rigorosamente os pilares de acessibilidade e usabilidade:

- **Uso equitativo e simples:** interface limpa (minimalista), sem jargões financeiros complexos.
- **Tipografia e contraste:** fontes legíveis (ex.: Inter, Roboto) e paleta de cores com alto contraste (padrão WCAG AA). Cores devem reforçar a semântica sem depender exclusivamente delas (ex.: usar setas e ícones junto às cores).
- **Tolerância a erros:** ações destrutivas devem ser fáceis de reverter. Confirmações visuais claras após registrar qualquer movimentação.
- **Navegação acessível:** botões de ação grandes (mínimo de 44x44 pixels) para facilitar o toque em telas mobile.

**4. Funcionalidades-chave (core features)**

1. **Chat de entrada contínua (receitas, despesas e metas):** o usuário pode registrar movimentações em linguagem natural. A criação de metas financeiras também deverá ser feita integralmente a partir da interação com o chat (ex.: "Quero criar uma meta para economizar 500 reais para uma viagem").
2. **Processamento inteligente de prazos (à vista vs. parcelado):** o sistema deve reconhecer se a despesa é imediata (débito, Pix) ou a prazo. A IA deve quebrar automaticamente parcelamentos nos meses seguintes.
3. **Projeção de comprometimento futuro:** cálculo automático que mostra ao usuário o quanto da renda já está "presa" nos próximos meses devido a faturas e parcelamentos.
4. **Conciliação bancária:** funcionalidade para ajustar e alinhar o saldo do aplicativo com as contas bancárias reais, facilitando a correção em caso de descompasso (esquecimento de registro de despesas ou receitas).
5. **Gestão e rendimento de investimentos:** permitir o acompanhamento de investimentos e a aplicação de rendimentos sobre os saldos já investidos.
6. **Dicas e alertas do agente:** alertas proativos sobre impactos no orçamento, andamento das metas e crescimento dos investimentos.

**5. Escopo do MVP (telas e estrutura para geração no Lovable)**

- **Tela 1: Onboarding simples.** Boas-vindas educacionais e configuração inicial, incluindo um passo para o usuário inserir saldo inicial em conta e investimentos realizados antes da criação da conta no aplicativo.
- **Tela 2: Tela principal (o chat).**
  - Área central de troca de mensagens.
  - Cards visuais gerados no chat para confirmar as ações (registro de compras, criação de nova meta, alerta de parcelamento).
- **Tela 3: Dashboard de saúde financeira (relatórios e extrato).**
  - **Relatórios e gráficos:** distribuição de categorias de gastos, evolução de metas e crescimento dos investimentos ao longo do tempo.
  - **Extrato detalhado:** histórico de transações, com revisão, edição rápida e conciliação bancária em caso de divergências de saldo.
  - **Visão de futuro:** indicador visual do nível de comprometimento da renda nos próximos meses.
- **Lógica base (mockada para validação):** para o MVP no Lovable, o reconhecimento de palavras como "em X vezes", "meta", "rendeu" e "ajustar saldo" pode ser usado para acionar as interfaces e testar a usabilidade das novas funções.

</details>

### 2. 💬 Interações com o Lovable

O projeto evoluiu por meio de refinamentos contínuos. Estas foram as etapas, em ordem:

| # | Etapa | Prompt utilizado |
|---|---|---|
| 1 | **Estrutura base** | Prompt inicial acima (menu inferior, onboarding e chat). |
| 2 | **Dashboard** | *"Excelente. Agora, adicione a Tela 3 (Dashboard) no menu inferior, incluindo os gráficos de categorias, a área de Extrato Detalhado para conciliação bancária e o indicador de comprometimento futuro."* |
| 3 | **Autenticação** | *"Painel aprovado, porem gostaria que fosse possível uma autenticação de usuário no inicio para mais que seja um app que possa ser utilizado por outro usuário que acesse o app e queira gerenciar suas despesas."* |
| 4 | **Categorias e metas** | *"Gostei do método de entrada, preciso que seja realizado um refinamento das categorias de despesas e que as metas e seus status seja apresentados no dashboard."* |
| 5 | **Prazo de metas e IA conversacional** | *"Permita definir um prazo para cada meta e mostre no Painel o valor mensal necessário para alcançá-la até essa data. Adicione um recurso no app que permita à pessoa usuária fazer perguntas em linguagem natural sobre seus gastos, categorias e metas e use um modelo para gerar respostas e sugestões personalizadas com base nos dados financeiros dela usando o AI Gateway."* |

---

## 🚀 Resultado final

Protótipo funcional publicado no Lovable:

🔗 **https://exact-capture-frame-39.lovable.app**

---

## 🧠 Reflexão

**✅ O que funcionou bem?**
O refinamento do PRD feito previamente no Gemini ajudou muito, pois os créditos do Lovable acabaram em poucas interações.

**⚠️ O que não funcionou como o esperado?**
Para um refinamento diferenciado, tentei usar o modo *Planejar* do Lovable antes do *Construir*, mas isso consumiu os créditos rapidamente e precisei de mais 3 períodos para finalizar o projeto.

**💡 O que aprendi sobre conversar com IAs?**
Que é basicamente igual a conversar com uma pessoa muito inteligente, porém o amadurecimento de qualquer ideia, com enriquecimento de informações e detalhes, é essencial para uma melhor interação e iteração.

---

## 💬 Conclusão

> **Vibe Coding é sobre clareza, curiosidade e criatividade, não sobre perfeição técnica.**

O verdadeiro objetivo aqui é aprender a pensar junto com a IA, transformando ideias em conceitos reais e enxergando a tecnologia como uma extensão do seu raciocínio criativo. Cada interação é um experimento: quanto mais clara for a sua intenção, mais surpreendente será o resultado.
