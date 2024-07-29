# Santander Dev Week 2024
Java RESTful API criado para o Santander Dev Week.

## Diagrama de Classes

  ```mermaid
classDiagram
    class User {
        +String name
        +Account account
        +List<Feature> features
        +Card card
        +List<News> news
    }

    class Account {
        +String number
        +String agency
        +Float balancy
        +Float limit
    }

    class Feature {
        +String icon
        +String description
    }

    class Card {
        +String number
        +Float limit
    }

    class News {
        +String icon
        +String description
    }

    User "1" -- "1" Account : contains
    User "1" -- "*" Feature : has
    User "1" -- "1" Card : has
    User "1" -- "*" News : has
```
