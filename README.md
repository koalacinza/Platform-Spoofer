# Platform-Spoofer

O **Platform-Spoofer** permite configurar a identificação de plataforma do Discord pelo BetterDiscord. Você pode marcar uma ou várias opções, como **PC + celular** ou **PC + console**.

### O que dá para selecionar?

- **PC** — cliente para Windows
- **Navegador** — versão web
- **Celular** — Discord para Android
- **Meta Quest** — identificação de VR
- **Console** — identificação de PlayStation

As opções são independentes: marque apenas as que quiser ou use os botões **Selecionar todas** e **Desativar todas**. As escolhas ficam salvas e são aplicadas com uma reconexão automática, sem precisar reiniciar o Discord.

## Como instalar

1. Coloque o arquivo `Platform-Spoofer.plugin.js` na pasta de plugins do BetterDiscord.
2. No Discord, abra **Configurações → BetterDiscord → Plugins** e ative **Platform-Spoofer**.
3. Entre nas configurações do plugin e escolha suas plataformas.

A pasta de plugins depende do sistema:

```text
Windows  %appdata%\BetterDiscord\plugins
Linux    ~/.config/BetterDiscord/plugins
macOS    ~/Library/Application Support/BetterDiscord/plugins
```

## Conferindo pelo console

Se quiser verificar a seleção ou tentar uma nova conexão, abra o console de desenvolvedor do Discord e use:

```js
__ps.status();     // Plataformas marcadas e estado das conexões
__ps.sessions();   // Sessões que o cliente consegue consultar
__ps.reconnect();  // Força uma nova conexão
```

> **Atenção:** este é um plugin não oficial que modifica o funcionamento da conexão do Discord. O uso pode contrariar os Termos de Serviço da plataforma. Utilize por sua conta e risco.
