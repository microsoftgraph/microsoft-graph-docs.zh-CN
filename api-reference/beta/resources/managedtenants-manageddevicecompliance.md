---
title: managedDeviceCompliance 资源类型
description: 表示属于给定托管租户的每个托管设备的设备合规性状态。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: ce9f8ea1ed4e2a083daa053d17714569b4b2abfe
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61811162"
---
# <a name="manageddevicecompliance-resource-type"></a>managedDeviceCompliance 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示属于给定托管租户的每个托管设备的设备合规性状态。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedDeviceCompliances](../api/managedtenants-managedtenant-list-manageddevicecompliances.md)|[microsoft.graph.managedTenants.managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) 集合|获取 [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) 对象及其属性的列表。|
|[获取 managedDeviceCompliance](../api/managedtenants-manageddevicecompliance-get.md)|[microsoft.graph.managedTenants.managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md)|读取 [managedDeviceCompliance 对象的属性和](../resources/managedtenants-manageddevicecompliance.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|complianceStatus|String|设备的符合性状态。 此属性是只读的。 可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod` 或 `configManager`。 可选。 只读。|
|deviceType|String|设备平台。 此属性是只读的。 可能的值是 `desktop` `windowsRT` `winMO6` ：、、、、、、、、、、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `chromeOS` `linux` `blackberry` `palm` `unknown` `cloudPC` 、  可选。 只读。|
|id|String|此实体的唯一标识。 必需。 只读。|
|inGracePeriodUntilDateTime|DateTimeOffset|宽限期到期的日期和时间。 可选。 只读。|
|lastRefreshedDateTime|DateTimeOffset|实体上次在多租户管理平台中更新的日期和时间。 可选。 只读。|
|lastSyncDateTime|DateTimeOffset|设备上次成功完成与用户同步的Microsoft Endpoint Manager。 可选。 只读。|
|managedDeviceId|String|托管设备在Microsoft Endpoint Manager。 可选。 只读。|
|managedDeviceName|String|托管显示名称的设备配置。 可选。 只读。|
|manufacturer|String|设备的制造。 可选。 只读。|
|model|String|设备的型号。 可选。 只读。|
|osDescription|String|托管设备的操作系统说明。 可选。 只读。|
|osVersion|String|托管设备的操作系统版本。 可选。 只读。|
|ownerType|String|托管设备的所有者类型。 可选。 只读。|
|tenantDisplayName|String|托管显示名称租户的租户。 可选。 只读。|
|tenantId|String|托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。 可选。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managedDeviceCompliance",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedDeviceCompliance",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "complianceStatus": "String",
  "osDescription": "String",
  "osVersion": "String",
  "lastSyncDateTime": "String (timestamp)",
  "ownerType": "String",
  "model": "String",
  "manufacturer": "String",
  "inGracePeriodUntilDateTime": "String (timestamp)",
  "lastRefreshedDateTime": "String (timestamp)",
  "deviceType": "String"
}
```
