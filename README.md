# 1º PROJETO PRÁTICO - DADOS
Primeiro projeto prático do Programa Desenvolve 2024 - Grupo Boticário em parceria com Alura (Trilha de Dados)

O projeto consiste na construção de um modelo de banco de dados relacional que representa o negócio do Boticário. Ele leva em consideração os conceitos e entidades relacionados à parte de vendas, sistema de pontuação e gestão de produtos em estoque.

<br>

## ✏️ Índice:

1. <a href="#entidades">Entidades</a>
2. <a href="#modelo-conceitual">Modelo Conceitual</a>
3. <a href="#modelo-logico">Modelo Lógico</a>
4. <a href="#modelo-fisico">Modelo Físico</a>
5. <a href="#tecnologias">Tecnologias Utilizadas</a>
6. <a href="#pessoas-autoras">Pessoas Autoras</a>

<br>

<span id="entidades"></span>

## 1. 📝 Entidades

### Neste projeto trabalharemos com sete entidades (tabelas).

1.1 - CLIENTES
* Aqui faremos o registro dos clientes, esta tabela contém seis atributos diretos, são eles:
    * cliente_id (primary key de identificação do cliente);
    * nome;
    * telefone_1;
    * telefone_2 (Opcional);
    * email;
    * cpf.
<br>

#### Exemplo de SELECT de clientes 
![tabela_clientes](/imagens/tabela_clientes.jpg)

<br><br>

1.2 - ENDEREÇOS
* Aqui faremos o registro dos endereços, esta tabela contém sete atributos, são eles:
    * cliente_id (foreign key - relação com a tabela clientes);
    * endereco_id (primary key - identificador do endereço);
    * rua;
    * bairro;
    * cidade;
    * cep;
    * estado.

<br>

#### Exemplo de SELECT de endereços
![tabela_clientes](/imagens/tabela_enderecos.jpg)

<br><br>

1.3 - PEDIDOS
* Aqui faremos o registro dos pedidos, esta tabela contém quatro atributos:
    * cliente_id (foreign key - relação com a tabela clientes);
    * pedido_id (primary key - identificador do pedido);
    * valor_pedido;
    * data_pedido.

<br>

#### Exemplo de SELECT de pedidos
![tabela_clientes](/imagens/tabela_pedidos.jpg)

<br><br>

1.4 - CATEGORIAS
* Aqui faremos o registro das categorias, esta tabela contém dois atributos:
    * categoria_id (foreign key - relação com a tabela categorias);
    * nome.    

<br>

#### Exemplo de SELECT de categorias
![tabela_clientes](/imagens/tabela_categorias.jpg)

<br><br>

1.5 - PRODUTOS
* Aqui faremos o registro dos produtos, esta tabela contém cinco atributos:
    * categoria_id (foreign key - relação com a tabela categorias);
    * produto_id (primary key - identificador do produto);
    * valor_produto;
    * nome;
    * descricao.

<br>

#### Exemplo de SELECT de produtos
![tabela_clientes](/imagens/tabela_produtos.jpg)

<br><br>

1.6 - PEDIDOS_PRODUTOS
* Aqui faremos o registro do relacionamento M:N entre pedidos e produtos, esta tabela contém três atributos:
    * pedido_id (foreign key - relação com a tabela pedidos);
    * produto_id (foreign key - relação com a tabela produtos);
    * qtd_produto.

<br>

#### Exemplo de SELECT de pedidos_produtos
![tabela_clientes](/imagens/tabela_pedidos_produtos.jpg)

<br><br>

1.7 - ESTOQUE
* Aqui faremos o registro dos produtos em estoque, esta tabela contém dois atributos:
    * produto_id (foreign key/primary key - relação com a tabela produtos e também identificador do registro);
    * qtd_estoque.

<br>

#### Exemplo de SELECT de estoque
![tabela_clientes](/imagens/tabela_estoque.jpg)

<br><br>

<span id="modelo-conceitual"></span>

## 2. 📐 Modelo Conceitual

* Essa etapa, em uma modelagem de banco de dados, consiste em criar um modelo um pouco mais abstrato. Focando em capturar as entidades, seus atributos e os relacionamentos entre elas, sem se preocupar com os detalhes da implementação. 

<br>

![Modelo_Conceitual](imagens/modelo_conceitual_img.jpg)

<br><br>

<span id="modelo-logico"></span>

## 3. ⌨️ Modelo Lógico

* Nesta etapa, em uma modelagem de banco de dados, iniciamos a inserção dos detalhes de implementação. Definimos as tabelas com suas respectivas chaves primárias, estrangeiras e todas as restrições de integridade.  

<br>

![Modelo_Logico](imagens/modelo_logico_img.jpg)

<br><br>

<span id="modelo-fisico"></span>

## 4. 💪 Modelo Físico

* Nesta etapa, em uma modelagem de banco de dados, temos uma implementação concreta no ambiente de banco de dados.

<br>

![Modelo_Fisico](imagens/modelo_fisico_img.jpg)

<br>
<span id="tecnologias"></span>

## 5. 🛠 Tecnologias e Ferramentas Utilizadas

- [SQL](https://learn.microsoft.com/pt-br/sql/?view=sql-server-ver16)
- [PostgreSQL](https://www.postgresql.org/docs/)
- [BR Modelo](https://www.brmodeloweb.com/lang/pt-br/index.html)
- [SQL Power Architect](https://dbmstools.com/tools/sql-power-architect)

<br>
<span id="pessoas-autoras"></span>

## 6. 👩🏽‍💻Pessoas Autoras:

<img style='width:130px'  src='https://avatars.githubusercontent.com/u/114631584?v=4' alt='pessoa desenvolvedora'>

<h4>Flávia Santos</h4>

Linkedin: https://www.linkedin.com/in/flavia-santos-dev/
