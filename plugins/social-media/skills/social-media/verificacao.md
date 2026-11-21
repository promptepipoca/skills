# Preparação (uma vez, no começo de cada conversa)

Esta é a etapa "Preparação" do painel. Faça os 4 itens em ordem, todos na mesma resposta. Não pergunte o que dá para descobrir sozinho: teste primeiro, pergunte depois.

## 1. Onde estou
Descubra em que tipo de app você está, porque muda onde guardar a ficha e como instalar o que falta:
- **App com acesso a arquivos do computador** (Claude Code, Codex, app do ChatGPT no computador com acesso local, Cowork com pasta conectada, outros agentes de terminal): você consegue ler e gravar arquivos.
- **Chat no navegador ou no app** (claude.ai, Claude Desktop sem pasta conectada, ChatGPT no navegador ou no celular): você não grava arquivos no computador da pessoa; ela guarda o que você entregar.
- **Modo anexo** (você está lendo a skill de um zip anexado): avise uma vez que a skill vale só para esta conversa e que, para as próximas, é preciso instalar (instalacao.md) ou anexar o zip e a ficha de novo.
Se não tiver certeza, pergunte em uma linha: "Você está me usando no navegador, no app do computador ou no terminal?"

## 2. A ficha do criador
Procure, nesta ordem, e pare no primeiro que achar:
1. Um arquivo **ficha.md** (ou com "ficha" no nome) anexado à conversa ou nos arquivos do Projeto (no Claude, Projetos guardam arquivos para todas as conversas daquele projeto).
2. Com acesso a arquivos: **~/social-media/ficha.md** (pasta pessoal da pessoa) ou **ficha.md** na pasta de trabalho atual.
3. A memória do app, se ele tiver e estiver ligada: procure "ficha do social media" ou o @ do Instagram.

**Achou:** leia inteira. Diga a data da última atualização e o que estava pendente (por exemplo, "o reel de quinta ainda está como roteiro pronto, sem legenda"). Se a ficha tiver mais de 30 dias, avise e pergunte se algo mudou em "Quem eu sou".
**Não achou:** pergunte "É a primeira vez que a gente trabalha junto?".
- Primeira vez: crie a ficha a partir de ficha-modelo.md. Pergunte só os campos de "Quem eu sou" que faltam, em no máximo 2 mensagens. O que der para puxar da Replin (bio, seguidores), puxe. Se a pessoa não tiver três legendas de que goste, siga sem elas e anote "sem exemplos".
- Não é a primeira vez: peça para anexar a ficha. Se a pessoa não tiver, refaça só os campos de "Quem eu sou" e siga.

**Onde guardar a ficha** (diga à pessoa onde ficou, toda vez que criar ou atualizar):
- Com acesso a arquivos: grave em ~/social-media/ficha.md (crie a pasta se não existir) ou na pasta que a pessoa preferir.
- No chat: entregue a ficha como arquivo ficha.md para baixar. Peça para salvar nos arquivos do Projeto "Instagram", **apagando a versão anterior** para não ficarem duas, ou para anexar no começo das próximas conversas. Se o app tiver memória ligada, guarde também um resumo curto lá.

## 3. A Replin (os números e o direct automático)
Teste, não pergunte: chame a ferramenta da Replin que lista as contas conectadas (accounts_list).
- **Respondeu com a conta:** confirme o @ com a ficha. Se houver mais de uma conta, pergunte qual e anote na ficha. Se vier marcada para reconectar, diga que a pessoa precisa reconectar o Instagram dentro do app da Replin (só ela faz isso).
- **Respondeu, mas sem nenhuma conta do Instagram:** a Replin está ligada, falta conectar o Instagram. Chame a ferramenta da Replin que devolve o link de conexão (instagram_connect), mostre o link e os passos, e espere a pessoa conectar. Depois teste de novo.
- **Não existe ferramenta da Replin, ou deu erro de acesso:** o conector não está ligado. Siga instalacao.md, parte "Replin", para o app em que você está. Depois de ligar, teste de novo. Em alguns apps o conector só aparece numa conversa nova: se for o caso, peça para abrir uma conversa nova e mandar a mesma mensagem.
- **A pessoa não quer usar a Replin agora:** siga sem ela, pedindo os números colados (texto ou print), e anote na ficha "sem Replin". Sem Replin não há direct automático: na hora da legenda, entregue os textos para a pessoa usar na ferramenta que preferir.

## 4. Busca na web
A pauta precisa pesquisar o que está em alta. Se você não tem busca na web ligada, diga onde ligar (instalacao.md, parte "Busca na web") e, enquanto isso, peça para a pessoa colar o que viu no nicho.

## Não pule etapas
- O que você lembra do criador (memória do app, conversas antigas) serve para preencher a ficha mais rápido, e só. Confirme com a pessoa o que for usar e não saia propondo conteúdo com base nisso.
- Não comece a análise do perfil nem o relatório antes de fechar os itens 2 e 3. Sem ficha, crie a ficha primeiro.
- Na Preparação você só testa se a Replin responde (lista de contas). Não puxe posts, totais nem horários: isso é das etapas Perfil e Relatório.
- Replin não ligada: pare e ofereça ligar agora. Só siga sem ela se a pessoa disser que quer seguir sem.
- Se uma instalação falhar, diga o que falhou e dê o caminho manual para o app em que você está (instalacao.md). Não siga em frente como se tivesse dado certo.

## Resultado
Feche a Preparação assim, e pare:
1. O painel do SKILL.md, com a linha PREPARAÇÃO marcada conforme o que você encontrou e as linhas SEMANA e POST DA VEZ marcadas pelo que está na ficha.
2. Três linhas:
   - Ficha: [achei de dd/mm | criei agora | falta]
   - Replin: [ligada na @conta | falta ligar | sem Replin]
   - Busca na web: [ligada | desligada]
3. O que acontece agora:
   - **Faltou algo na Preparação:** diga o que é e passe o primeiro passo para resolver (instalacao.md). Não faça mais nada nesta resposta.
   - **Preparação completa e pedido genérico:** diga qual é a primeira etapa em aberto e pergunte "Posso seguir?".
   - **Preparação completa e pedido específico:** faça a etapa pedida, e só ela.
Anote em "O que está ligado" na ficha, e só isso. Não preencha outras partes da ficha na Preparação.
