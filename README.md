# 💸 App de Organização de Finanças Pessoais com Vibe Coding
Desafio de Projeto da DIO utilizando vibe coding e lovable.

- **prompt final** (PRD):  
# Product Requirement Document (PRD) - App de Finanças Pessoais com IA

## 1. Visão Geral do Produto

### 1.1. Contexto
Criar um aplicativo de Organização de Finanças Pessoais que funcione por meio de conversas com o usuário em linguagem natural. A ideia é facilitar o controle financeiro de forma simples e natural, sem formulários manuais ou planilhas complexas.

### 1.2. Problema
Muitas pessoas desistem de controlar seus gastos porque os apps atuais exigem muita entrada manual e pouca personalização. Estatisticamente, 80% das pessoas desistem de apps financeiros em até 30 dias. Este app resolve isso com uma experiência de conversa e recomendações automáticas de economia.

### 1.3. Tom de Voz
Amigável, motivador, simples e acessível. O agente financeiro deve se comunicar como um conselheiro paciente, não como um contador.

### 1.4. Público-Alvo
Pessoas que querem começar a organizar suas finanças de forma prática e sem complicação, principalmente iniciantes.

Persona principal: Ana, 28 anos, autônoma, quer economizar para viajar, mas se sente sobrecarregada com planilhas. Nível de conhecimento financeiro: zero. Precisa de onboarding guiado.

---

## 2. Funcionalidades-Chave (MVP)

### 2.1. Registro de Gastos via Chat
Campo de texto com exemplos visíveis: "Gastei R$50 no supermercado". A IA extrai valor, categoria e data automaticamente.

### 2.2. Classificação Automática
Categorias fixas iniciais: Alimentação, Transporte, Lazer, Moradia, Saúde, Educação, Outros. O usuário pode criar novas categorias via chat.

### 2.3. Metas Financeiras
Definir metas simples como: "Quero juntar R$1000 em 3 meses". O app calcula automaticamente quanto guardar por dia/semana e mostra progresso em barra.

### 2.4. Agente Financeiro (Dicas)
Disparos automáticos: quando gasto em lazer ultrapassa 30% da renda, o app sugere corte. Dica semanal enviada por push/notificação. As dicas devem ser personalizadas com base no histórico do usuário.

### 2.5. Relatórios Simples
Gráficos básicos: pizza por categoria, linha de evolução de saldo. Gerados sob demanda via chat com comandos como "Mostre meus gastos esse mês".

---

## 3. Design Universal e Acessibilidade

### 3.1. O que é Design Universal
Abordagem de criar produtos que podem ser usados por todas as pessoas, independentemente de idade, habilidade ou condição. Não é sobre adaptar depois, mas projetar para a diversidade humana desde o início.

Princípios aplicados:
- Uso equitativo: útil para pessoas com diferentes habilidades
- Uso flexível: atende a diferentes ritmos e preferências
- Simples e intuitivo: fácil de entender
- Informação perceptível: comunica-se por múltiplos canais (visual, auditivo)
- Tolerância ao erro: minimiza riscos
- Baixo esforço físico: requer o mínimo de força
- Espaço e tamanho adequados: para uso independente

### 3.2. Por que é Crítico
- Inclusão financeira: pessoas com deficiência também precisam gerenciar dinheiro
- Longevidade: app se adapta a mudanças (envelhecimento, lesões temporárias)
- Diferencial competitivo: poucos apps financeiros são acessíveis
- Legal e ético: conformidade com LGPD, WCAG e Lei Brasileira de Inclusão
- Melhora para todos: legendas ajudam em ambientes barulhentos, contraste ajuda em luz solar

### 3.3. Grupos Beneficiados
- Pessoas com baixa visão ou cegueira: texto legível, contraste, leitores de tela
- Pessoas com daltonismo: não usar apenas cores para transmitir info
- Pessoas com dificuldade motora: botões grandes, atalhos por voz
- Pessoas com dislexia ou baixa alfabetização: texto simples, ícones claros
- Pessoas com deficiência auditiva: feedback visual e vibratório
- Pessoas com autismo ou TDAH: layout limpo, modo foco
- Idosos: modo fácil com interface ampliada

### 3.4. Requisitos Técnicos de Acessibilidade
- Contraste de cores: razão mínima de 4.5:1 para texto normal
- Tamanho de fonte: mínimo 16px com opção de aumentar até 200%
- Navegação por teclado: todos os elementos interativos acessíveis via Tab, Enter e Espaço
- Suporte a leitores de tela: ARIA labels em todos os componentes
- Texto alternativo: descrições em imagens e gráficos
- Não depender de cor: usar ícones, padrões ou textos além das cores
- Legendas e transcrições: para vídeos tutoriais
- Tempo suficiente: sem timeout para ações
- Redução de movimento: respeitar prefers-reduced-motion
- Modo escuro/claro: ambos com contraste adequado

### 3.5. Funcionalidades Específicas Acessíveis
- Chat: comando de voz + leitura automática das respostas
- Relatórios: descrição textual dos gráficos + tabela de dados acessível
- Metas: barra com percentual numérico e descrição textual
- Dicas: notificações visuais e sonoras (com opção de desligar som)
- Registro: sugestões automáticas + confirmação por voz
- Onboarding: tutorial em áudio e versão legendada

