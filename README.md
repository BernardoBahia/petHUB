<p align="center">
  <img src="https://i.imgur.com/JXyyAti.png" alt="petHUB">
</p>

## Descrição

O petHUB é um gerenciador de petshop, pensado para facilitar o gerenciamento de vendas e de vacinas de um petshop.

Este projeto foi desenvolvido como parte da atividade avaliativa A3 da disciplina de Programação de Soluções Computacionais de Análise e Desenvolvimento de Sistemas da UNIFG/BA.

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white) ![NetBeans IDE](https://img.shields.io/badge/NetBeansIDE-1B6AC6.svg?style=for-the-badge&logo=apache-netbeans-ide&logoColor=white) ![Apache Maven](https://img.shields.io/badge/Apache%20Maven-C71A36?style=for-the-badge&logo=Apache%20Maven&logoColor=white)

## Integrantes

- Bernardo Almeida de Oliveira Bahia
- Daniel Fernandes Cardoso

## Funcionalidades

- Controle de clientes
- Controle de animais
- Controle de vacinas
- Controle de vendas
- Controle de produtos
- Controle de fornecedores
- Controle de Funcionário com nível de acesso
- Geração de Relatórios e pedido de venda
- Ficha Animal com todas as vacinas registradas

## Dependências

- [Apache Maven](https://maven.apache.org/download.cgi)
- [JDK 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- [json-20160810](https://repo1.maven.org/maven2/org/json/json/20160810/json-20160810.jar)
- [mysql-connector](https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31/mysql-connector-j-8.0.31.jar)
- [jBCrypt](https://repo1.maven.org/maven2/de/svenkubiak/jBCrypt/0.4/jBCrypt-0.4.jar)
- [JasperReports® Library](https://community.jaspersoft.com/download-jaspersoft/community-edition/)

## Pacotes Externos

- [ViaCEP](https://gitlab.com/parg/ViaCEP) - Biblioteca para consulta de CEPs através da API do ViaCEP (https://viacep.com.br/)

## Telas

<div align="center">

| Login | Dashboard |
| --- | --- |
| <img src="https://i.imgur.com/vHZlwML.png" width="410" height="200" /> | <img src="https://i.imgur.com/ZoDNkZd.png" width="410" height="200" /> |

| Cadastro Cliente | Cadastro Pet |
| --- | --- |
| <img src="https://i.imgur.com/g4d3ifI.png" width="410" height="200" /> | <img src="https://i.imgur.com/ztUzGoP.png" width="410" height="200" /> |

| Cadastro Funcionário | Cadastro Fornecedor |
| --- | --- |
| <img src="https://i.imgur.com/azLimIr.png" width="410" height="200" /> | <img src="https://i.imgur.com/lVr8fXu.png" width="410" height="200" /> |

| Cadastro Produto | Controle Estoque |
| --- | --- |
| <img src="https://i.imgur.com/d5iZf2i.png" width="410" height="200" /> | <img src="https://i.imgur.com/4PcNczU.png" width="410" height="200" /> |

| Agenda de Serviços| Cadastro de Serviços|
|----------------------------------------------------------------------|----------------------------------------------------------------------|
| <img src="https://i.imgur.com/tjYihKK.png" width="410" height="200" /> | <img src="https://i.imgur.com/c8xttFO.png" width="410" height="200" /> |

| Controle Vacinas | Tela Vendas |
| --- | --- |
| <img src="https://i.imgur.com/tdSff3N.png" width="410" height="200" /> | <img src="https://i.imgur.com/cRSas9n.png" width="410" height="200" /> |

| Total Vendas | Histórico Vendas |
| --- | --- |
| <img src="https://i.imgur.com/zUTUt8b.png" width="410" height="200" /> | <img src="https://i.imgur.com/9roCAxs.png" width="410" height="200" /> |

</div>

## Logins

### Administrador (Acesso Total ao Sistema)
- **Usuário:** admin@admin.com
- **Senha:** 123

### Vendedor
- **Acessos:** Cadastro de Clientes, Animais, Produtos e Serviços, Agenda de Serviços e Abrir PDV
- **Usuário:** vendedor@vendedor.com
- **Senha:** 123

### Veterinário
- **Acessos:** Cadastro de Clientes, Animais, Produtos e Serviços, Agenda de Serviços, Gerar Ficha Animal e Registro de Vacina
- **Usuário:** veterinario@veterinario.com
- **Senha:** 123

## Documentação

Toda a documentação em Javadoc pode ser acessada pelo link: [Documentação do petHUB](https://danielf-cardoso.github.io/petHUB/)

## Instalação

Antes de começar, verifique se você possui o Java 17/22 e o Apache Maven instalado em seu computador. Se não tiver, faça o download e a instalação a partir dos sites oficiais.

1. **Configuração do Banco de Dados**
    - Abra o arquivo `config.properties` dentro da pasta `resources`.
    - Edite o arquivo com as informações do seu banco de dados.

2. **Importação do Banco de Dados**
    - Importe o banco de dados disponível na raiz do projeto (petHUB.sql) para o seu servidor MySQL.

3. **Execução do Projeto**
    - No diretório raiz do projeto, execute os seguintes comandos do Maven para limpar e empacotar o projeto:
      ```sh
      mvn clean package
      ```
    - O comando acima irá gerar um arquivo `petHUB-1.0-SNAPSHOT.jar` na pasta `target`.

4. **Iniciando a Aplicação**
    - Execute o arquivo `petHUB-1.0-SNAPSHOT.jar` gerado, que já estará com todas as dependências necessárias:
      ```sh
      java -jar target/petHUB-1.0-SNAPSHOT.jar
      ```
