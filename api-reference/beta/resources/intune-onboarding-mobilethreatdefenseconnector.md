---
title: mobileThreatDefenseConnector 资源类型
description: 表示移动威胁防护合作伙伴连接的实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30dbd65cc36f220051348bbc3d0efc79b949eae5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725188"
---
# <a name="mobilethreatdefenseconnector-resource-type"></a>mobileThreatDefenseConnector 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示移动威胁防护合作伙伴连接的实体。

## <a name="methods"></a>Methods
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
|id|String|尚未记录|
|lastHeartbeatDateTime|DateTimeOffset|从数据同步合作伙伴接收到上一个检测信号的日期/时间|
|partnerState|[mobileThreatPartnerTenantState](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|此帐户的数据同步合作伙伴状态。 可取值为：`unavailable`、`available`、`enabled`、`unresponsive`。|
|androidMobileApplicationManagementEnabled|布尔|对于 Android，请设置是否应在移动应用程序管理 (MAM) 评估期间使用来自数据同步合作伙伴的数据。 对于移动应用程序管理 (MAM) 评估，仅可为每个平台启用一个合作伙伴。|
|iosMobileApplicationManagementEnabled|布尔|对于 IOS，获取或设置是否应在移动应用程序管理 (MAM) 评估期间使用来自数据同步合作伙伴的数据。 对于移动应用程序管理 (MAM) 评估，仅可为每个平台启用一个合作伙伴。|
|androidEnabled|Boolean|对于 Android 设备，设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据|
|iosEnabled|Boolean|对于 iOS 设备，获取或设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据|
|windowsEnabled|布尔|对于 Windows，获取或设置是否应在合规性评估期间使用来自数据同步合作伙伴的数据|
|macEnabled|布尔|对于 Mac，获取或设置是否应在合规性评估期间使用来自数据同步合作伙伴的数据|
|androidDeviceBlockedOnMissingPartnerData|Boolean|对于 Android 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据|
|iosDeviceBlockedOnMissingPartnerData|Boolean|对于 iOS 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据|
|windowsDeviceBlockedOnMissingPartnerData|布尔|对于 Windows，在将设备标记为合规之前，设置 Intune 是否必须接收来自数据同步合作伙伴的数据|
|macDeviceBlockedOnMissingPartnerData|布尔|对于 Mac，获取或设置 Intune 是否必须在标记符合设备的之前从数据同步合作伙伴接收数据|
|partnerUnsupportedOsVersionBlocked|Boolean|获取或设置是否阻止不符合数据同步合作伙伴最低版本要求的启用平台上的设备|
|partnerUnresponsivenessThresholdInDays|Int32|获取或设置每个租户允许此合作伙伴集成不响应的天数|
|allowPartnerToCollectIOSApplicationMetadata|布尔|对于 IOS 设备，管理员可以配置数据同步合作伙伴是否可以从 Intune 收集有关已安装应用程序的元数据|

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
  "androidMobileApplicationManagementEnabled": true,
  "iosMobileApplicationManagementEnabled": true,
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





