---
title: managedDeviceComplianceTrend 资源类型
description: 表示给定托管租户的兼容和不兼容设备的趋势。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 671f54fb20f8ef3ecc94525061009a26e2f583f9
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61793892"
---
# <a name="manageddevicecompliancetrend-resource-type"></a>managedDeviceComplianceTrend 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示给定托管租户的兼容和不兼容设备的趋势。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedDeviceComplianceTrends](../api/managedtenants-managedtenant-list-manageddevicecompliancetrends.md)|[microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) 集合|获取 [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) 对象及其属性的列表。|
|[获取 managedDeviceComplianceTrend](../api/managedtenants-manageddevicecompliancetrend-get.md)|[microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md)|读取 [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|compliantDeviceCount|Int32|具有兼容状态的设备数量。 必需。 只读。|
|configManagerDeviceCount|Int32|Configuration Manager 管理的设备数量。 必需。 只读。|
|countDateTime|String|执行合规性快照的日期和时间。 必需。 只读。|
|errorDeviceCount|Int32|出现错误状态的设备数。 必需。 只读。|
|id|String|此实体的唯一标识符。 必需。 只读。|
|inGracePeriodDeviceCount|Int32|宽限期状态的设备数量。 必需。 只读。|
|noncompliantDeviceCount|Int32|不合规状态的设备数量。 必需。 只读。|
|tenantDisplayName|String|托管显示名称租户的租户。 可选。 只读。|
|tenantId|String|托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。 可选。 只读。|
|unknownDeviceCount|Int32|未知状态的设备数量。 必需。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managedDeviceComplianceTrend",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedDeviceComplianceTrend",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "unknownDeviceCount": "Integer",
  "compliantDeviceCount": "Integer",
  "noncompliantDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "inGracePeriodDeviceCount": "Integer",
  "configManagerDeviceCount": "Integer",
  "countDateTime": "String"
}
```
