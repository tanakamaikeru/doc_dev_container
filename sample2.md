# サンプル2

## アクティビティ図

```plantuml
@startuml (id=sample)
:別ファイルに定義;
note right
    別で定義した図をinclude出来ます
endnote
@enduml
```

## シーケンス図

シーケンス図のヘッダ部分の共通化も出来ます

```plantuml
@startuml (id=sequence_header)
hidefootbox
actor tanaka as t
participant web as w
@enduml
```

共通ヘッダを用いて記述が出来ます

```plantuml
@startuml (id=consider)
!include sample2.md!sequence_header
group
w -> w: 悩む
note right
    別ファイルに色々定義できます
endnote
end
@enduml
```