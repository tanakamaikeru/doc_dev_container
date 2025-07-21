# サンプル

PlantUMLでの描画サンプルです

## アクティビティ図

```plantuml
@startuml
start
:サンプル;
if (分岐) then(no)
else(yes)
    !include ./sample2.md!sample
endif
end
@enduml
```

## シーケンス図

```plantuml
@startuml
!include ./sample2.md!sequence_header
t -> w: 表示してほしい
!include ./sample2.md!consider
w -> t: 表示してあげる
@enduml
```
