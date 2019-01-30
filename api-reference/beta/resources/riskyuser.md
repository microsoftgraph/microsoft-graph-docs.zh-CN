---
title: riskyUsers 资源类型
description: 代表 Azure AD 用户面临危险。 Azure AD 不断计算用户根据各种信号和机器学习的风险。 此 API 在 Azure AD 中所有存在风险的用户提供编程访问。
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 27c189a81d6ba4e088c1242acfd2cf0d0f5c56c5
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643907"
---
# <a name="riskyusers-resource-type"></a>riskyUsers 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表 Azure AD 用户面临危险。 Azure AD 不断计算用户根据各种信号和机器学习的风险。 此 API 在 Azure AD 中所有存在风险的用户提供编程访问。

> **注意：** 此 API 要求的 Azure AD Premium P2 许可证。

有关风险事件的详细信息，请参阅[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)。

## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列表 riskyUsers](../api/riskyusers-list.md) | [riskyUsers](riskyuser.md) |列出 risky 用户和及其属性。|
|[获取 riskyUsers](../api/riskyusers-get.md) | [riskyUsers](riskyuser.md)|获取特定 risky 用户和其属性。|

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|`id`|`string`|风险的用户的唯一 id|
|`isDeleted`|`bool`|指示是否删除用户。 可能的值为： `true`，`false`|
|`isGuest`|`bool`|指示用户是否来宾用户。 可取值为：`true`、`false`。 如果用户的标识位于中考虑租户之外，则为 true。 此用户可以在 Azure AD，MSA 中是 B2B 或 B2C 用户标识或第三方标识提供程序。 如果用户的标识位于内部中考虑租户则为 false|
|`riskDetail`|`riskDetail`|提供风险用户、登录或风险事件的特定状态背后的“原因”。 可取值包括：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`unknownFutureValue`。 值 `none` 表示到目前为止尚未对用户或登录执行任何操作。|
|`riskLevel`|`riskLevel`|提供 risky 用户、 登录或风险事件的总体风险级别。 可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。 值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。|
|`riskState`|`riskState`|提供风险用户、登录或风险事件的“风险状态”。 可取值包括：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。|
|`riskLastUpdatedDateTime`|`datetime`|日期和 risky 用户上次更新时间|
|`userDisplayName`|`string`|Risky 的用户显示名称|
|`userPrincipalName`|`string`|Risky 的用户主体名称|

## <a name="relationships"></a>关系

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|id|UserObjectId| 与给定的风险事件相关联的用户的唯一标识符。|
|isGuest|isGuest| Risky 用户可以是家庭用户 (B2E) 或来宾用户 （B2B、 B2C）。|
|isDeleted|isDeleted| 用户可能也不能删除。 |
|riskState|riskState| Risky 用户可能存在多个状态之一。 |
|riskDetail|riskDetail| 特定状态中，risky 用户可能会因多个原因。 |
|riskLevel|riskLevel| Risky 用户可以被视为多个风险级别之一。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskyusers"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isGuest": "boolean",
"isDeleted": "boolean",
"riskDetail":  {"@odata.type": "microsoft.graph.riskDetail"},
"riskLevel":  {"@odata.type": "microsoft.graph.riskLevel"},
"riskState":  {"@odata.type": "microsoft.graph.riskState"},
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/riskyuser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
