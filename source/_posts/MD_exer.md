Header One | Header Two
:--------- | :---------
Item One   | Item Two

[官网参考链接](http://knsv.github.io/mermaid/#flowcharts-basic-syntax)

```{mermaid}
graph BT
A --> B
id1[This is the text in the box]
id2[This is the text in the box]
id3(This is the text in the box)
id4((This is the text in the box))
```

```{mermaid}
graph LR
id1((this is a circle)) --> id2{this is a square}
A --- B
```

```{mermaid}
%% Example of sequence diagram
sequenceDiagram
    Alice->>John: Hello John, how are you?
    John-->>Alice: Great!
```

```{mermaid}s
graph TB
id1(start)--> id2{123}
id2 --> 122
```

```{mermaid}
graph LR
%% 前两个-后三个-
  subgraph first
  A-- This is the text --- B
  end
  subgraph second
  C-- 123 ---DD
  end
  subgraph third
  E -- 555 --> F
  end
  A-->E
```

```{mermaid}
graph LR
id1[Hard Edge] -- Link Test --> id2(round edge)  
id2 --> id3{Decision}
id3 --> id4[Result one]
id3 --> id5[Result two]
```

```{mermaid}
graph LR
id1[Square Rect] --> id2((Circle))
id2 --> id3{Rhombus}
id1 --> id4(Round Rect)
id4 --> id3
```
