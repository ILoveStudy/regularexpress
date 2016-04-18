### regularexpress

#1.惰性匹配

```
.*?

```

# 2.环视否定

```
var reg = ^(\d)\1(?:(?!\1)\d)$/

```

### 这个例子中,表示:三位数字,最后侧不能出现前两位的数字


(?<=Expression) 逆序肯定环视，表示所在位置左侧能够匹配Expression

(?<!Expression) 逆序否定环视，表示所在位置左侧不能匹配Expression

(?=Expression) 顺序肯定环视，表示所在位置右侧能够匹配Expression

(?!Expression) 顺序否定环视，表示所在位置右侧不能匹配Expression

