---
title: riskyUserHistoryItem 资源类型
description: 有风险的用户历史记录项
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4bcf9e1834e8fff48a148095ffe7ddbd459ee23e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895998"
---
# <a name="riskyuserhistoryitem-resource-type"></a>riskyUserHistoryItem 资源类型

命名空间：microsoft.graph

表示 azure AD 用户的风险历史记录，由 Azure AD Identity Protection 确定。


继承自[riskyUser](../resources/riskyuser.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表历史记录](../api/riskyuser-list-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)集合|从 "历史记录" 导航属性中获取 riskyUserHistoryItems。|
|[获取历史记录](../api/riskyuser-get-riskyuserhistoryitem.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|读取[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|activity|[riskUserActivity](../resources/riskuseractivity.md)|与用户风险级别更改相关的活动。|
|id|String|继承自[entity](../resources/entity.md)|
|initiatedBy|String|执行此操作的主角的 id。|
|isDeleted|Boolean| 继承自[riskyUser](../resources/riskyuser.md)|
|isProcessing|Boolean| 继承自[riskyUser](../resources/riskyuser.md)|
|riskDetail|riskDetail|继承自[riskyUser](../resources/riskyuser.md)。 可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。|
|riskLastUpdatedDateTime|DateTimeOffset|继承自[riskyUser](../resources/riskyuser.md)|
|riskLevel|riskLevel|继承自[riskyUser](../resources/riskyuser.md)。 可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。|
|riskState|riskState|继承自[riskyUser](../resources/riskyuser.md)。 可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。|
|userDisplayName|String|继承自[riskyUser](../resources/riskyuser.md)|
|userId|String|用户的 id。|
|userPrincipalName|字符串|有风险的用户主体名称。 继承自[riskyUser](../resources/riskyuser.md)|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|日志|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)集合| 继承自[riskyUser](../resources/riskyuser.md)|

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

