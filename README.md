
Sistema de Contratação e Demissão — QBCore
==========================================

Um script simples e funcional para servidores FiveM usando o framework QBCore, que permite convidar jogadores para empregos (jobs) e demiti-los com confirmação via menu interativo.

Funcionalidades
---------------
- Comando `/contratar [ID] [job]` convida o jogador a ingressar em um emprego.
- Comando `/demitir [ID]` envia uma solicitação de desligamento com confirmação.
- Menus interativos com `qb-menu` para aceitar/recusar convite ou demissão.
- Totalmente integrado ao sistema de empregos do QBCore.
- Mensagens de notificação via `QBCore.Functions.Notify`.

Exemplo de uso
--------------
✅ Contratar jogador:
    /contratar 10 police
    O jogador ID 10 verá um menu perguntando se deseja entrar para a organização 'police'.

❌ Demitir jogador:
    /demitir 10
    O jogador ID 10 verá um menu perguntando se deseja sair da organização atual e voltar a ser 'unemployed'.

Dependências
------------
- qb-core
- qb-menu
- Sistema de jobs padrão do QBCore

Estrutura do Script
-------------------
contratar/
├── client.lua
├── server.lua
├── fxmanifest.lua

Instalação
----------
1. Coloque a pasta `contratar` em sua pasta `resources`.
2. Adicione ao server.cfg:
       ensure contratar
3. Certifique-se que `qb-core` e `qb-menu` estão funcionando corretamente.

Permissões
----------
O script não faz checagem de permissão por grupo/admin, mas pode ser facilmente adaptado usando QBCore.Functions.HasPermission.

Autor
-----
Feito por Mulambo - Crash Store https://discord.gg/r6VEw4fXzQ
Licença
-------
Este projeto é de uso livre, mas mantenha os créditos.
