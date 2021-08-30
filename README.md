# formulario-de-cadastro
Projeto que visa a implementação de um formulário de cadastro com os principais dados do usuário, como nome, CPF, RG...
## Implementação
* Foram utilizados campos com label, para que a página fique acessível a leitores de tela, para que possa ser falado o campo que será preenchido
* As informações estão agrupadas por categoria, para facilitar o entendimento do usuário na hora de preencher o formulário. Dados pessoais, endereço, informações de contato e dados de acesso da plataforma
* Os campos que contém números como CPF, RG e Cep, foi utilizado um input com inputmode type numeric, que torna visível o teclado numérico em dispositivos móveis, para os campos de telefone, foi usado um input do tipo tel
* O campo E-mail é do tipo email, para que possa ser validado automaticamente pelo navegador, bem como tentar sugerir o E-mail pro usuário
* Ao preencher o sep, uma função javascript é disparada, para pesquisar o cep na API do viacep.com.br, e ainda tenta preencher os campos do endereço automaticamente
* Os campos CPF, cep, telefone fixo e telefone celular são mascarados a medida que o usuário digita
* Os campos obrigatórios são sinalizados com *, e o atributo required foi usado para isso, pois ao submeter o formulário com campos obrigatórios em branco, o mesmo é direcionado para esse campo para que possa ser preenchido de novo
* Para enviar o formulário, além de preencher todos os campos obrigatórios, precisa está com o CPF válido, caso não queira digitar o telefone fixo e sep, deixar os campos em branco, pois ao digitar algo o script de validação vai entender que algo tinha que ser digitado e o formulário não é submetido
* Ao digitar um campo e esse ficar inválido, um alert é exibido ao usuário informando o motivo do erro, bem como focando o cursor do usuário no respectivo campo, para melhorar a experiência desse usuário, bem como melhorar a acessibilidade com leitores de tela
* Ao terminar a inserção das informações, surge na tela um diálogo de confirmação para que o usuário escolha se quer enviar o formulário. Caso clique em ok, o formulário é submetido. Será mostrado um alert, como o nome do usuário, e a confirmação do cadastro das informações
## Referências
[Consultando cep na API viacep.com.br](https://viacep.com.br/)