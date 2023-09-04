# API-DevHouse

Neste projeto, mergulhei de cabeça no mundo do desenvolvimento web, utilizando tecnologias como MongoDB, Express.js e Yarn para criar uma plataforma que permite aos usuários cadastrar, atualizar e até mesmo excluir casas disponíveis para aluguel. Cada casa é única, com detalhes que vão desde fotos incríveis até descrições cativantes, preços acessíveis, localizações estratégicas e um status claro sobre sua disponibilidade para aluguel. 
Uma das características mais empolgantes deste projeto foi a implementação de um sistema de login seguro com validação de e-mail, garantindo que apenas usuários autenticados possam acessar e interagir com a plataforma. Aqui estão as rotas para o funcionamento da API:

Endpoint/Requisições
Execultando via localhost no Postman, as solicitações possíveis são:

Session

GET:
     http://localhost:3333/sessions
     -Loga um usuário no sistema com o Email


House

GET:
     http://localhost:3333/houses?status=
     -Requisição para listar todas as casas cadastradas podendo ser

         {true}
          -Retorna as casas disponíveis para aluguel

         {false}
          -Retorna as casas indisponiveis para aluguel

Post:
      http://localhost:3333/houses
      -Requisição para cadastrar uma casa no sistema

Put:
     http://localhost:3333/houses/ 
     -Id da casa na qual deseja atualizar ou editar = {64f3ab89845c5b82bc70e2e5}

Delete:
       http://localhost:3333/houses
       -Requisição para deletar uma casa



Dashboard

Get:
     http://localhost:3333/dashboard
     -Requisição para buscar todas as casas cadastras pelo usuário que está logado


Reserves

Get:
    http://localhost:3333/reserves
    -Requisição para listar as reservas do usuário

Post:
     http://localhost:3333/houses/64f3d9e19a7b6d1efabe2f4f/reserve
     -Rquisição para fazer uma reserva {64f3d9e19a7b6d1efabe2f4f = id do usuario logado} 

Delete: 
       http://localhost:3333/reserves/cancel
       -Requisição para cancelar uma reserva

