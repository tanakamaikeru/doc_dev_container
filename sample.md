# サンプル

PlantUMLでの描画サンプルです

## サンプル図1

```plantuml
@startuml
start
:サンプル;
if (分岐) then(no)
else(yes)
    !include ./sample2.md!sample2_1
endif
end
@enduml
```

## サンプル図2

```plantuml
@startuml
!include ./sample2.md!sequence_header
t -> w: 表示してほしい
!include ./sample2.md!consider
w -> t: 表示してあげる
@enduml
```

- [サンプル](#サンプル)
  - [サンプル図1](#サンプル図1)
  - [サンプル図2](#サンプル図2)
