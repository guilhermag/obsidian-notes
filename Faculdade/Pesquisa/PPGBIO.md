```mermaid
graph 
    A(Inicio) --> B{Paciente possui <br>exames prévios ?}
    B --> |Sim| C[Entrar com os dados do exame]
    B --> |Não| B1(Coletar exames)
    B1 --> C
    C --> D{Taxa <= 30 ml/min/1,73m2}
    D --> |Sim| E(Risco Alto - <br> Encaminhar Nefro)
    D --> |Não| F{Taxa > 30 e < 60 ml/min/1,73m2}
```


