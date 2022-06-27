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

ぐるぐる回る

```mermaid
flowchart LR
開始 --> 中間
中間 --> 終了
終了 --> 開始
```

```mermaid
flowchart LR
1 --> 2
2 --> 3
3 --> 4
4 --> 1
```

```mermaid
flowchart LR
1 --> 2
2 --> 3
3 --> 4
4 --> 2
2 --> 1
```

---

サブグラフ

```mermaid
flowchart TB
    c1-->a2
    subgraph グラフ1
    a1-->a2
    end
    subgraph グラフ2
    b1-->b2
    end
    subgraph グラフ3
    c1-->c2
    end
    グラフ1 --> グラフ2
    グラフ3 --> グラフ2
    グラフ2 --> c2
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

---

style を適用

```mermaid
flowchart LR
    id1(Start)-->id2(Stop)
    style id1 fill:#f9f,stroke:#333,stroke-width:4px
    style id2 fill:#bbf,stroke:#f66,stroke-width:2px,color:#fff,stroke-dasharray: 5 5
```

---

色々な線

```mermaid
flowchart LR
A == 太線 === B
A -. 点線 -.- C
A == 太い矢印 ==> D
A -. 点線矢印 .-> E
A -- 丸矢印 --o F
A -- x矢印 --x G
H <-->|双方向矢印| I
H x--x|双方向矢印| J
H o--o|双方向矢印| K
```
