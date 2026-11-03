# Guia de setup — plugins, conectores e acessos

## 1. Instalar os plugins (as "skills")

Um **plugin** é um pacote de habilidades que você ativa uma vez na sua conta do Claude.
Depois disso, ele fica disponível nas conversas e eu uso quando fizer sentido.

### Pelo navegador (claude.ai) ou pelo app

1. Abra **claude.ai** (ou o app do Claude no computador).
2. No menu lateral esquerdo, clique em **Customize** (Personalizar).
3. Vá em **Plugins**, clique no **+** e depois em **Browse plugins** (Explorar plugins).
4. Na busca, digite o nome do plugin e clique no **+** (ou **Install**) ao lado dele.
5. Se pedir login ou permissão, siga as telas.

> Os nomes dos menus podem mudar um pouco conforme a versão do app.
> Se não achar, me manda um print da tela que eu te guio.

### Quais instalar (em ordem)

| Ordem | Plugin (nome para buscar) | Para quê | Custo |
|---|---|---|---|
| **1º — agora** | **Social Media Skills** | Roteiros de Reels, ganchos, carrosséis, otimizar bio, crescimento no Insta | Grátis |
| 2º — depois | **Windsor.ai Ads and Marketing Data** | Puxar as métricas reais do Instagram | Tem plano grátis limitado; conferir no site |
| 3º — fase 2 | **instagram** | Responder comentários e DMs (funil para Move/comunidade) | Exige configurar um app na Meta |

O plugin **Marketing** (da Anthropic) já está disponível para você.

## 2. Conectar os dados do Instagram (deixamos para depois)

Opções, todas usando a API oficial da Meta:

- **Windsor.ai** (plugin acima): bom para relatórios.
- **Metricool**: conector em Customize → **Connectors**. Também agenda posts e mostra o
  melhor horário para postar.
- **Supermetrics**: você já começou a conectar, mas não terminou. É pago.

Pré-requisitos (você já tem): conta profissional + página do Facebook vinculada.

**Até conectar:** toda segunda, mande prints de
*Painel profissional → Insights* (visão geral, contas alcançadas, seguidores, top posts)
que eu monto o relatório.

## 3. Liberar o Instagram nesta sessão na nuvem (opcional)

Para eu conseguir abrir perfis públicos (o seu e as referências) daqui:

1. No título da sessão, abra o menu do **ambiente na nuvem** e clique em **Edit**.
2. Em **Network access**, adicione `instagram.com` e `www.instagram.com` em
   **Allowed domains** (deixe marcado "Allow package managers").
3. Salve e me avise.

Passo a passo oficial: https://code.claude.com/docs/en/cloud-environments#network-access

> Mesmo liberado, o Instagram costuma bloquear leitura sem login. Prints ou a conexão
> de dados (item 2) são o caminho mais garantido.

## 4. Rotina semanal automática (quando os dados estiverem conectados)

Uma tarefa agendada toda **segunda de manhã** que:
1. puxa as métricas da semana,
2. gera o relatório em `relatorios/AAAA-MM-DD.md`,
3. sugere a pauta e os roteiros da semana.

É só pedir: "Jarvis, agenda a rotina semanal".
