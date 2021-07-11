### cmake 变量
```makefile

# 变量声明
set(hello1 "hello1")
message("变量 hello1=" ${hello1})

set(hello2 hello2)
message("变量 hello2=" ${hello2})
# hello2和hello1效果相同
#---------------------------------

# 变量复制
set(helloCopy ${hello2})
message("变量 helloCopy=" ${helloCopy})
#---------------------------------

# 类似数组遍历
set(a "1")
set(b "2")
set(c "3")
set(arr a b c)
message("变量 arr=" ${arr}) #a,b,c
foreach(item ${arr})
  # 取变量里的内容
  message("变量 ${item}:" ${${item}})
endforeach()
#---------------------------------

```
