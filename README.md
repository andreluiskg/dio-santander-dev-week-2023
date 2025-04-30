# Santander Dev Week 2023
Java RESTful API criada para a Santander Dev Week 2023

## Diagrama de Classes

```mermaid
classDiagram
  class User {
    .String name
    .Account acount
    .Feature[] features
    .Card card
    .News[] news
  }

  class Account {
    .String number
    .String agency
    .Number balance
    .Number limit
  }

  class Feature {
    .String icon
    .String description
  }

  class Card {
    .String number
    .number limit
  }

  class News {
    .String icon
    .String description
  }

<<<<<<< HEAD
  User "1" *-- "1" Account
  User "1" *-- "N" Feature
  User "1" *-- "1" Card
  User "1" *-- "N" News
=======
  User --> Account
  User --> Feature
  User --> Card
  User --> News
>>>>>>> dffa6a6f3792539b241efc9255235c1888c6e5dc
```