# SequenceDiagram

```mermaid
sequenceDiagram
    店員->>+管理画面: 在庫確認
    管理画面->>+倉庫: 在庫検索
    倉庫->>+商品リスト: 商品検索
    商品リスト-->>-倉庫: 商品一覧
    倉庫 -->>-管理画面: 在庫一覧
    管理画面-->>-店員: 在庫結果確認
```

## Actor

```mermaid
sequenceDiagram
    actor ロイド
    actor ヨル
    actor アーニャ
    ロイド->ヨル:偽装家族
    ヨル->アーニャ: 偽装家族
```

```mermaid
sequenceDiagram
    participant ジョン
    Note right of ジョン: 年齢18歳
```

```mermaid
sequenceDiagram
    participant ジョン
    Note over ジョン: 年齢18歳
```

```mermaid
sequenceDiagram
    ジョン --> ジョージ: 同級生
    Note over ジョン,ジョージ: 年齢18歳
```
