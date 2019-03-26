# TaskHub
![v1.0](https://img.shields.io/badge/version-1.0-green.svg) ![task](https://img.shields.io/badge/type-task-yellow.svg) ![v1.0](https://img.shields.io/badge/state-done-blue.svg) ![task](https://img.shields.io/badge/type-task-yellow.svg)
## 分组学习 1 

- [ ] 学习DOM虚拟方法 `MUST` `Done` `2019-1-1 20:28` `Task`
---
#### Vue 虚拟DOM方法

说的发生地方
   
   
   
- [ ] 学习DOM虚拟方法, 很长的一行阿萨德发生的发送到发送到发送到发送到发送到发送到发送到发送到发送到费阿萨德发生的发生地方 `MUST` `Done` `2019-1-1 20:28` ` 2019-2-1 10:28` `BUG`




## 分组学习 2

- [ ] 学习DOM虚拟方法 `MUST` `Done` `2019-1-1 20:28` `Task`
```markdown

## Vue 虚拟DOM方法
说的发生地方
```


- [ ] 学习DOM虚拟方法, 很长的一行阿萨德发生的发送到发送到发送到发送到发送到发送到发送到发送到发送到费阿萨德发生的发生地方 `MUST` `Done` `2019-1-1 20:28` ` 2019-2-1 10:28` `BUG`





[TaskHub] 

* 创建电子流程
```json
{
    props: {
        amount: {
            name: '报销金额',
            type: Number,
            default: 100,
        },
        description: {
            name: '报销类别',
            type: String,
            deafult: '采购'
        },
        pictures: {
            name: '电子发票',
            type: File,
            require: false,
        }
    },
}
```
* 主管审批
* 会计核算
* 银行转账



|              |  1   |  2   |  3   |  4   |
| ------------ | :--: | :--: | :--: | :--: |
| 创建电子流程 |      |  1   |      |      |
| 主管审批     |      |      |  1   |      |
| 会计核算     |      |      |      |  1   |
| 银行转账     |      |      |      |      |



#### 表单 (默认require = true)

```json
{
    props: {
        amount: {
            name: '报销金额',
            type: Number,
            default: 100,
        },
        description: {
            name: '报销类别',
            type: String,
            deafult: '采购'
        },
        pictures: {
            name: '电子发票',
            type: File,
            require: false,
        }
    },
    
    calculated: {
        totalAmount: {
            name: '总额',
            type: Number,
        },
    },
    
    replay: {
        comment: {
            name: '意见',
            type: String,
        },
        
    },
    
    
}



```



## 报销

| 属性     | 值                                 |
| -------- | ---------------------------------- |
| 报销金额 | 100                                |
| 报销类别 | 采购电脑配件                       |
| 电子发票 | https://www.taskhub.work/file/xxxx |
| 报销人   | z0001                          |



## 审批历史

| 时间           | 审批人 | 意见     |
| -------------- | ------ | -------- |
| 2019-1-1 11:02 | c0000  | 同意报销 |
| 2019-1-1 11:04 | z0000  | 同意     |
|                |        |          |
|                |        |          |





