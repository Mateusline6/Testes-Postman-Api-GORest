# Testes-Postman-Api-GORest
Este conjunto de testes foi desenvolvido para validar a funcionalidade de uma API que gerencia usuários, posts e comentários. Os testes estão organizados de maneira a garantir que todas as requisições sejam executadas na ordem correta, evitando falhas devido a dependências entre os endpoints.

Fluxo de Execução dos Testes
Os testes devem ser executados seguindo a ordem abaixo, pois cada etapa depende da anterior:

Criação de Usuário

Um usuário é criado de maneira aleatória, e seu ID é armazenado em uma variável de ambiente (idUsuario).
Testes validam se os dados foram gerados corretamente (nome, e-mail, gênero e status).
Criação de Post

Um post é criado e associado ao usuário recém-criado (user_id).
O ID do post é salvo na variável de ambiente (random_post_id).
Testes validam se o título e o corpo do post foram gerados corretamente.
Busca de Posts

Testes para validar a busca de todos os posts.
Teste específico para validar a busca de um post pelo seu ID.
Criação de Comentário

Um comentário é criado e vinculado ao post criado anteriormente (post_id).
As informações geradas são armazenadas em variáveis de ambiente (random_comment_id, random_body, random_email, random_name).
Testes validam se os dados foram gerados corretamente.
Busca de Comentários

Testes validam a busca de todos os comentários.
Testes verificam a busca de um comentário específico pelo seu ID.
Execução dos Testes
Para rodar todos os testes corretamente, basta executar a Collection Runner no Postman, garantindo que as variáveis de ambiente estão sendo salvas corretamente.
Os testes incluem validações para garantir que todos os valores aleatórios gerados são corretamente armazenados e utilizados nas requisições seguintes.
Caso algum teste falhe, verifique se as variáveis de ambiente estão sendo corretamente atribuídas e reutilizadas.
Objetivo dos Testes
Os testes garantem que:

Os endpoints da API estão funcionando conforme esperado.
Os dados gerados aleatoriamente são válidos e coerentes.
Todas as requisições são executadas na ordem correta, evitando erros de dependência entre endpoints.
As respostas da API seguem o formato esperado, retornando os dados corretamente.
