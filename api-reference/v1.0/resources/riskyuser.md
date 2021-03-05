---
title: riskyUser 资源类型
description: 有风险的用户项
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 00a284f4a3592ccf378e0e6f218c56902c219d51
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448989"
---
# <a name="riskyuser-resource-type"></a>riskyUser 资源类型

命名空间：microsoft.graph

表示处于风险中的 Azure AD 用户。 Azure AD 根据各种信号和机器学习持续评估用户风险。 此 API 为 Azure AD 中所有处于风险中的用户提供编程访问。

有关风险事件详细信息，请参阅 Azure [Active Directory Identity Protection。](/azure/active-directory/identity-protection/overview-identity-protection)

>**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 riskyUsers](../api/riskyuser-list.md)|[riskyUser](../resources/riskyuser.md) 集合|获取 **riskyUser** 对象及其属性的列表。|
|[获取 riskyUser](../api/riskyuser-get.md)|[riskyUser](../resources/riskyuser.md)|读取 **riskyUser** 对象的属性和关系。|
|[消除 riskyUser](../api/riskyuser-dismiss.md)|无|消除一个或多个 **riskyUser 对象** 的风险。 |
|[确认 riskyUser 已泄露](../api/riskyuser-confirmcompromised.md)|无|确认一个或多个 **riskyUser** 对象受到威胁。|
|[列表历史记录](../api/riskyuser-list-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 集合|从 **历史记录导航属性获取 riskyUserHistoryItems。**|
|[获取历史记录](../api/riskyuser-get-riskyuserhistoryitem.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|读取 [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 对象的属性和关系。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|处于风险中的用户的唯一 ID。|
|isDeleted|Boolean|指示用户是否被删除。 可能的值 `true` 是： `false`|
|isProcessing|Boolean|指示后端正在处理用户的风险状态|
|riskDetail|riskDetail|检测到的风险的详细信息。 可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。|
|riskLastUpdatedDateTime|DateTimeOffset|风险用户上次更新的日期和时间。|
|riskLevel|riskLevel|检测到的风险用户级别。 可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。|
|riskState|riskState|用户风险的状态。 可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。|
|userDisplayName|String|有风险的用户显示名称。|
|userPrincipalName|String|有风险的用户主体名称。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|历史记录|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 集合|   与用户风险级别更改相关的活动|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUser",
  "id": "String (identifier)",
  "isDeleted": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String"
}
```
