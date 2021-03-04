---
title: riskyUser 资源类型
description: 表示处于风险中的 Azure AD 用户。 Azure AD 根据各种信号和机器学习持续评估用户风险。 此 API 为 Azure AD 中所有处于风险中的用户提供编程访问。
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
ms.openlocfilehash: 9a234bc4c84ed6acc569f98c8c9b5d475a5b56be
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442852"
---
# <a name="riskyuser-resource-type"></a>riskyUser 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示处于风险中的 Azure AD 用户。 Azure AD 根据各种信号和机器学习持续评估用户风险。 此 API 为 Azure AD 中所有处于风险中的用户提供编程访问。

有关风险事件详细信息，请参阅 Azure [Active Directory Identity Protection。](/azure/active-directory/identity-protection/overview-identity-protection)

>**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。

## <a name="methods"></a>Methods

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 riskyUsers](../api/riskyusers-list.md) | [riskyUser](riskyuser.md) 集合|列出有风险的用户及其属性。|
|[获取 riskyUser](../api/riskyusers-get.md) | [riskyUser](riskyuser.md)|获取特定有风险的用户及其属性。|
|[列表历史记录](../api/riskyuser-list-history.md) | [riskyUserHistoryItem](riskyuserhistoryitem.md) 集合|获取 Azure AD 用户的风险历史记录。|
|[确认 riskyUsers 泄露](../api/riskyusers-confirmcompromised.md)|无 |确认风险用户受到威胁。|
|[消除 riskyUsers](../api/riskyusers-dismiss.md)|无 | 消除风险用户的风险。|

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|`id`|`string`|处于风险中的用户的唯一 ID。|
|`isDeleted`|`bool`|指示是否删除用户。 可取值为：`true`、`false`。|
|`isProcessing`|`bool`|指示后端是否正在处理用户的风险状态。|
|`riskLastUpdatedDateTime`|`datetime`|风险用户上次更新的日期和时间|
|`riskLevel`|`riskLevel`| 可能的值为低、中、高、隐藏、无、unknownFutureValue。  |
|`riskState`|`riskState`| 可能的值是 none、confirmedSafe、修正、atRisk、unknownFutureValue。  |
|`riskDetail`|`riskDetail`| 可能的值为 none、adminGeneratedTemporaryPassword、 userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromed、hidden、adminConfirmedUserCompromed、unknownFutureValue。  |
|`userDisplayName`|`string`|有风险的用户显示名称。|
|`userPrincipalName`|`string`|有风险的用户主体名称。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isProcessing": "boolean",
"isDeleted": "boolean",
"riskDetail":  "string",
"riskLevel":  "string",
"riskState":  "string",
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
