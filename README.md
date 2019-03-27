# Spring-MultiRequestBody
## 项目主要功能
为Spring多@RequestBody支持，来解决Controller中POST方式JSON格式请求时
1. 无法直接用@RequestBody解析基本类型包装类的问题。
2. 无法使用@RequestBody接收多个实体的问题。
3.提供从方法上提供自定义注解、从参数上提供自定义注解解决 @RequestBody 需要后台用bean 接受参数 限制

## 项目优势
1. 支持通过注解的value指定JSON的key来解析对象。
2. 支持通过注解无value，直接根据参数名来解析对象
3. 支持基本类型的注入
4. 支持GET和其他请求方式注入
5. 支持通过注解无value且参数名不匹配JSON串key时，根据属性解析对象。
6. 支持多余属性(不解析、不报错)、支持参数“共用”（不指定value时，参数名不为JSON串的key）
7. 支持当value和属性名找不到匹配的key时，对象是否匹配所有属性。

## 重要更新记录
- 2019年02月25日 新增xml方式参考配置

- 2019年02月07日  fix 当list参数为空时，parameterType.newInstance会导致异常

- 2018年12月28日  新增测试用例，完善解析部分代码

- 2018年10月23日  完善项目格式

- 2018年08月28日  创建第一版

## 参考资料
* 对应博文： [明明如月小角落CSDN](https://blog.csdn.net/w605283073/article/details/82119284)
* 其他参考：[StackOverFlow讨论](https://stackoverflow.com/questions/12893566/passing-multiple-variables-in-requestbody-to-a-spring-mvc-controller-using-ajax)


