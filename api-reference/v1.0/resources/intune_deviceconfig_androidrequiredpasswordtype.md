# <a name="androidrequiredpasswordtype-enum-type"></a>androidRequiredPasswordType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Android 所需的密码类型。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认值，没有用途。|
|alphabetic|1|必需是字母密码。|
|alphanumeric|2|必须是字母数字密码。|
|alphanumericWithSymbols|3|必需是带符号的字母数字密码。|
|lowSecurityBiometric|4| 需要低安全性的基于生物的密码。|
|numeric|5|必需数字密码。|
|numericComplex|6|必需是复杂的数字密码。|
|any|7|Password 或模式是必需的且可接受任何形式。|



