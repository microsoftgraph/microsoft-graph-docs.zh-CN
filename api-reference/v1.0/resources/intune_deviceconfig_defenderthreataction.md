# <a name="defenderthreataction-enum-type"></a>defenderThreatAction 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

防护程序对其检测到恶意软件威胁所执行的默认操作。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|基于更新定义应用操作。|
|清理|1|清理检测到的威胁。|
|隔离|2|隔离检测到的威胁。|
|删除|3|删除检测到的威胁。|
|允许|4|允许检测到的威胁。|
|userDefined|5|检测到威胁时允许用户确定要采取的操作。|
|block － 阻止|6|阻止检测到的威胁。|








