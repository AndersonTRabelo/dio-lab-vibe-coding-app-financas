# 💸 App de Finanças Pessoais em Design Universal criado com Vibe Coding

Um aplicativo de finanças pessoais focado em simplicidade e acessibilidade. Através de uma interface conversacional intuitiva, o usuário 
registra receitas, despesas e metas financeiras utilizando linguagem natural, eliminando a fricção de planilhas complexas e formulários 
manuais de preenchimento.

## 🎯 Principais Funcionalidades

* **Registro via Chat:** Inserção contínua de gastos, receitas e criação de metas conversando de forma natural (ex: "Gastei R$ 50 no iFood"
  ou "Quero guardar R$ 1000 para viajar").
* **Inteligência de Parcelamentos:** Reconhecimento automático de compras a prazo, dividindo as parcelas e projetando o comprometimento da
  renda nos meses futuros.
* **Dashboard e Relatórios:** Painel visual com gráficos de distribuição de despesas, visão do mês atual e indicador de comprometimento
  futuro.
* **Conciliação e Investimentos:** Extrato detalhado para conciliação bancária, configuração de saldos iniciais e acompanhamento de
  rendimentos de aplicações prévias.
* **Alertas Proativos:** Dicas e avisos gerados pelo agente sobre impactos no orçamento e evolução dos objetivos financeiros.
* **Design Universal:** Interface *mobile-first* limpa, com alto contraste, tolerância a erros e navegação adaptada para garantir uma
  experiência inclusiva e acessível a todos os usuários.

---

## 🛠️ Processo de Criação (Vibe Coding)

### 1. Prompt Inicial e PRD (Product Requirements Document)

Abaixo está o documento base e o prompt inicial utilizados para instruir a IA na criação da arquitetura e design do aplicativo.

```txt
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

# PRD: App Assistente Financeiro Conversacional 

## 1. Visao Geral do Produto (Contexto)
Um aplicativo Web/Mobile PWA de Organizacao de Financas Pessoais cuja principal interface e conversacional (estilo chat). O objetivo e
eliminar o atrito do controle financeiro manual, permitindo que o usuario registre receitas, gastos imediatos, compromissos futuros e
acompanhe investimentos, atraves de interacoes em linguagem natural de forma simples, fluida e amigavel.

## 2. Problema e Publico-Alvo
* Problema: Alta taxa de abandono no controle financeiro devido a friccao de inserir dados manuais, a falta de visibilidade do impacto das
compras a prazo no orcamento, a dificuldade de manter saldos reais sincronizados com o app e de acompanhar rendimentos.
* Publico-Alvo: Pessoas que desejam organizar as financas de forma pratica, com foco em iniciantes que tem dificuldade em visualizar o
comprometimento futuro de sua renda e precisam de ajuda para gerenciar metas e investimentos simples.

## 3. Principios de Design Universal (Regras de UI/UX para a IA)
A interface deve ser gerada respeitando rigorosamente os pilares de acessibilidade e usabilidade:
* Uso Equitativo e Simples: Interface limpa (minimalista), sem jargoes financeiros complexos. 
* Tipografia e Contraste: Uso de fontes legiveis (ex: Inter, Roboto) e paleta de cores com alto contraste (aderente ao padrao WCAG AA). Cores
devem reforcar a semantica sem depender exclusivamente delas (ex: usar setas e icones junto as cores).
* Tolerancia a Erros: Acoes destrutivas devem ser faceis de reverter. Confirmacoes visuais claras apos registrar qualquer movimentacao.
* Navegacao Acessivel: Botoes de acao grandes (minimo de 44x44 pixels) para facilitar o toque em telas mobile. 

## 4. Funcionalidades-Chave (Core Features)
1. Chat de Entrada Continua (Receitas, Despesas e Metas): O usuario pode registrar movimentacoes em linguagem natural. A criacao de metas
financeiras tambem devera ser feita integralmente a partir da interacao com o Chat (ex: "Quero criar uma meta para economizar 500 reais para
uma viagem").
2. Processamento Inteligente de Prazos (A vista vs. Parcelado): O sistema deve reconhecer se a despesa e imediata (debito, Pix) ou a prazo. A
IA deve quebrar automaticamente parcelamentos nos meses seguintes.
3. Projecao de Comprometimento Futuro: Calculo automatico que mostra ao usuario o quanto da renda ja esta "presa" nos proximos meses devido a
faturas e parcelamentos.
4. Conciliacao Bancaria: Funcionalidade para ajustar e alinhar o saldo do aplicativo com as contas bancarias reais, facilitando a correcao em
caso de descompasso (esquecimento de registro de despesas ou receitas).
5. Gestao e Rendimento de Investimentos: Permitir o acompanhamento de investimentos e a aplicacao de rendimentos sobre os saldos ja
investidos.
6. Dicas e Alertas do Agente: Alertas proativos sobre impactos no orcamento, andamento das metas e crescimento dos investimentos.

## 5. Escopo do MVP (Telas e Estrutura para Geracao no Lovable)
* Tela 1: Onboarding Simples. Boas-vindas educacionais e configuracao inicial. Deve incluir um passo para o usuario inserir informacoes de
saldo inicial em conta e investimentos realizados anteriormente a criacao da conta no aplicativo.
* Tela 2: Tela Principal (O Chat).
  - Area central de troca de mensagens.
  - Cards visuais gerados no chat para confirmar as acoes (registro de compras, criacao de nova meta, alerta de parcelamento).
* Tela 3: Dashboard de Saude Financeira (Relatorios e Extrato).
  - Relatorios e Graficos: Graficos consolidados mostrando a distribuicao de categorias de gastos, evolucao de metas e crescimento dos
investimentos ao longo do tempo.
  - Extrato Detalhado: Uma secao de extrato com o historico de transacoes, permitindo revisao, edicao rapida e conciliacao bancaria em caso
de divergencias de saldo.
  - Visao de Futuro: Indicador visual do nivel de comprometimento da renda dos proximos meses.
* Logica Base (Mockada para Validacao): Para o MVP no Lovable, o reconhecimento de palavras como "em X vezes", "meta", "rendeu" e "ajustar
saldo" pode ser usado para acionar as interfaces e testar a usabilidade das novas funcoes.

```

