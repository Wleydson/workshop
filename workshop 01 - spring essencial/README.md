# WorkShop Spring Essencial ![Java](http://img.shields.io/badge/-Java-007396?style=flat-square&logo=java&logoColor=ffffff) ![Spring](http://img.shields.io/badge/-Spring-6DB33F?style=flat-square&logo=spring&logoColor=ffffff)
<p>
  Nesse workshop será desenvolvido uma Rest Api de serviços, o objetivo é mostrar o básico sobre spring boot framework criando dois módulos de CRUD um de cliente e um de serviços.
</p>

## Aula 1
<p>
  Link para criação do projeto: https://start.spring.io/
</p>

### Configurações no pom.xml

    <dependency>
      <groupId>org.springframework.boot</groupId>
      <artifactId>spring-boot-starter-web</artifactId>
    </dependency>

    <dependency>
      <groupId>org.springframework.boot</groupId>
      <artifactId>spring-boot-starter-data-jpa</artifactId>
    </dependency>
    
    <dependency>
      <groupId>org.projectlombok</groupId>
      <artifactId>lombok</artifactId>
      <optional>true</optional>
    </dependency>

    <dependency>
      <groupId>com.h2database</groupId>
      <artifactId>h2</artifactId>
    </dependency>
   
   ### Configurações Banco H2

    spring.datasource.url=jdbc:h2:mem:db
    spring.datasource.driver-class-name=org.h2.Driver
    spring.datasource.username=sa
    spring.datasource.password=sa

    spring.jpa.database-platform=org.hibernate.dialect.H2Dialect

    spring.h2.console.enabled=true
    spring.h2.console.path=/h2-console
    
### Diagrama
link: https://lucid.app/lucidchart/invitations/accept/e91057a3-e361-4483-a9a8-71482d25ddef
![Image](https://github.com/Wleydson/workshop/blob/main/workshop%2001%20-%20spring%20essencial/diagrama_entidades.png "Diagrama das entidades")

### Lombok
<p>
  Link:https://projectlombok.org/ <br/>
  IntelliJ IDEA: Settings > Plugins > aba Installed > Lombok <br/>
  Lombok para eclipse: https://dicasdejava.com.br/como-configurar-o-lombok-no-eclipse/
</p>
<br/>
<p>
Lembre de pega o arquivo data.sql aqui no repositorio para ter massa de dados para iniciar a implementação,
o caminho para colocar o arquivo do data.sql:
          
       src/main/resources
</p>
<br/>

## Aula 2
Para conhecer mais sobre as anotações que contém no spring, segue um link para ajuda: https://www.javatpoint.com/spring-boot-annotations
<br/>
Anotações que iremos usar na camada de controller:
      
      @RestController
      @RequestMapping("path")
      @PostMapping
      @GetMapping
      @DeleteMapping
      @PutMapping
      @ResponseStatus(HttpStatus)
      @RequestBody
      @PathVariable
      
    
Link dos Http status code: https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Status
<br/>


## Aula 3
ModelMapper: http://modelmapper.org/
<br/>
Bean Validation: https://www.baeldung.com/spring-boot-bean-validation
<br/>

    <dependency>
      <groupId>org.springframework.boot</groupId>
      <artifactId>spring-boot-starter-validation</artifactId>
    </dependency>

    <dependency>
     <groupId>org.modelmapper</groupId>
      <artifactId>modelmapper</artifactId>
      <version>2.3.0</version>
    </dependency>
    
![Image](https://github.com/Wleydson/workshop/blob/main/workshop%2001%20-%20spring%20essencial/diagram_dtos.png "DTOs")

<br/>
Handler Exception: https://www.baeldung.com/exception-handling-for-rest-with-spring


## Aula 4
<p>
  Adicionando o Swagger na api
  
	<dependency>
	  <groupId>io.springfox</groupId>
	  <artifactId>springfox-swagger2</artifactId>
	  <version>2.6.1</version>
	</dependency>
	
	<dependency>
	  <groupId>io.springfox</groupId>
	  <artifactId>springfox-swagger-ui</artifactId>
	  <version>2.6.1</version>
	</dependency>
    
  Verificar o commit no projeto que foi criado para pega a configuração do swagger: 
  <br/>
  https://github.com/Wleydson/se-workshop/commit/2bd65190899d11a3288cf08edaaf94281a5218fc
</p>


## Extra
 <p>
  Bem agora que terminamos a ultima aula ta na hora da surpresinha<br/>
  Vamos lá de desafio hehehe<br/>
  <br/>
  O desafio baseia se em criar um nova entidade chama comentario e relacionar ele com a entidade já existente serviços, e lembrando de manter as boas praticas e criar os endpoints de serviços e comentários.
</p>

![Image](https://github.com/Wleydson/workshop/blob/main/workshop%2001%20-%20spring%20essencial/desafio.png "desafio")
