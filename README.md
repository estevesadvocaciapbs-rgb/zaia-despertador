# Despertador da Za.Ia

Recebe os avisos (webhooks) da Za.Ia e religa o plantão do despachante do funil se ele estiver parado.

- Gatilho: `repository_dispatch` (o tipo do evento é o nome do evento da Za.Ia; o botão Testar manda `teste`).
- Segredo `DESPACHANTE_TOKEN`: token fine-grained só do repositório despachante-funil, permissão Actions: Read and write.
- O token cadastrado na Za.Ia é outro, só deste repositório (Contents: Read and write).
- Repositório público: o conteúdo do aviso nunca vai para o log.
