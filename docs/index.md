# Template de Entrega

???+ info inline end "Edição"

    2025.1

## Ycaro Campovilla Mendes De Barros

- Sou **Cientista de Dados e Desenvolvedor Full Stack** com expertise em **UX/UI e Data Analytics**, apaixonado por tecnologia, automação e soluções que unem performance e experiência.  
- Minha formação em **Ciência de Dados e Negócios pela ESPM** me permite atuar tanto no lado analítico — interpretando informações e extraindo insights estratégicos — quanto no lado criativo e técnico, desenvolvendo aplicações funcionais e intuitivas.  
- Busco constantemente aprimorar minhas habilidades em **programação, análise estatística e design de interfaces**, conciliando dados e usabilidade para entregar soluções completas.  
- Acredito que o futuro pertence a quem consegue **transformar informação em inovação**.  

---

### 🛠️ Minhas Skills

- **Dados**: Python, SQL, Tableau, PrepBuilder, Looker, Google Analytics, TGI, Ibope Monitor, PySpark, RapidMiner  
- **Front-End**: HTML, CSS, JavaScript, UX/UI, Astah  
- **Back-End**: Python, SQL, Banco de Dados, automação e integração  
- **Certificações**: Google Analytics Certificate  

---

!!! tip "Instruções"

    Vocês devem utilizar este template como um bloco de notas para registrar o que foi feito e o que falta fazer.  
    O template deve ser editado e atualizado a cada entrega, registrando assim a data de entrega e o que foi feito até o momento via Git.

---

## Entregas

- [x] Roteiro 1 - Data 23/02/2025  
- [ ] Roteiro 2  
- [ ] Roteiro 3  
- [ ] Roteiro 4  
- [ ] Projeto  

---

## Diagramas

Use o [Mermaid](https://mermaid.js.org/intro/){:target='_blank'} para criar os diagramas de documentação.

[Mermaid Live Editor](https://mermaid.live/){:target='_blank'}

```mermaid
flowchart TD
    subgraph Cluster [Infraestrutura]
        Deployment:::orange -->|defines| ReplicaSet
        ReplicaSet -->|manages| pod((Pod))
        pod:::red -->|runs| Container
        Deployment -->|scales| pod
        Deployment -->|updates| pod
        Service:::orange -->|exposes| pod
    end

    subgraph Configuração
        ConfigMap:::orange
        Secret:::orange
    end

    ConfigMap --> Deployment
    Secret --> Deployment

    classDef red fill:#f55
    classDef orange fill:#ffa500
