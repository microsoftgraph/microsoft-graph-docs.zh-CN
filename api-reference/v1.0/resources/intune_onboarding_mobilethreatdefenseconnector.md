# <a name="mobilethreatdefenseconnector-resource-type"></a>mobileThreatDefenseConnector 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

表示移动威胁防护合作伙伴连接的实体。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List mobileThreatDefenseConnectors](../api/intune_onboarding_mobilethreatdefenseconnector_list.md)|[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 集合|列出 [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 对象的属性和关系。|
|[Get mobileThreatDefenseConnector](../api/intune_onboarding_mobilethreatdefenseconnector_get.md)|[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)|读取 [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 对象的属性和关系。|
|[Create mobileThreatDefenseConnector](../api/intune_onboarding_mobilethreatdefenseconnector_create.md)|[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)|创建新的 [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 对象。|
|[Delete mobileThreatDefenseConnector](../api/intune_onboarding_mobilethreatdefenseconnector_delete.md)|无|删除 [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)。|
|[Update mobileThreatDefenseConnector](../api/intune_onboarding_mobilethreatdefenseconnector_update.md)|[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)|更新 [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|
|lastHeartbeatDateTime|DateTimeOffset|管理员启用“连接到 MTP”选项后的上次检测信号的时间戳|
|partnerState|String|此租户的合作伙伴状态 可取值为：`unavailable`、`available`、`enabled`、`unresponsive`。|
|androidEnabled|Boolean|Android 切换，打开或关闭。|
|androidDeviceBlockedOnMissingPartnerData|Boolean|对于 Android，允许管理员配置必须先从数据同步合作伙伴接收到数据才能将其视为符合|
|iosDeviceBlockedOnMissingPartnerData|Boolean|对于 IOS，允许管理员配置必须先从数据同步合作伙伴接收到数据才能将其视为符合|
|partnerUnsupportedOsVersionBlocked|Boolean|允许管理员阻止启用的平台上不符合最低版本要求的设备|
|iosEnabled|Boolean|IOS 切换，打开或关闭。|
|partnerUnresponsivenessThresholdInDays|Int32|获取或设置每个租户允许此合作伙伴集成不响应的天数|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileThreatDefenseConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "androidEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 1024
}
```