### 3.6. Histórias de Usuário Acessíveis
- Como usuário com baixa visão, quero aumentar a fonte em até 200% sem quebrar o layout.
- Como usuário surdo, quero receber notificações visuais quando o Agente tiver uma dica.
- Como usuário com dificuldade motora, quero registrar gastos por comando de voz.
- Como usuário daltônico, quero que os gráficos usem padrões além de cores.

### 3.7. Testes de Acessibilidade
- Lighthouse (Chrome): relatório automatizado
- WAVE: contrastes, estrutura, ARIA
- NVDA (Windows) / VoiceOver (Mac/iOS): navegação com leitor de tela
- Simulador de daltonismo: extensões como Colorblindly
- Teste com usuários reais com deficiências

---

## 4. Estrutura de Telas (MVP)

### 4.1. Tela 1: Chat Principal
Componentes: Campo de texto + histórico de mensagens + botão de envio.
Interação: IA interpreta entradas e responde com confirmações.

### 4.2. Tela 2: Dashboard
Componentes: Saldo atual, gastos do mês, meta em progresso.
Interação: Dados atualizados em tempo real via chat.

### 4.3. Tela 3: Metas
Componentes: Lista de metas + barra de progresso.
Interação: Criar/editar metas via chat.

### 4.4. Tela 4: Relatórios
Componentes: Gráfico de pizza + linha do tempo.
Interação: Gerados com comando "mostrar relatório".

### 4.5. Tela 5: Perfil/Configurações
Componentes: Renda mensal, categorias personalizadas, preferências de acessibilidade.
Interação: Alterar preferências via chat ou formulário simplificado.

---

## 5. Entregável da IA (Lovable)

Gerar um plano de MVP com as principais telas, recursos necessários e um esboço de validação inicial. Usar tom educativo e linguagem acessível, em português.

Interações com Deepseek:
1- "Olá, gostaria que me ajudasse a revisar meu Product Required Document para utilizá-lo no lovable para exercitar minhas habilidades de vibecoding. Ficarei feliz se como resposta você me enviasse a revisão de forma sintetizada e didatica trazendo os conceitos de vibe coding e PRD para enriquecer meus estudos: ..."
2- "Gostaria que adicionasse ao PRD a necessidade de um desing universal e salientasse a sua importância, dando visibilidade e acesso para grupos que possuem debilidades."
3- "Poderia me enviar uma versão final do prd revisada como snippet txt e sem emojis, apenas markdown."

Interação lovable:
1- "Crie um app de finanças pessoais considerando o PRD:..."

Prints:
<img width="1880" height="941" alt="Deepseek print 1" src="https://github.com/user-attachments/assets/1cdfa847-b887-450b-9eb9-90f2f8b1a9cb" />
<img width="1846" height="909" alt="Deepseek print 2" src="https://github.com/user-attachments/assets/9474b2cc-a1bf-4701-8911-eb1b3b2058ec" />
<img width="1884" height="936" alt="Lovable print 1" src="https://github.com/user-attachments/assets/28d68d98-3677-42bb-910f-7135e9172e73" />
<img width="1898" height="929" alt="lovable app 4" src="https://github.com/user-attachments/assets/1781762d-06f1-41dd-8d37-9bfe1df757d7" />

<img width="1246" height="899" alt="lovable app 1" src="https://github.com/user-attachments/assets/f42a5187-f857-407f-8be7-605ad31069e2" />
<img width="1256" height="899" alt="lovable app 3" src="https://github.com/user-attachments/assets/47f1b18b-c588-45c7-ab12-198c792d10d3" />
<img width="1246" height="899" alt="lovable app 2" src="https://github.com/user-attachments/assets/37707874-a30f-43be-a5d3-97ce283912e0" />

# O que o app faz?

Um assistente financeiro pessoal que funciona por meio de conversas em linguagem natural, permitindo que o usuário gerencie suas finanças de forma simples, sem planilhas ou formulários complexos.

## Funcionalidades Principais

- Registra gastos via chat (ex: "Gastei R$50 no supermercado")
- Classifica automaticamente as transações em categorias
- Ajuda a definir e acompanhar metas de economia
- Oferece dicas personalizadas de economia
- Gera relatórios visuais sob demanda

## Público-Alvo

Pessoas iniciantes em controle financeiro que buscam uma solução prática, acessível e sem complicações.

## Diferenciais

- Interface conversacional e intuitiva
- Design universal e acessível para todos os usuários
- Recomendações automáticas baseadas no histórico
- Experiência personalizada e motivadora

## Tecnologia

Construído com abordagem de vibe coding, utilizando ferramentas low-code com IA para desenvolvimento ágil.

##Reflexão:
  - O que funcionou bem?
  O PRD gerado ajudou pois permitiu que eu pudesse ter um resultado satisfatório na primeira interação com o Lovable e que ja gastou todos os créditos.
  - O que não funcionou como o esperado?
  A montagem do PRD, que em geral, ao dar o incentivo correta a velocidade e a quantidade de interação com a IA foi minimizado e mesmo assim alcançou um ótimo resultado. 
  - O que aprendeu sobre conversar com IAs?
  Que se receberem prompts bem construidos sao capazes de trazer alta assertividade no resultado de um projeto, acelerando o desenvolvimento.

  link do resultado: https://chat-financeiro-legal.lovable.app
