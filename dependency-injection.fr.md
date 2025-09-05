# Injection de dépendance
## scope
 - ce principe concerne les services (c'est-à-dire les objets définissant des comportements), lorsqu'un client A utilise un service B 
```mermaid
flowchart LR
    A[client A] -- utilise --> B[service B]
```
## principe
 - le client A ne doit pas importer directement l'implémentation du service B
```mermaid
classDiagram
    B <-- ImplementationB
    A o-- B
namespace client {
    class B {<<Interface>>}
    class A
}
```
