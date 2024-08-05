
- Работодатель
- Работник
- Супервайзер
- Внешний табель
- Рабочий день






```mermaid
---
title: Вшешний табель
---

erDiagram

    EMPLOYER 1 to 0+ WORKER : "hire"
    EMPLOYER 1 to 0+ SUPERVISOR : "hire"

    WORKER 1 to 0+ WORKDAY : "has"

    SUPERVISED_GROUP 1 to 0+ WORKER : "contains"

    SUPERVISOR 1 to 0+ SUPERVISED_GROUP : "controls"
    SUPERVISOR 1 .. 0+ WORKDAY : "edit"

    WORKDAY {
        uuid Worker
        date Date
        bool status
        int workhours
        string comment
    }

    TabelFacade {
        API query()
    }

```


