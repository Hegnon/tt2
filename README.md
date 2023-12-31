Teste Técnico

- [x] Escreva um método que dado um inteiro x, um inteiro y e um inteiro w retorne todos os
números divisíveis por w entre x e y.
https://github.com/users/Hegnon/projects/15/views/1 - https://github.com/Hegnon/tt2/tree/main/divisiveis%20por%20w

- [ ] Em um sistema web, cada usuário pode se inscrever em diversos eventos, cada evento
possui até 3 prêmios que são distribuídos entre os usuários presentes. O sistema precisa
guardar a informação sobre quem participou de cada evento e quem ganhou os prêmios.
Modele um banco de dados capaz de suportar essas regras.

- [ ] Considere um sistema onde cada Usuário possui os atributos nome (String), idade
(Inteiro) e profissão (String). Faça uma query que retorne o nome de todos os usuários com
idade maior ou igual à 18 anos e cuja profissão seja programador ou desenvolvedor

- [x] Quais são as vantagens/desvantagens de se usar a arquitetura MVC (Model, View e
Controller)?

* Vantagens da Arquitetura MVC:
 A arquitetura MVC (Model-View-Controller) oferece várias vantagens significativas no desenvolvimento de software. Ela promove a separação de responsabilidades, tornando o código  mais organizado e reutilizável. Com componentes claramente definidos, a manutenção se torna mais fácil, resultando em um desenvolvimento mais ágil. Além disso, a arquitetura MVC  favorece a testabilidade, permitindo a criação de testes unitários e de integração eficazes. Sua estrutura facilita a colaboração em equipes de desenvolvimento, promovendo o uso de um mesmo modelo com várias interfaces de usuário. Em resumo, o MVC é uma escolha sólida para aplicativos de médio a grande porte, proporcionando eficiência e escalabilidade.

* Desvantagens da Arquitetura MVC:
 Apesar das inúmeras vantagens, a arquitetura MVC também apresenta desvantagens. Ela inicialmente introduz complexidade no projeto, exigindo a definição de interfaces e aumento na quantidade de código. Para equipes inexperientes, há uma curva de aprendizado e adoção, tornando a transição desafiadora. A estrutura completa MVC pode ser excessiva para aplicativos pequenos, resultando em desperdício de recursos. Além disso, a comunicação entre componentes, como Controller e View, requer atenção, sendo um desafio em algumas situações. Portanto, a escolha da arquitetura deve levar em consideração as necessidades específicas do projeto e a experiência da equipe de desenvolvimento.

 - [x] Usando Ruby on Rails, cite pelo menos uma forma de criar uma rota para um método
chamado find_user dentro de um controller com o nome UsersController.

* Uma das formas mais comuns é definir uma rota personalizada no arquivo config/routes.rb

  Exemplo:
  #config/routes.rb

Rails.application.routes.draw do

  #Rota personalizada para o método find_user em UsersController
  
  get 'users/find_user', to: 'users#find_user'
  
end

 - [x] Considerando a estrutura padrão de arquivos de um projeto feito com Ruby on Rails, em
quais pastas devem se encontrar os models, os controllers e as views de um projeto? De
que modo é possível saber qual controller é responsável por gerenciar uma determinada
view?

* Models (Modelos): Os modelos representam os objetos de dados do aplicativo e geralmente estão localizados na pasta app/models. Cada modelo é geralmente definido em seu próprio arquivo com o nome no singular e em letra maiúscula (por exemplo, User para um modelo de usuário).

* Controllers (Controladores): Os controladores lidam com as solicitações do cliente e a lógica do aplicativo. Eles geralmente são armazenados na pasta app/controllers e seguem a convenção de nomes no plural, com o sufixo Controller (por exemplo, UsersController).

* Views (Visualizações): As visualizações representam a camada de apresentação do aplicativo e geralmente estão localizadas na pasta app/views. Dentro dessa pasta, você encontrará subpastas correspondentes a cada controlador, com os nomes no plural (por exemplo, users para um controlador UsersController). As visualizações para um controlador específico são armazenadas nessa subpasta.

Exemplo:

![Screenshot from 2023-10-17 06-55-10](https://github.com/Hegnon/tt2/assets/111914933/9b04f509-8c5c-4781-b835-2f6acba5cc4f)
