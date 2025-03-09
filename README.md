# Projeto DSCommerce
### Projeto: Sistema de Comercio
[![NPM](https://img.shields.io/badge/license-MIT-npm)](https://github.com/olarthur/dscommerce/blob/main/LICENSE)
## Sobre o Projeto
O projeto foi desenvolvido em conjunto com o curso Java Spring Professional, organizado pelo Professor [Nelio](https://github.com/acenelio)
da comunidade [DevSuperior](https://devsuperior.com.br/) e conta com o back-end do sistema de um comércio.<br>
<br>
O sistema deve manter um cadastro de usuário, produtos e suas categorias. Cada
usuário possui nome, email, telefone, data de nascimento e uma senha de acesso. Os
dados dos produtos são: nome, descrição, preço e imagem. <br>
<br>
O sistema apresenta um catálogo de produtos, os quais podem ser filtrados pelo nome do produto. A partir
desse catálogo, o usuário pode selecionar um produto para ver seus detalhes e para
decidir se o adiciona a um carrinho de compras. O usuário pode incluir e remover itens
do carrinho de compra, bem como alterar as quantidades de cada item. Uma vez que o
usuário decida encerrar o pedido, o pedido deve então ser salvo no sistema com o status
de "aguardando pagamento". <br> 
<br>
Os dados de um pedido são: instante em que ele foi salvo,
status, e uma lista de itens, onde cada item se refere a um produto e sua quantidade no
pedido. O status de um pedido podem ser: aguardando pagamento, pago, enviado,
entregue e cancelado. Quando o usuário paga por um pedido, o instante do pagamento
deve ser registrado. <br>
<br>
Usuários do sistema podem ser clientes ou administradores,
sendo que todo usuário cadastrado por padrão é cliente. Aqueles não identificados
podem se cadastrar no sistema, navegar no catálogo de produtos e no carrinho de
compras. Clientes podem atualizar seu cadastro no sistema, registrar pedidos e visualizar
seus próprios pedidos. Usuários administradores tem acesso à área administrativa onde
pode acessar os cadastros de usuários, produtos e categorias. 

## Modelo Conceitual
![Modelo Conceitual](https://github.com/olarthur/dscommerce/blob/main/assets/modelo-conceitual.png)

## Casos de Uso
![Casos de Uso](https://github.com/olarthur/dscommerce/blob/main/assets/casos-de-uso.png)

## Tecnologias Utilizadas
- **Linguagem:** Java. 
- **Framework:** Spring Boot.
- **Acesso a Banco de Dados:** Spring Data JPA.
- **Validação:** Bean Validation.
- **Controle de Acesso:** OAuth2 e JWT.
- **Gerenciamento de Depedência:** Maven.
- **Banco de dados:** H2 e Postgres.
- **Ferramenta de Teste:** Postman.

## Como executar o projeto
- **Pré-Requisitos:** Java 11


  ```bash
  # clonar o repositório
  git clone https://github.com/olarthur/dscommerce.git

  # entrar na pasta
  cd dscommerce

  # configure o projeto
  mvn clean install

  # rode a aplicação
  mvn spring-boot:run
  ```

- **Teste os endpoints**
  - Baixe a collection do projeto: [Collection](https://drive.google.com/file/d/14h48Dqi7mC8Srqfh2tBXesKo24IaVc1t/view?usp=drive_link)
  - Baixe o environment: [Environment](https://drive.google.com/file/d/1n3Ycib8WhF8BS4TgktuFpv2E4H6p5Nr1/view?usp=drive_link)
  - Importe-os no PostMan e Teste
