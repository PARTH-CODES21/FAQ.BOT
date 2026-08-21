# FAQ.BOT

import java.util.Scanner;

public class FAQBot {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("===== FAQ Bot =====");
        System.out.println("Ask me a question about Java or Spring Boot.");
        System.out.println("Type 'exit' to quit.\n");

        while (true) {
            System.out.print("You: ");
            String question = sc.nextLine();

            if (question.equalsIgnoreCase("exit")) {
                System.out.println("Bot: Goodbye!");
                break;
            }

            String answer = getAnswer(question);
            System.out.println("Bot: " + answer);
        }
        sc.close();
    }

    static String getAnswer(String question) {

        String q = question.toLowerCase();

        if (q.contains("what is java")) {
            return "Java is a popular, object-oriented programming language used to build "
                    + "everything from mobile apps to large backend systems.";
        }
        else if (q.contains("what is oop")) {
            return "OOP stands for Object-Oriented Programming. It is a programming approach "
                    + "based on objects and classes.";
        }
        else if (q.contains("what is a class")) {
            return "A class is a blueprint for creating objects. It defines the data and "
                    + "behavior that its objects will have.";
        }
        else if (q.contains("what is an object")) {
            return "An object is an instance of a class. It contains data and can perform "
                    + "actions defined by its class.";
        }
        else if (q.contains("what is inheritance")) {
            return "Inheritance allows one class to acquire the properties and methods of "
                    + "another class.";
        }
        else if (q.contains("what is polymorphism")) {
            return "Polymorphism means one interface can be used for different forms of "
                    + "objects, allowing the same method to behave differently.";
        }
        else if (q.contains("what is encapsulation")) {
            return "Encapsulation means bundling data and methods together and controlling "
                    + "direct access to the data.";
        } 
        else if (q.contains("what is abstraction")) {
            return "Abstraction means hiding unnecessary implementation details and showing "
                    + "only the important features to the user.";
        }
        else if (q.contains("what is jvm")) {
            return "JVM stands for Java Virtual Machine. It runs Java bytecode and allows Java "
                    + "programs to run on different operating systems.";
        }
        else if (q.contains("what is jdk")) {
            return "JDK stands for Java Development Kit. It contains the tools needed to "
                    + "develop, compile, and run Java programs.";
        } 
        else if (q.contains("what is jre")) {
            return "JRE stands for Java Runtime Environment. It provides the environment "
                    + "needed to run Java applications.";
        }
        else if (q.contains("jdk vs jre")) {
            return "JDK is used to develop Java applications, while JRE is mainly used to "
                    + "run Java applications.";
        }
        else if (q.contains("jvm vs jdk")) {
            return "JVM runs Java bytecode, while JDK provides development tools and includes "
                    + "the components needed to run Java programs.";
        }
        else if (q.contains("what is constructor")) {
            return "A constructor is a special method used to initialize an object when it "
                    + "is created.";
        }
        else if (q.contains("what is method overloading")) {
            return "Method overloading means having multiple methods with the same name but "
                    + "different parameters.";
        }
        else if (q.contains("what is method overriding")) {
            return "Method overriding happens when a child class provides its own implementation "
                    + "of a method defined in its parent class.";
        }
        else if (q.contains("what is exception handling")) {
            return "Exception handling is a way to handle runtime errors using mechanisms such "
                    + "as try, catch, and finally.";
        }
        else if (q.contains("what is array")) {
            return "An array is a collection of elements of the same type stored under one "
                    + "variable name.";
        }
        else if (q.contains("what is string")) {
            return "A String in Java is an object used to represent a sequence of characters.";
        }
        else if (q.contains("what is spring boot")) {
            return "Spring Boot is a Java framework that makes it easy to build applications "
                    + "quickly, without a lot of manual setup.";
        }
        else if (q.contains("why use spring boot")) {
            return "Spring Boot simplifies Java application development by providing automatic "
                    + "configuration, starter dependencies, and embedded servers.";
        }
        else if (q.contains("what is spring")) {
            return "Spring is a Java framework used to build scalable applications and provides "
                    + "features such as dependency injection and application configuration.";
        } else if (q.contains("what is dependency injection")) {
            return "Dependency Injection means Spring automatically creates and provides the "
                    + "objects a class needs, instead of the class creating them itself.";
        }
        else if (q.contains("what is ioc")) {
            return "IoC stands for Inversion of Control. It means the responsibility of creating "
                    + "and managing objects is given to the Spring framework.";
        }
        else if (q.contains("what is bean")) {
            return "A Spring Bean is an object that is created, configured, and managed by "
                    + "the Spring container.";
        }
        else if (q.contains("what is spring container")) {
            return "The Spring container is responsible for creating, configuring, and managing "
                    + "Spring Beans and their dependencies.";
        }
        else if (q.contains("what is autowired")) {
            return "@Autowired tells Spring to automatically inject a required dependency into "
                    + "a class.";
        }
        else if (q.contains("what is component")) {
            return "@Component tells Spring that a class should be detected and managed as "
                    + "a Spring Bean.";
        } else if (q.contains("what is service")) {
            return "@Service is a Spring annotation commonly used to mark a class that contains "
                    + "business logic.";
        } else if (q.contains("what is repository")) {
            return "@Repository is used for classes that handle database-related operations.";
        } else if (q.contains("what is controller")) {
            return "@Controller is used in Spring MVC to handle web requests and return responses "
                    + "or views.";
        } else if (q.contains("what is restcontroller")) {
            return "@RestController is used to create REST APIs where methods typically return "
                    + "data directly as HTTP responses.";
        } else if (q.contains("what is rest api") || q.contains("what is api")) {
            return "A REST API is a way for two programs to communicate over the internet "
                    + "using HTTP requests and responses.";
        } else if (q.contains("what is http")) {
            return "HTTP is a protocol used for communication between clients and servers over "
                    + "the web.";
        } else if (q.contains("what is get request")) {
            return "A GET request is used to retrieve data from a server.";
        } else if (q.contains("what is post request")) {
            return "A POST request is commonly used to send new data to a server.";
        } else if (q.contains("what is put request")) {
            return "A PUT request is commonly used to update an existing resource.";
        } else if (q.contains("what is delete request")) {
            return "A DELETE request is used to remove a resource from a server.";
        } else if (q.contains("what is json")) {
            return "JSON stands for JavaScript Object Notation. It is a lightweight format "
                    + "commonly used to exchange data between applications.";
        } 
        else if (q.contains("what is database")) {
            return "A database is a system used to store, organize, and retrieve data efficiently.";
        }
        else if (q.contains("what is mysql")) {
            return "MySQL is a popular relational database management system that stores data "
                    + "in tables using SQL.";
        }
        else if (q.contains("what is sql")) {
            return "SQL stands for Structured Query Language. It is used to create, read, update, "
                    + "and delete data in relational databases.";
        } 
        
    else if (q.contains("what is crud")) {
            return "CRUD stands for Create, Read, Update, and Delete, the four basic operations "
                    + "commonly performed on stored data.";
        } 
        else if (q.contains("what is maven")) {
            return "Maven is a build and dependency management tool commonly used in Java projects.";
        }
        
        else if (q.contains("what is gradle")) {
            return "Gradle is a build automation tool used to compile code, manage dependencies, "
                    + "and build Java applications.";
        }
        else if (q.contains("what is localhost")) {
            return "Localhost refers to your own computer. It is commonly used when testing "
                    + "applications locally.";
        }
        else if (q.contains("what is port")) {
            return "A port is a logical endpoint used by applications to communicate over a network. "
                    + "For example, Spring Boot commonly runs on port 8080.";
        }
        else if (q.contains("hello") || q.contains("hi")) {
            return "Hello! Ask me about Java, Spring Boot, REST APIs, databases, or OOP.";
        }
        else {
            return "Sorry, I don't have an answer for that yet. Try asking about Java, OOP, "
                    + "Spring Boot, REST APIs, databases, or SQL.";
        }
    }
    }
