tags: #article #software-architecture #monolith #mircoservice #distributed-system

# Untangling Microservices, or Balancing Complexity in Distributed Systems
## Article
https://vladikk.com/2020/04/09/untangling-microservices/

## Thoughts
When designing microservice you should not forget about that it will live inside of system complexity. Try to minimise service interface. Allowing access database directly hugely expands service interface.

## Quotes

> Often, teams fail to achieve business goals because of the exponentially growing — or even worse unpredictable — costs of making a change. In other words, the system is unable to keep up with the needs of the business.

> We Build Systems!
>We build systems, not sets of services. We use microservices-based architecture to optimize a system’s design, not the design of individual services. No matter what others may say, microservices cannot, and will never be neither completely decoupled, nor fully independent. **You cannot build a system out of independent components!** That would go against the very definition of the term “system”


Russian translation: https://habr.com/ru/post/590165/