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


## Aula 2
Link dos Http status code: https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Status

## Aula 3
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


## Aula 4
 <p>
  Bem agora que terminamos a ultima aula ta na hora da surpresinha<br/>
  Vamos lá de desafio hehehe<br/>
  <br/>
  O desafio baseia se em criar um nova entidade chama comentario e relacionar ele com a entidade já existente serviços, e lembrando de manter as boas praticas.
</p>

![Image](https://github.com/Wleydson/workshop/blob/main/workshop%2001%20-%20spring%20essencial/desafio.png "desafio")
