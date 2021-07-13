---
title: windowsProtectionState 资源类型
description: 表示Windows托管设备的 Windows。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: dc89db998f8fa75e46b3346f2517e5ee950e0ab5
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402228"
---
# <a name="windowsprotectionstate-resource-type"></a>windowsProtectionState 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示Windows托管设备的 Windows。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsProtectionStates](../api/managedtenants-managedtenant-list-windowsprotectionstates.md)|[microsoft.graph.managedTenants.windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) 集合|获取 [windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) 对象及其属性的列表。|
|[获取 windowsProtectionState](../api/managedtenants-windowsprotectionstate-get.md)|[microsoft.graph.managedTenants.windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md)|读取 [windowsProtectionState 对象的属性和](../resources/managedtenants-windowsprotectionstate.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|antiMalwareVersion|String|托管设备的反恶意软件版本。 可选。 只读。|
|attentionRequired|布尔|指示托管设备是否需要关注的标志。 可选。 只读。|
|deviceDeleted|布尔|指示是否已删除托管设备的标志。 可选。 只读。|
|devicePropertyRefreshDateTime|DateTimeOffset|设备属性已刷新的日期和时间。 可选。 只读。|
|engineVersion|String|托管设备的防病毒引擎版本。 可选。 只读。|
|fullScanOverdue|布尔|指示托管设备快速扫描是否过期的标志。 可选。 只读。|
|fullScanRequired|布尔|指示托管设备是否过期的完整扫描的标志。 可选。 只读。|
|id|String|保护状态Windows标识符。 必填。 只读。|
|lastFullScanDateTime|DateTimeOffset|完成完全扫描的日期和时间。 可选。 只读。|
|lastFullScanSignatureVersion|String|用于执行上一次完全扫描的反恶意软件版本。 可选。 只读。|
|lastQuickScanDateTime|DateTimeOffset|完成快速扫描的日期和时间。 可选。 只读。|
|lastQuickScanSignatureVersion|String|用于执行上一次完全扫描的反恶意软件版本。 可选。 只读。|
|lastRefreshedDateTime|DateTimeOffset|实体上次在多租户管理平台中更新的日期和时间。 可选。 只读。|
|lastReportedDateTime|DateTimeOffset|上次为托管设备报告保护状态的日期和时间。 可选。 只读。|
|malwareProtectionEnabled|布尔|指示是否对托管设备启用恶意软件保护的标志。 可选。 只读。|
|managedDeviceHealthState|String|托管设备的运行状况。 可选。 只读。|
|managedDeviceId|String|托管设备的唯一标识符。 可选。 只读。|
|managedDeviceName|String|托管显示名称的设备配置。 可选。 只读。|
|networkInspectionSystemEnabled|布尔|指示是否已启用网络检查系统的标志。 可选。 只读。|
|quickScanOverdue|布尔|指示快速扫描过期的天气标志。 可选。 只读。|
|realTimeProtectionEnabled|布尔|指示是否已启用实时保护的标志。 可选。 只读。|
|rebootRequired|布尔|指示是否需要重新启动的标志。 可选。 只读。|
|signatureUpdateOverdue|布尔|指示签名更新是否过期的标志。 可选。 只读。|
|signatureVersion|String|托管设备的签名版本。 可选。 只读。|
|tenantDisplayName|String|托管显示名称租户的租户。 可选。 只读。|
|tenantId|String|托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。 可选。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.windowsProtectionState",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.windowsProtectionState",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "malwareProtectionEnabled": "Boolean",
  "managedDeviceHealthState": "String",
  "realTimeProtectionEnabled": "Boolean",
  "networkInspectionSystemEnabled": "Boolean",
  "quickScanOverdue": "Boolean",
  "fullScanOverdue": "Boolean",
  "signatureUpdateOverdue": "Boolean",
  "rebootRequired": "Boolean",
  "attentionRequired": "Boolean",
  "fullScanRequired": "Boolean",
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)",
  "devicePropertyRefreshDateTime": "String (timestamp)",
  "deviceDeleted": "Boolean",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
