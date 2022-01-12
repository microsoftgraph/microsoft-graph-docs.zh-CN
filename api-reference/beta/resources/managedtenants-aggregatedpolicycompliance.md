---
title: aggregatedPolicyCompliance 资源类型
description: 表示托管租户的设备合规性聚合视图。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 9db12e1a86ee6953c81be839abee695d2ba3a55a
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61862337"
---
# <a name="aggregatedpolicycompliance-resource-type"></a>aggregatedPolicyCompliance 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示托管租户的设备合规性聚合视图。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 aggregatedPolicyCompliances](../api/managedtenants-managedtenant-list-aggregatedpolicycompliances.md)|[microsoft.graph.managedTenants.aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) 集合|获取聚合 [PolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) 对象及其属性的列表。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|compliancePolicyId|String|设备合规性策略的标识符。 可选。 只读。|
|compliancePolicyName|String|设备合规性策略的名称。 可选。 只读。|
|compliancePolicyPlatform|String|设备合规性策略的平台。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`androidAOSP`、`all`。 可选。 只读。|
|compliancePolicyType|String|合规性策略的类型。 可选。 只读。|
|id|String|聚合设备合规性策略的唯一标识符。 必需。 只读|
|lastRefreshedDateTime|DateTimeOffset|实体上次在多租户管理平台中更新的日期和时间。 可选。 只读。|
|numberOfCompliantDevices|Int64|符合标准的设备数量。 可选。 只读。|
|numberOfErrorDevices|Int64|出现错误状态的设备数。 可选。 只读。|
|numberOfNonCompliantDevices|Int64|不合规状态的设备数量。 可选。 只读。|
|policyModifiedDateTime|DateTimeOffset|上次修改设备策略的日期和时间。 可选。 只读。|
|tenantDisplayName|String|托管显示名称租户的租户。 可选。 只读。|
|tenantId|String|托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。 可选。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.aggregatedPolicyCompliance",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.aggregatedPolicyCompliance",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "compliancePolicyId": "String",
  "compliancePolicyName": "String",
  "compliancePolicyType": "String",
  "compliancePolicyPlatform": "String",
  "numberOfCompliantDevices": "Integer",
  "numberOfNonCompliantDevices": "Integer",
  "numberOfErrorDevices": "Integer",
  "policyModifiedDateTime": "String (timestamp)",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
