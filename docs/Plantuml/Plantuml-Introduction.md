# Plantuml Introduction

## 什么是 PlantUML

首先，引用一段官网的说法

> PlantUML 是一个开源项目，支持快速绘制：
>
> - 时序图
> - 用例图
> - 类图
> - 活动图 (旧版语法在此处)
> - 组件图
> - 状态图
> - 对象图
> - 部署图
> - 定时图
>
> 同时还支持以下非 UML 图:
>
> - 线框图形界面
> - 架构图
> - 规范和描述语言 (SDL)
> - Ditaa diagram
> - 甘特图
> - 思维导图
> - Work Breakdown Structure diagram
> - 以 AsciiMath 或 JLaTeXMath 符号的数学公式
> - Entity Relationship diagram
>
> 通过简单直观的语言来定义这些示意图。

简单的说，PlantUML 定位是用一种比较易读的文字标记来描述各种常用的“图”。

一些例子如下：

简单的时序图

```plantuml
@startuml
Alice -> Bob: Authentication Request
Bob --> Alice: Authentication Response

Alice -> Bob: Another authentication Request
Alice <-- Bob: another authentication Response
@enduml
```

简单的用例图

```plantuml
@startuml
:Main Admin: as Admin
(Use the application) as (Use)

User -> (Start)
User --> (Use)

Admin ---> (Use)

note right of Admin : This is an example.

note right of (Use)
  A note can also
  be on several lines
end note

note "This note is connected\nto several objects." as N2
(Start) .. N2
N2 .. (Use)
@enduml
```

简单的类图

```plantuml
@startuml

class BaseClass

namespace net.dummy #DDDDDD {
	.BaseClass <|-- Person
	Meeting o-- Person

	.BaseClass <|- Meeting
}

namespace net.foo {
  net.dummy.Person  <|- Person
  .BaseClass <|-- Person

  net.dummy.Meeting o-- Person
}

BaseClass <|-- net.unused.Person

@enduml
```

简单的流程图

```plantuml
@startuml
:Ready;
:next(o)|
:Receiving;
split
 :nak(i)<
 :ack(o)>
split again
 :ack(i)<
 :next(o)
 on several line|
 :i := i + 1]
 :ack(o)>
split again
 :err(i)<
 :nak(o)>
split again
 :foo/
split again
 :i > 5}
stop
end split
:finish;
@enduml
```

具体各种图的例子可以参考其官网
plantuml.com
