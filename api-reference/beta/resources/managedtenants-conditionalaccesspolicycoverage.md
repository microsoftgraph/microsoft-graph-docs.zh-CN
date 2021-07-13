---
title: conditionalAccessPolicyCoverage 资源类型
description: 表示有关定义Azure Active Directory托管租户的资源访问规则的任何策略的信息。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: a4bc4f336692166ff032727a6fb13222edd9d7d9
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402069"
---
# <a name="conditionalaccesspolicycoverage-resource-type"></a>conditionalAccessPolicyCoverage 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关定义Azure Active Directory托管租户的资源访问规则的任何策略的信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 conditionalAccessPolicyCoverages](../api/managedtenants-managedtenant-list-conditionalaccesspolicycoverages.md)|[microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) 集合|获取 [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) 对象及其属性的列表。|
|[获取 conditionalAccessPolicyCoverage](../api/managedtenants-conditionalaccesspolicycoverage-get.md)|[microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md)|读取 [conditionalAccessPolicyCoverage 对象的属性和](../resources/managedtenants-conditionalaccesspolicycoverage.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|conditionalAccessPolicyState|String|条件访问策略的状态。 可取值为：`enabled`、`disabled`、`enabledForReportingButNotEnforced`。 此为必需属性。 只读。|
|id|String|此实体的唯一标识符。 必填。 只读。|
|latestPolicyModifiedDateTime|DateTimeOffset|上次修改条件访问策略的日期和时间。 必填。 只读。|
|requiresDeviceCompliance|布尔|指示条件访问策略是否需要设备符合性的标志。 必填。 只读。|
|tenantDisplayName|String|托管显示名称租户的租户。 必填。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
  "id": "String (identifier)",
  "tenantDisplayName": "String",
  "conditionalAccessPolicyState": "String",
  "requiresDeviceCompliance": "Boolean",
  "latestPolicyModifiedDateTime": "String (timestamp)"
}
```
