# Instalação (só o que faltar)

Guie um passo de cada vez e espere a pessoa dizer que fez antes de passar ao próximo. Login, senha e autorização são sempre dela.
Os menus do Claude podem aparecer em português ou em inglês: os dois nomes estão aqui.

## A skill
Se você está lendo isto, a skill já está instalada nesta conversa. Esta parte serve para quando a pessoa quer instalar em outro app, atualizar, ou quando ela te mandou só o guia em PDF.
Arquivo: social-media.zip (o link está no guia). A pasta de dentro se chama social-media.

- **Claude no navegador, no app do computador ou no Cowork:**
  1. Configurações → Recursos (Settings → Capabilities): ligar "Criar e editar arquivos" (Create and edit files).
  2. Abrir claude.ai/customize/skills, ou Personalizar → Habilidades (Customize → Skills).
  3. Botão "+" → Criar habilidade (Create skill) → Fazer upload de uma habilidade (Upload a skill) → escolher o social-media.zip, sem descompactar.
  4. Conferir se a skill ficou ligada na lista.
  Para atualizar: apagar a social-media antiga na lista (abrir a skill → "..." → Excluir) e enviar o zip novo.
- **Claude Code:** a pasta fica em ~/.claude/skills/social-media/. Rodar na pasta onde o zip foi baixado (normalmente Downloads).
  - Mac/Linux: `cd ~/Downloads && mkdir -p ~/.claude/skills && unzip -o social-media.zip -d ~/.claude/skills/`
  - Windows (PowerShell): `cd $HOME\Downloads; Expand-Archive social-media.zip -DestinationPath $HOME\.claude\skills -Force`
  Abrir uma sessão nova do Claude Code. Para chamar pelo nome: /social-media.
- **Codex e app do ChatGPT no computador:** os dois leem a mesma pasta, ~/.agents/skills/social-media/.
  - Mac/Linux: `cd ~/Downloads && mkdir -p ~/.agents/skills && unzip -o social-media.zip -d ~/.agents/skills/`
  - Windows (PowerShell): `cd $HOME\Downloads; Expand-Archive social-media.zip -DestinationPath $HOME\.agents\skills -Force`
  Sem terminal: descompactar o zip e mover a pasta social-media para dentro de .agents/skills, na pasta de usuário (no Windows, C:\Users\[seu usuário]\.agents\skills; criar as pastas se não existirem).
  Abrir uma conversa nova. A skill aparece em Skills, na barra lateral do app do ChatGPT. Para chamar pelo nome: @social-media no ChatGPT, $social-media no Codex.
  Os mesmos comandos atualizam uma versão antiga.
- **ChatGPT no navegador ou no celular:** skills avulsas não funcionam lá (só as que vêm dentro de plugins), segundo a documentação da OpenAI. Use o app do ChatGPT no computador, ou o modo anexo abaixo.
- **Outro app compatível com Agent Skills** (o formato aberto de pasta com SKILL.md): colocar a pasta social-media onde o app procura skills. Veja a documentação do app.
- **App sem suporte a skills:** a pessoa pode anexar os arquivos .md da pasta no começo da conversa. Funciona, mas precisa anexar de novo a cada conversa.

Se você tem acesso a arquivos e terminal no computador da pessoa, pode baixar o zip e fazer a cópia você mesmo, depois de mostrar o comando e a pessoa concordar. Anexo de conversa nem sempre fica no computador dela: se a cópia falhar, não insista. Passe o caminho manual acima ou use o modo anexo.

### Modo anexo (quando não dá para instalar)
Se a pessoa anexou o social-media.zip na conversa e você consegue abrir arquivos:
1. Descompacte o zip no seu espaço de trabalho.
2. Leia SKILL.md e depois verificacao.md, e siga a skill normalmente nesta conversa.
3. Avise: "Estou usando a skill pelo anexo. Vale só para esta conversa; para as próximas, instale ou anexe o zip e a ficha de novo."
No modo anexo, a ficha é ainda mais importante: entregue a ficha atualizada no fim de cada pedido.

## Replin (números da conta e direct automático)
Primeiro, fora do assistente (só a pessoa faz):
1. Criar a conta grátis em replin.com.br (não pede cartão).
2. Dentro da Replin, conectar o Instagram pelo login oficial da Meta. Precisa ser conta profissional (Criador ou Empresa). Se a conta ainda é pessoal: nas configurações do Instagram, procure "conta profissional" e faça a troca (é grátis).

Depois, ligar a Replin no app. O endereço é sempre o mesmo: https://api.replin.com.br/mcp
- **Claude no navegador/app:** Personalizar → Conectores (Customize → Connectors) → Descobrir (Browse), procurar Replin → Conectar → entrar na Replin e Permitir. Não achou: Adicionar → Conector personalizado (Add custom connector), nome Replin, colar o endereço.
- **Claude Code:** `claude mcp add --scope user --transport http replin https://api.replin.com.br/mcp`, depois, dentro do Claude Code, `/mcp` → replin → entrar e autorizar no navegador.
- **App do ChatGPT no computador:** Configurações (Settings) → Servidores MCP (MCP servers) → Adicionar servidor (Add server) → nome replin, tipo Streamable HTTP, colar o endereço → Salvar → Reiniciar (Restart). Na lista, clicar em Autenticar (Authenticate) e entrar na Replin. Para conferir: digitar /mcp no campo de mensagem.
- **Codex (terminal):** `codex mcp add replin --url https://api.replin.com.br/mcp`. Se não abrir o login sozinho: `codex mcp login replin` e autorizar no navegador. O app do ChatGPT no computador e o Codex dividem a mesma configuração: ligou em um, vale para o outro.
- **ChatGPT no navegador ou no celular:** lá os conectores só entram por plugins. Sem a Replin, siga com os números colados pela pessoa.
- **Outro app:** qualquer app compatível com conectores MCP aceita o mesmo endereço, segundo a Replin.

Teste: chame a ferramenta da Replin que lista as contas (accounts_list). Apareceu o @? Está ligado. Veio vazio? Falta o passo 2 acima: use a ferramenta que devolve o link de conexão (instagram_connect).

## Busca na web
- **Claude no navegador/app:** no campo de mensagem, no menu de ferramentas, ligar a busca na web (Web search).
- **Claude Code e Codex:** a busca costuma vir disponível. Se não estiver, a pessoa pode colar o que viu no nicho.

## Projeto (só no chat do Claude, recomendado)
Criar um Projeto chamado "Instagram" e fazer as conversas de social media dentro dele. A ficha fica salva nos arquivos do projeto e toda conversa nova já começa com ela.

Ao terminar, volte para verificacao.md e refaça o teste.
