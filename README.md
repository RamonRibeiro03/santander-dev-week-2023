# Santander-Dev-Week 2023
Java RESTfull API criada para a Santander Dev Week

## Diagrama de Classes

```mermaid
classDiagram
    class User {
        -String name
        -Account account
        -Feature[] features
        -Card card
        -News news
    }

    class Account {
       -String number
        -String agency
        -Number balance
        -Number limit
    }

    class Feature {
       -String icon
        -String description
    }

    class Card {
        -String number
        -Number limit
    }

    class News {
        -String icon
        -String description
    }

    User "1" *-- "1" Account 
    User "1" *-- "1..N" Feature 
    User "1" *-- "1" Card 
    User "1" *-- "1..N" News 

```
## Teconoligas utilizadas : 

APIRESTFUL;
Banco de Dados PostegreSQL e banco em memória H2
DEPLOY da API na Nubem (Railway);