### 2. 💬 Interações com o Lovable

Evolução do projeto através de refinamentos contínuos:

> Aja como um Desenvolvedor Front-end Senior e Especialista em UX/UI com foco em Design Universal e Acessibilidade.
> Abaixo, fornecerei o PRD (Product Requirements Document) de um novo aplicativo de financas pessoais chamado "Assistente Financeiro
Conversacional".
> Por favor, leia as especificacoes e inicie o desenvolvimento do MVP seguindo estas diretrizes rigorosas:

> Excelente. Agora, adicione a Tela 3 (Dashboard) no menu inferior, incluindo os gráficos de categorias, a área de Extrato Detalhado para
conciliação bancária e o indicador de comprometimento futuro.

> Painel aprovado, porem gostaria que fosse possível uma autenticação de usuário no inicio para mais que seja um app que possa ser utilizado
por outro usuário que acesse o app e queira gerenciar suas despesas.

> Gostei do método de entrada, preciso que seja realizado um refinamento das categorias de despesas e que as metas e seus status seja
apresentados no dashboard.

> Permita definir um prazo para cada meta e mostre no Painel o valor mensal necessário para alcançá-la até essa data.
> Adicione um recurso no app que permita à pessoa usuária fazer perguntas em linguagem natural sobre seus gastos, categorias e metas e use um
modelo para gerar respostas e sugestões personalizadas com base nos dados financeiros dela usando o AI Gateway.

---

## 🧠 Reflexão

*** O que funcionou bem?
O refinamento do PRD previamente feito no Gemini ajudou muito, pois os créditos do Lovable acabaram em poucas interações.

*** O que não funcionou como o esperado?
Para um refinamento diferenciado tentei utilizar a forma Planejar do Lovable antes do Construir e consumiu os créditos rapidamente e precisei 
de mais 3 períodos para finalizar o projeto.

*** O que aprendeu sobre conversar com IAs?
Aprendi que é basicamente igual a conversar com uma pessoa bem inteligente, porém o amadurecimento de qualquer idéia para enriquecimento de 
informações e detalhes são essenciais para melhor interação e iteração.

## 💬 Conclusão

Vibe Coding é sobre clareza, curiosidade e criatividade, não sobre perfeição técnica. O verdadeiro objetivo aqui é aprender a pensar junto 
com a IA, transformando ideias em conceitos reais e enxergando a tecnologia como uma extensão do seu raciocínio criativo. Cada interação é um 
experimento, quanto mais clara for sua intenção, mais surpreendente será o resultado.
