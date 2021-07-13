---
title: riskyUser 资源类型
description: 表示每个托管租户中标记为风险的帐户。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 3f66998080abcf9580cdd36e0f3e4b24edab2d2d
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402398"
---
# <a name="riskyuser-resource-type"></a>riskyUser 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示每个托管租户中标记为风险的帐户。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 riskyUsers](../api/managedtenants-managedtenant-list-riskyusers.md)|[microsoft.graph.managedTenants.riskyUser](../resources/managedtenants-riskyuser.md) 集合|获取 [riskyUser](../resources/managedtenants-riskyuser.md) 对象及其属性的列表。|
|[获取 riskyUser](../api/managedtenants-riskyuser-get.md)|[microsoft.graph.managedTenants.riskyUser](../resources/managedtenants-riskyuser.md)|读取 [riskyUser](../resources/managedtenants-riskyuser.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此实体的唯一标识符。 必填。 只读。|
|isDeleted|布尔|指示帐户是否已删除的标志。 可选。 只读。|
|lastRefreshedDateTime|DateTimeOffset|实体上次在多租户管理平台中更新的日期和时间。 可选。 只读。|
|riskDetail|String|标记为风险的帐户的风险详细信息。 可选。 只读。|
|riskLastUpdatedDateTime|DateTimeOffset|上次更新风险信息的日期和时间。 可选。 只读。|
|riskLevel|String|检测到的风险级别。 可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。 可选。 只读。|
|riskState|String|检测到的风险状态。 可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。 可选。 只读。|
|tenantDisplayName|String|托管显示名称租户的租户。 可选。 只读。|
|tenantId|String|托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。 必填。 只读。|
|userDisplayName|String|The 显示名称 for the account where risk was detected. 可选。 只读。|
|userId|String|检测到风险的用户帐户的标识符。 必填。 只读。|
|userPrincipalName|String|用户主体名称 (检测) 帐户的 UPN 名称。 可选。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.riskyUser",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.riskyUser",
  "id": "String (identifier)",
  "userId": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "riskState": "String",
  "riskLevel": "String",
  "riskDetail": "String",
  "isDeleted": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
