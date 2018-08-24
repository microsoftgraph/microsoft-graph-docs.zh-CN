# <a name="deviceenrollmentfailurereason-enum-type"></a>deviceEnrollmentFailureReason enum type

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

用于注册的顶级故障类别。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|未知|0|默认值，失败原因未知。|
|身份验证|1|身份验证失败|
|授权|2|呼叫已通过身份验证，但未被授权注册。|
|accountValidation|3|无法验证注册的帐户。 （帐户已被阻止，注册未启用）|
|userValidation|4|用户无法验证。 （用户不存在，缺少许可证）|
|deviceNotSupported|5|移动设备管理不支持设备。|
|inMaintenance|6|帐户在维护中。|
|badRequest|7|客户端发送服务无法理解/不支持的请求。|
|featureNotSupported|8|此帐户不支持此注册使用的功能。|
|enrollmentRestrictionsEnforced|9|管理员配置的注册限制阻止了此注册。|
|clientDisconnected|10|客户端超时或注册已由最终用户中止。|



