
```mermaid
flowchart TD
    A1([Inicio])-->B1
    B1[tablero = ?]-->C1
    C1[fila = 0]-->D1
    D1{¿Quedan filas?}
    D1 -->|No| E1([Fin])
    D1 -->|Sí| F1[Recorrer fila]
    F1 --> G1[fila+1]-->D1
        
