# <a name="defenderthreataction-enum-type"></a>defenderThreatAction 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Defender 的默认操作以对其执行检测到恶意软件的威胁。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|应用基于更新定义的操作。|
|clean|1|清理检测到的威胁。|
|隔离|2|隔离检测到的威胁。|
|删除|3|删除检测到的威胁。|
|允许|4|允许检测到的威胁。|
|用户定制|5|允许用户以确定要使用的检测威胁采取的操作。|
|阻止|6|阻止检测到的威胁。|



