---
title: mobileThreatDefenseConnector 资源类型
description: 表示移动威胁防护合作伙伴连接的实体。
ms.openlocfilehash: ee832f8e3acce151d51483522aa0c76b181e93d6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045105"
---
# <a name="mobilethreatdefenseconnector-resource-type"></a>mobileThreatDefenseConnector 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

表示移动威胁防护合作伙伴连接的实体。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List mobileThreatDefenseConnectors](../api/intune-onboarding-mobilethreatdefenseconnector-list.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 集合|列出 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象的属性和关系。|
|[Get mobileThreatDefenseConnector](../api/intune-onboarding-mobilethreatdefenseconnector-get.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|读取 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象的属性和关系。|
|[Create mobileThreatDefenseConnector](../api/intune-onboarding-mobilethreatdefenseconnector-create.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|创建新的 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象。|
|[Delete mobileThreatDefenseConnector](../api/intune-onboarding-mobilethreatdefenseconnector-delete.md)|无|删除 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)。|
|[Update mobileThreatDefenseConnector](../api/intune-onboarding-mobilethreatdefenseconnector-update.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|更新 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|尚未记录|
|lastHeartbeatDateTime|DateTimeOffset|从数据同步合作伙伴接收到上一个检测信号的日期/时间|
|partnerState|[mobileThreatPartnerTenantState](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|数据同步合作伙伴为此帐户的的状态。 可取值为：`unavailable`、`available`、`enabled`、`unresponsive`。|
|androidEnabled|Boolean|对于 Android 设备，设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据|
|iosEnabled|Boolean|对于 iOS 设备，获取或设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据|
|windowsEnabled|布尔|用于 Windows，获取或设置是否法规遵从性评估期间应使用从数据同步合作伙伴的数据|
|macEnabled|布尔|用于 Mac，获取或设置是否法规遵从性评估期间应使用从数据同步合作伙伴的数据|
|androidDeviceBlockedOnMissingPartnerData|Boolean|对于 Android 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据|
|iosDeviceBlockedOnMissingPartnerData|Boolean|对于 iOS 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据|
|windowsDeviceBlockedOnMissingPartnerData|布尔|对于 Windows，设置是否 Intune 必须接收来自之前标记设备符合数据同步合作伙伴的数据|
|macDeviceBlockedOnMissingPartnerData|布尔|用于 Mac，获取或设置是否 Intune 必须接收来自之前标记设备符合数据同步合作伙伴的数据|
|partnerUnsupportedOsVersionBlocked|Boolean|获取或设置是否阻止不符合数据同步合作伙伴最低版本要求的启用平台上的设备|
|partnerUnresponsivenessThresholdInDays|Int32|获取或设置每个租户允许此合作伙伴集成不响应的天数|
|allowPartnerToCollectIOSApplicationMetadata|布尔|对于 IOS 设备，允许管理员配置是否从 Intune 数据同步合作伙伴中可能还收集有关已安装应用程序的元数据|

## <a name="relationships"></a>Relationships
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
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 1024,
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```





