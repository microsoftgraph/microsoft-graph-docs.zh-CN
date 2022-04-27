---
title: riskyUserHistoryItem 资源类型
description: 有风险的用户历史记录项
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c5853ec669c4b8ed1e048dce701ac65b3fbc1dc4
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060977"
---
# <a name="riskyuserhistoryitem-resource-type"></a>riskyUserHistoryItem 资源类型

命名空间：microsoft.graph

表示由Azure AD标识保护确定的Azure AD用户的风险历史记录。

继承自 [riskyUser](../resources/riskyuser.md)。

>[!NOTE]
> 1. 使用此 API 需要Azure AD Premium P2许可证。
> 2. 风险历史记录数据的可用性受[Azure AD数据保留策略](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data)的控制。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出历史记录](../api/riskyuser-list-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 集合|从历史记录导航属性获取 riskyUserHistoryItems。|
|[获取历史记录](../api/riskyuser-get-riskyuserhistoryitem.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|读取 [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|活动|[riskUserActivity](../resources/riskuseractivity.md)|与用户风险级别更改相关的活动。|
|id|String|继承自 [实体](../resources/entity.md)|
|initiatedBy|String|执行操作的执行组件的 ID。|
|isDeleted|Boolean| 继承自 [riskyUser](../resources/riskyuser.md)|
|isProcessing|Boolean| 继承自 [riskyUser](../resources/riskyuser.md)|
|riskDetail|riskDetail|继承自 [riskyUser](../resources/riskyuser.md)。 可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。|
|riskLastUpdatedDateTime|DateTimeOffset|继承自 [riskyUser](../resources/riskyuser.md)|
|riskLevel|riskLevel|继承自 [riskyUser](../resources/riskyuser.md)。 可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。|
|riskState|riskState|继承自 [riskyUser](../resources/riskyuser.md)。 可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。|
|userDisplayName|String|继承自 [riskyUser](../resources/riskyuser.md)|
|userId|String|用户的 ID。|
|userPrincipalName|String|有风险的用户主体名称。 继承自 [riskyUser](../resources/riskyuser.md)|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|历史|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 集合| 继承自 [riskyUser](../resources/riskyuser.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
  "id": "String (identifier)",
  "isDeleted": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userId": "String",
  "initiatedBy": "String",
  "activity": {
    "@odata.type": "microsoft.graph.riskUserActivity"
  }
}
```


