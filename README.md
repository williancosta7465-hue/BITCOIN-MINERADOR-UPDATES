# ₿ Bitcoin Minerador Solo

Minerador experimental de Bitcoin em **solo mining via CKPool** para Windows, com histórico persistente, atualização automática, Watchdog 2.0, diagnóstico 24/7 e monitoramento online opcional.

> **Versão estável atual: v2.2.0**

## ⬇️ BAIXAR O MINERADOR

### [Baixar Bitcoin Minerador Solo v2.2.0 — Windows x64](https://raw.githubusercontent.com/williancosta7465-hue/BITCOIN-MINERADOR-UPDATES/main/releases/v2.2.0/BitcoinMineradorSolo_Setup_v2.2.0.exe)

O instalador usa arquitetura `onedir` e instala o programa em uma pasta fixa do Windows. Depois da instalação, as próximas versões estáveis podem ser recebidas pelo botão **Verificar atualizações** dentro do próprio programa.

Para conferir a versão publicada e os hashes SHA-256, consulte [`latest-v2.json`](./latest-v2.json).

## O que o programa mostra

- Hashrate atual e gráfico dos últimos minutos
- Hashes da sessão e hashes históricos
- Shares encontradas, aceitas e rejeitadas
- Melhor dificuldade e melhor hash histórico
- Tempo da sessão e tempo total de mineração
- Quedas de conexão e tempo offline
- Watchdog 2.0 com heartbeat individual dos workers
- Página **Diagnóstico 24/7**
- Atualização automática com verificação SHA-256
- Página **Monitoramento** para servidor próprio

## Como começar

1. Instale o programa.
2. Abra **Configurações**.
3. Informe **somente o endereço público Bitcoin** que receberia uma eventual recompensa.
4. Escolha o perfil de carga: Leve, Normal ou Máximo.
5. Clique **Iniciar**.
6. Quando aparecer **Conectado ao CKPool**, o minerador está trabalhando.

## 📱 Monitoramento pelo celular — v2.2.0

A v2.2.0 permite acompanhar o minerador de qualquer lugar usando um **PWA**, que pode ser adicionado à tela inicial do celular sem APK e sem Play Store.

Arquitetura:

`Bitcoin Minerador Solo → seu servidor Cloudflare → Bitcoin Minerador Monitor no celular`

O painel exibe status online/offline, hashrate, hashes, shares, melhor dificuldade, blocos, workers, último job, tempo minerando, quedas, tempo offline, watchdog e eventos recentes.

### Configuração

1. Criar uma conta gratuita na Cloudflare.
2. Criar o servidor Worker + D1 usando o modelo do projeto.
3. Criar duas chaves exclusivas: `DEVICE_KEY` e `VIEW_KEY`.
4. No minerador, abrir **Monitoramento**, informar a URL do servidor e as duas chaves e clicar **Testar conexão**.
5. Clicar **Conectar celular • QR Code**.
6. Escanear o QR Code com o celular.
7. Adicionar **Bitcoin Minerador Monitor** à tela inicial.

Cada pessoa pode usar **a própria conta Cloudflare e o próprio servidor**. O programa não depende de um servidor central do desenvolvedor.

### Segurança do monitoramento

- `DEVICE_KEY` autoriza o minerador a enviar status e eventos.
- `VIEW_KEY` autoriza o celular a consultar o painel.
- As chaves devem ficar apenas no servidor e nos dispositivos autorizados.
- O snapshot de monitoramento não envia seed, chave privada, senha da carteira ou token administrativo.

## Segurança

- Nunca informe seed, palavras de recuperação, chave privada ou senha da carteira ao programa.
- O minerador precisa apenas do **endereço público BTC**.
- Tokens administrativos não devem ser colocados no código ou publicados no GitHub.
- Softwares de mineração podem ser sinalizados por antivírus. Verifique a origem e os hashes antes de executar; não é recomendado desativar o antivírus globalmente.

## Importante

CPU mining de Bitcoin possui probabilidade extremamente pequena de encontrar um bloco. Este projeto é um experimento de solo mining e **não representa promessa de renda ou retorno financeiro**.

---

### Canal de atualizações

Este repositório contém os pacotes e metadados necessários para distribuição e atualização do Bitcoin Minerador Solo. Dados pessoais, configurações locais, logs, seed, chave privada, senha de carteira e tokens não devem ser publicados aqui.
