Exemplos de código em JSF

# Iniciando um projeto

## Archetype
Execute o comando abaixo para criar um projeto web:

	mvn archetype:generate -DgroupId={project-packaging} -DartifactId={project-name} -DarchetypeArtifactId=maven-archetype-webapp -DinteractiveMode=false

## Dependências
[Dependência do Mojarra JSF](https://javaserverfaces.java.net/download.html)

[Dependência do PrimeFaces](http://primefaces.org/downloads)

## Jetty Plugin

[Tutorial Getting Start](http://www.eclipse.org/jetty/documentation/current/jetty-maven-plugin.html)

Você pode encontrar como adicionar o plugin do jetty neste [commit](https://github.com/wapmesquita/formacao-jsf/commit/ee8f9b09fccfcf85e08b00829d999dbce2720a0b)

Após adicionar o plugin, é necessário inserir as dependências de JSF para o plugin [commit](https://github.com/wapmesquita/formacao-jsf/commit/2464a102726ce53688ffcf4203eb5463cd14b66f)

# Primeira paǵina

* Configurando o projeto e criando minha primeira página - [Como fazer?](https://github.com/wapmesquita/formacao-jsf/commit/3b838da3eb0b0b5038b1215ca94f7f5bc1ffd67c)

* Criando meu primeiro ManageBean - [Como Fazer?](https://github.com/wapmesquita/formacao-jsf/commit/232d5f90af70aaa7c115ae10f927599c971273eb)

# Utilizando o [PrimeFaces](http://www.primefaces.org/)

Abixo você poderá encontrar como utilizar os componentes do PrimeFaces em seu projeto.

## Primeiro teste

Alterando o index.xhtml para utilizar um componente do PrimeFaces - [Como Fazer?](https://github.com/wapmesquita/formacao-jsf/commit/938211895761902dff7589187e3feb0771c7afd8)

## Alterando [tema](http://www.primefaces.org/themes) do PrimeFaces

Neste [exemplo](https://github.com/wapmesquita/formacao-jsf/commit/e455efc6c96843a9ffffbd42f39e60b366f0a77b) você pode ver como utilizar um tema do PrimeFaces.


# Manipulando páginas e ManageBeans

## Acessando uma classe

Você pode acessar os atributos de uma classe em um arquivo *.xhtml* da mesma forma que acessa um atributo do ManageBena. Neste [exemplo](https://github.com/wapmesquita/formacao-jsf/commit/e73dfb7d696ade6d3897c9b5c105f3cff83a0a0d) criamos a classe *Pessoa*, e acessamos o atributo *name* em nossos arquivo *.xhtml*

## Executando ações em botões

É possível executar determinado método em nosso ManageBean a partir do clique de um botão. Este método pode ser para navegação ou apenas para alguma ação.

### Navegação

Como mostrado neste [exemplo](https://github.com/wapmesquita/formacao-jsf/commit/6797d7fe3cfcc0f0815ab3410705f5f61a3ca467), para executar a navegação, basta retornar o caminho do arquivo desejado.

### Ação

Neste [exemplo](https://github.com/wapmesquita/formacao-jsf/commit/c559460f521c10813b633781165ce46516a742a0), utilizamos apenas a informação enviado do *index.xhtml* para o ManageBean e registramos no console.
