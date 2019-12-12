
##最佳实践：
###分组
 当一个接口有多种实现时，可以用 group 区分。
 给不同业务方提供的接口，可以用不同group

###参数校验
* 
在客户端验证参数（通过注解）
<dubbo:reference id="validationService" interface="org.apache.dubbo.examples.validation.api.ValidationService" validation="true" />

在服务器端验证参数
<dubbo:service interface="org.apache.dubbo.examples.validation.api.ValidationService" ref="validationService" validation="true" />




