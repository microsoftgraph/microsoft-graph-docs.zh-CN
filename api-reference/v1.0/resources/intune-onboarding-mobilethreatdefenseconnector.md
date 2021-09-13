---
title: mobileThreatDefenseConnector 资源类型
description: 表示移动威胁防护合作伙伴连接的实体。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6648c53a65898b124c544e30cae0f3d74f8f92e0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094294"
---
# <a name="mobilethreatdefenseconnector-resource-type"></a>mobileThreatDefenseConnector 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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
|id|String|尚未记录|
|lastHeartbeatDateTime|DateTimeOffset|从数据同步合作伙伴接收到上一个检测信号的日期/时间|
|partnerState|[mobileThreatPartnerTenantState](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|数据同步此帐户的合作伙伴状态。 可取值为：`unavailable`、`available`、`enabled`、`unresponsive`。|
|androidEnabled|Boolean|对于 Android 设备，设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据|
|iosEnabled|Boolean|对于 iOS 设备，获取或设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据|
|androidDeviceBlockedOnMissingPartnerData|Boolean|对于 Android 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据|
|iosDeviceBlockedOnMissingPartnerData|Boolean|对于 iOS 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据|
|partnerUnsupportedOsVersionBlocked|Boolean|获取或设置是否阻止不符合数据同步合作伙伴最低版本要求的启用平台上的设备|
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
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 1024
}
```




