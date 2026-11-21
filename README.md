# social-media 🍿

Skill grátis do **Prompt & Pipoca** que coloca um social media de Instagram dentro do seu assistente de IA.

Ela analisa o seu perfil, lê os números reais da sua conta, monta a pauta da semana e escreve roteiro de reel, carrossel, legenda e o direct automático do "comenta X". Quem grava e posta é você.

Funciona no Claude (site, app e Cowork), no Claude Code, no Codex e no app do ChatGPT no computador.

## O que você precisa

- Um assistente que aceite skills (lista acima).
- Uma conta grátis na [Replin](https://replin.com.br) com o seu Instagram conectado (conta profissional: Criador ou Empresa). É dela que vêm os números da conta e o direct automático.
- Busca na web ligada no assistente, para a pesquisa de pauta.

## Instalar

### Claude Code

```
/plugin marketplace add promptepipoca/skills
/plugin install social-media@promptepipoca
```

O plugin já traz a conexão com a Replin. Depois de instalar, abra uma sessão nova, rode `/mcp`, escolha `replin` e autorize no navegador. Para chamar a skill: `/social-media:social-media`.

Para atualizar: `claude plugin marketplace update promptepipoca` e depois `claude plugin update social-media@promptepipoca`.

### Codex

```
codex plugin marketplace add promptepipoca/skills
codex plugin add social-media@promptepipoca
codex mcp login replin
```

O plugin já traz a conexão com a Replin; o último comando abre o navegador para você autorizar. Numa conversa nova, digite `$` e escolha `social-media`.

Para atualizar: `codex plugin marketplace upgrade promptepipoca`.

### App do ChatGPT no computador

Use a instalação manual abaixo (pasta `~/.agents/skills/`).

### Claude (site, app ou Cowork)

1. Baixe o `social-media.zip` em [Releases](https://github.com/promptepipoca/skills/releases/latest). Não descompacte.
2. Em Configurações → Recursos, ligue "Criar e editar arquivos".
3. Em Personalizar → Habilidades, clique em "+" → Criar habilidade → Fazer upload de uma habilidade, e envie o zip.
4. Ligue a Replin: Personalizar → Conectores → Descobrir, procure Replin e conecte. Não achou? Adicionar → Conector personalizado, nome Replin, endereço `https://api.replin.com.br/mcp`.

### Instalação manual (qualquer app)

Baixe o `social-media.zip` em Releases e descompacte a pasta `social-media` em:

- Claude Code: `~/.claude/skills/`
- Codex e app do ChatGPT: `~/.agents/skills/`

## Usar

Abra uma conversa nova e escreva:

```
quero que você seja o meu social media
```

Toda resposta dela começa com este painel:

```
PREPARAÇÃO   [x] Skill   [x] Replin   [x] Busca na web   [x] Ficha
SEMANA       [ ] Perfil   [ ] Relatório   [ ] Pauta
POST DA VEZ  [ ] Roteiro ou carrossel   [ ] Material   [ ] Legenda   [ ] Direct
Etapa atual: ...   Próxima: ...   Só avanço com o seu ok.
```

Ela faz uma etapa por vez e pergunta "Posso seguir?" antes da próxima. Se o painel não aparecer, a skill não está sendo usada: chame pelo nome (`/social-media:social-media` no Claude Code, `$social-media` no Codex, `@social-media` no ChatGPT).

Use um caminho só por app (plugin ou zip). Os dois juntos deixam a skill repetida.

Na primeira conversa ela monta a sua **ficha** (quem você é, como grava, o que já foi feito). Nas seguintes ela lê a ficha e segue de onde parou.

## O que ela não faz

- Não posta nem grava por você.
- Não inventa número: ou vem da Replin, ou vem com o link da fonte.
- Não cria nem liga nada na Replin sem mostrar antes e você aprovar.
- Não promete seguidores, views ou vendas.

## Privacidade

A skill é só texto: instruções que o seu assistente lê. Ela não envia nada para o Prompt & Pipoca. Os dados do Instagram passam pela Replin, na conta que você mesmo conecta, e seguem a política de privacidade dela.

## Licença

MIT. Use, copie e adapte à vontade.

---

Feito por [Prompt & Pipoca](https://www.instagram.com/promptepipoca/) 🍿
