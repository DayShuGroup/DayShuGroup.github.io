### 画流程图

```flow
st=>start: 开始
ed=>end: 结束
inputAccount=>inputoutput: 输入账号信息
checkData=>condition: 校验数据
compareData=>condition: 比较密码

st->inputAccount->checkData
checkData(yes)->compareData
checkData(no,right)->inputAccount
compareData(yes)->ed
compareData(no)->inputAccount
```





1. Typora 编辑器列表正确使用

   先`1. `创建第一列表项，然后回车创建下一个列表项，留一个列表项，编辑某项内容时，现在列表项<kbd>Enter</kbd>，然后<kbd>Backspace</kbd>

2. 
