# フローチャート(TD,BT,LR,RL)

フローチャートの方向

```
TB : top to bottom
TD : top-down/ same as top to bottom
BT : bottom to top
RL : right to left
LR : left to right
```

```mermaid
flowchart TB
    開始 --> 終了
```

```mermaid
flowchart TD
    開始 --> 終了
```

```mermaid
flowchart BT
    開始 --> 終了
```

```mermaid
flowchart RL
    開始 --> 終了
```

```mermaid
flowchart LR
    開始 --> 終了
```

---

```mermaid
flowchart TB

A[四角形] -->|文字| B(丸い四角)
B --> C{決定}
C -->|壱| D[結果 1]
C -->|弐| E[結果 2]
C -->|参| F[結果 3]
```
