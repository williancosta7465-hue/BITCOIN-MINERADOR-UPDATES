# ₿ Bitcoin Minerador Solo

Minerador experimental de Bitcoin em **solo mining via CKPool**, com interface para Windows, histórico persistente, atualização automática e diagnóstico 24/7.

> **Versão estável atual: v2.1.3**

## ⬇️ Baixar o instalador

**[Baixar Bitcoin Minerador Solo v2.1.3 para Windows x64](https://raw.githubusercontent.com/williancosta7465-hue/BITCOIN-MINERADOR-UPDATES/main/releases/v2.1.3/BitcoinMineradorSolo_Setup_v2.1.3.exe)**

O instalador usa arquitetura `onedir` e instala o programa em uma pasta fixa no Windows. As próximas versões podem ser recebidas pelo botão **Verificar atualizações** dentro do próprio aplicativo.

Para conferir a versão publicada e os hashes SHA-256, consulte [`latest-v2.json`](./latest-v2.json).

## O que o programa mostra

- Hashrate atual e gráfico dos últimos minutos
- Hashes da sessão e hashes históricos
- Shares encontradas, aceitas e rejeitadas
- Melhor dificuldade e melhor hash histórico
- Tempo total de mineração
- Quedas de conexão e tempo offline
- Watchdog 2.0 com heartbeat por worker
- Página **Diagnóstico 24/7**
- Atualização automática com verificação SHA-256

## Como começar

1. Instale o programa.
2. Abra **Configurações**.
3. Informe **somente o endereço público Bitcoin** que receberia uma eventual recompensa.
4. Escolha o perfil de carga: Leve, Normal ou Máximo.
5. Clique **Iniciar**.
6. Quando aparecer **Conectado ao CKPool**, o minerador está trabalhando.

## Monitoramento pelo celular

Está em desenvolvimento a versão **v2.2.0**, com monitoramento online por PWA: um painel que pode ser adicionado à tela inicial do celular sem APK ou Play Store. A arquitetura prevista usa um servidor Cloudflare configurável pelo próprio usuário, para que cada pessoa possa manter seus próprios dados e sua própria conta.

A configuração será guiada pelo programa e por uma página **Primeiros passos**, incluindo criação do servidor, conexão do minerador e pareamento do celular por QR Code.

## Segurança

- Nunca informe seed, palavras de recuperação, chave privada ou senha da carteira ao programa.
- O minerador precisa apenas do **endereço público BTC**.
- Tokens de GitHub, Cloudflare ou outras credenciais administrativas não devem ser colocados no código nem publicados neste repositório.
- Softwares de mineração podem ser sinalizados por antivírus. Verifique a origem e os hashes antes de executar; não é recomendado desativar o antivírus globalmente.

## Importante

CPU mining de Bitcoin possui probabilidade extremamente pequena de encontrar um bloco. Este projeto é um experimento de solo mining e **não representa promessa de renda ou retorno financeiro**.

---

### Canal de atualizações

Este repositório público contém os pacotes e metadados necessários para distribuição e atualização do Bitcoin Minerador Solo. Dados pessoais, configurações locais, logs, seed, chave privada, senha de carteira e tokens não devem ser publicados aqui.
