
```mermaid
flowchart TD
    A1([Inicio])-->B1
    B1[tablero = ?]-->C1
    C1[fila = 0]-->D1
    D1{¿Quedan filas?}
    D1 -->|No| E1([Fin])
    D1 -->|Sí| F1[Recorrer fila]
    F1 --> G1[fila+1]-->D1
        
    A2[fila = ?]-->B"
    B2[col = 0]-->C2
    C2{¿Quedan columnas?}
    C2 -->|Sí|D2[quedanvio]
    D2 --> E2[col++]
    E2 --> C2
    C2 -->|No| F2([Fin])
   
    A3[celda]
    B3{¿0?}
    C3[Agua]
    D3{¿1?}
    E3[Correción]
    F3{¿2?}
    G3[“Posiciones”]
    H3[Submarino]
    I3([Fin])
    A3 --> B3
    B3 -->|Sí| C3 --> H3 --> I3
    B3 -->|No| D3
    D3 -->|Sí| E3 --> H3
    D3 -->|No| F3
    F3 -->|Sí| G3 --> H3
    F3 -->|No| H3
    H3 --> I3  