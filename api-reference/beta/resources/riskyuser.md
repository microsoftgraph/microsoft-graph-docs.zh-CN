---
title: riskyUser 资源类型
description: 表示有风险的 Azure AD 用户。 Azure AD 会根据各种信号和机器学习持续评估用户风险。 此 API 提供对 Azure AD 中所有风险用户的编程访问。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 179a6cbddf3e4b27c47761bd81aad1052ae7f728
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343533"
---
# <a name="riskyuser-resource-type"></a>riskyUser 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有风险的 Azure AD 用户。 Azure AD 会根据各种信号和机器学习持续评估用户风险。 此 API 提供对 Azure AD 中所有风险用户的编程访问。

有关风险事件的详细信息, 请参阅[Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)。

>**注意:** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。

## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 riskyUsers](../api/riskyusers-list.md) | [riskyUser](riskyUser.md)集合|列出有风险的用户及其属性。|
|[获取 riskyUser](../api/riskyusers-get.md) | [riskyUser](riskyUser.md)|获取特定的有风险的用户及其属性。|
|[确认 riskyUsers 已泄露](../api/riskyusers-confirmcompromised.md)|无 |确认有风险的用户受到威胁。|
|[消除 riskyUsers](../api/riskyusers-dismiss.md)|无 | 消除有风险的用户的风险。|

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|`id`|`string`|用户面临风险的唯一 id|
|`isDeleted`|`bool`|指示是否删除用户。 可能的值包括`true`:、`false`|
|`isGuest`|`bool`|指示用户是否为来宾用户。 可取值为：`true`、`false`。 如此如果用户的标识位于租户外部, 请考虑。 此用户可以是在 Azure AD、MSA 或第三方标识提供程序中具有标识的 B2B 或 B2C 用户。 假如果用户的标识位于租户内部, 则考虑|
|`isProcessing`|`bool`|指示后端正在处理用户的危险状态 wehther|
|`riskLastUpdatedDateTime`|`datetime`|上次更新有风险的用户的日期和时间|
|`riskLevel`|`riskLevel`| 可能的值为 low、medium、high、hidden、none、向 unknownfuturevalue。  |
|`riskState`|`riskState`| 可能的值为 none、confirmedSafe、修正、atRisk、向 unknownfuturevalue。  |
|`riskDetail`|`riskDetail`| 可能的值为 none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、向 unknownfuturevalue。  |
|`userDisplayName`|`string`|有风险的用户显示名称|
|`userPrincipalName`|`string`|有风险的用户主体名称|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|日志|[riskyUserHistoryItem](riskyuserhistoryitem.md)集合| |

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
"isGuest": "boolean",
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
