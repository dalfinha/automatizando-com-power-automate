# Fluxos no Power Automate

# 1º - Protótipo: Notificando uma nova tarefa do Planner
## Observações ⭐
- Não foram utilizadas Conexões Premium para construção do fluxo.
- É importante lembrar que algumas organizações/ambientes possuem <a href="https://learn.microsoft.com/pt-br/power-platform/admin/wp-data-loss-prevention">políticas de DLP</a> - o que fazem com que a conexão do Gmail não esteja disponível. Porém você pode substitui-la pelo Envio de E-mail pelo Outlook. 
- O e-mail é construído com HTML e CSS, adicionado na conexão de envio de e-mail. 

## O que o fluxo faz? ⭐
- Utilizando a conexão do Planner com o Gmail, a partir do gatilho "Quando uma tarefa é atribuída a mim" é enviado um e-mail com o nome da tarefa, descrição e um botão de direcionamento para o plano do Planner.

**Corpo do e-mail**
![image](https://user-images.githubusercontent.com/72402847/230810202-8daf68c8-38a5-4717-9a54-e33b37639cad.png)

**Corpo do fluxo**
![image](https://user-images.githubusercontent.com/72402847/230809974-b0969f7a-af82-4b49-aefb-e177bc262908.png)

## Aprimore! ⭐
- Crie mais labels no HTML do envio de e-mail e adicione as informações que achar necessário como Atribuído por, Data de Conclusão e outras.
- Crie um bot para o Teams também notifica-lo quando a tarefa estiver perto do vencimento. 
- Ao mudar a classificação ou rótulo da tarefa, envie um e-mail para quem atribuiu a tarefa informando que está enfrentando dificuldades.
