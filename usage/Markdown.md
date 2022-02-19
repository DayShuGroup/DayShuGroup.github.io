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





