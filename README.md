# Config_JAVA_WEB

## JSTL 
```
<dependency>
    <groupId>jakarta.servlet.jsp.jstl</groupId>
    <artifactId>jakarta.servlet.jsp.jstl-api</artifactId>
    <version>3.0.0</version>
</dependency>
<dependency>
    <groupId>org.glassfish.web</groupId>
    <artifactId>jakarta.servlet.jsp.jstl</artifactId>
    <version>3.0.1</version>
</dependency>
```
- Khái niệm
    - jakarta.servlet.jsp.jstl-api (JSTL API):
      
    Là API (Application Programming Interface) của JSTL.
  <br>
    Cung cấp các giao diện và lớp trừu tượng cho phát triển các thư viện thực thi JSTL.
    <b>Không chứa mã thực thi, chỉ chứa khai báo và giao diện.</b>
    Giúp đảm bảo tính đồng nhất và tương thích giữa các thư viện thực thi JSTL khác nhau.

    - jakarta.servlet.jsp.jstl (JSTL Runtime Library):

    Là thư viện thực thi của JSTL.
  <br>
    <b>Chứa mã nguồn thực thi cho các tag JSTL cụ thể.</b>
    Thêm vào classpath của ứng dụng web để thực thi các tag JSTL trong mã JSP.
    Cung cấp các thư viện để xử lý điều kiện, lặp, định dạng ngày tháng, và nhiều chức năng khác.
    Tách biệt mã logic từ giao diện người dùng trong trang JSP.
    Giúp làm cho mã nguồn trở nên dễ đọc và dễ bảo trì hơn.

- Công dụng
  - Core - JSTL 
    ```
    <%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core" %>
    ```
  - Form - JSTL 
    ``` 
    <%@ taglib prefix="form" uri="http://www.springframework.org/tags/form" %>
    ```

## Config jsp 
```
spring.mvc.view.prefix: /WEB-INF/view/
spring.mvc.view.suffix: .jsp
```
## Hibernate

```
<dependency>
    <groupId>org.hibernate</groupId>
    <artifactId>hibernate-core-jakarta</artifactId>
    <version>5.6.10.Final</version>
</dependency>
```
## Nhúng Tomcat 
```
<dependency>
    <groupId>org.apache.tomcat.embed</groupId>
    <artifactId>tomcat-embed-jasper</artifactId>
</dependency>
```

## Lombox
```
<dependency>
    <groupId>org.projectlombok</groupId>
    <artifactId>lombok</artifactId>
    <version>1.18.30</version>
    <scope>provided</scope>
</dependency>
```

## Commons-lang3
```
<!-- https://mvnrepository.com/artifact/org.apache.commons/commons-lang3 -->
<dependency>
    <groupId>org.apache.commons</groupId>
    <artifactId>commons-lang3</artifactId>
    <version>3.14.0</version>
</dependency>
```
- cung cấp rất nhiều phương thức hỗ trợ các lớp Java Core, bao gồm các phương thức để xử lý: strings, numbers, dates, concurrency, reflection, … 

## MSSQL JDBC
``` 
<dependency>
    <groupId>com.microsoft.sqlserver</groupId>
    <artifactId>mssql-jdbc</artifactId>
    <version>9.4.1.jre16</version>
</dependency>
```

## MySQL
``` 
<dependency>
    <groupId>mysql</groupId>
    <artifactId>mysql-connector-java</artifactId>
    <version>8.0.31</version>
</dependency>
```

## JPA 
```
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-jpa</artifactId>
</dependency>
```

## Spring Validator 
``` 
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-validation</artifactId>
</dependency>
```


