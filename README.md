# OK
- 1
- 2
- 3 

```mermaid
sequenceDiagram
    participant A
    participant B
    participant C

    A->>B : Hello
    B-->>A : Bye
    
```


```mermaid
stateDiagram
    [*] --> A
    A --> B
    A --> C
    C --> A
    B --> [*]
```


```mermaid
---
title: Order example
---
erDiagram

    ORDER 1 .. 1 ITEM : ok

    CUSTOMER {
        string FIO
        USER account

    }

    ORDER 0+ to 1+ FOOBAR : kk

```



```mermaid
mindmap
    PayPeople
        Ежедневные платежи
            Учет
            Заявка
            Подтверждение
            Проведение платежа
            Ограничения на выплаты

        Юридические лица
            Управление
                Сотрудниками
                Выплатами
```