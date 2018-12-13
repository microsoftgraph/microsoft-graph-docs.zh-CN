---
title: riskyUsers 资源类型
description: 代表 Azure AD 用户面临危险。 Azure AD 不断计算用户根据各种信号和机器学习的风险。 此 API 在 Azure AD 中所有存在风险的用户提供编程访问。
ms.openlocfilehash: 47856ab28a52046f19087e0f59745efb9855e81a
ms.sourcegitcommit: ba6b1d1a12dcb54916b4d3e529c856f6514e01e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/12/2018
ms.locfileid: "27241060"
---
# <a name="riskyusers-resource-type"></a>riskyUsers 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

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
|`riskDetail`|`riskDetail`|提供原因后面的 risky 用户、 登录或风险事件特定状态。 可能的值为： `none`， `adminGeneratedTemporaryPassword`， `userPerformedSecuredPasswordChange`， `userPerformedSecuredPasswordReset`， `adminConfirmedSigninSafe`， `aiConfirmedSigninSafe`， `userPassedMFADrivenByRiskBasedPolicy`， `adminDismissedAllRiskForUser`， `adminConfirmedSigninCompromised`， `unknownFutureValue`。 值`none`是指的任何操作已执行上的用户或登录到目前为止。|
|`riskLevel`|`riskLevel`|提供 risky 用户、 登录或风险事件的总体风险级别。 可能的值为： `none`， `low`， `medium`， `high`， `hidden`，和`unknownFutureValue`。 值`hidden`是指为 Azure AD 身份保护未启用的用户或登录。|
|`riskState`|`riskState`|提供 risky 用户、 登录或风险事件的风险状态。 可能的值为： `none`， `confirmedSafe`， `remediated`， `dismissed`， `atRisk`， `confirmedCompromised`， `unknownFutureValue`。|
|`riskLastUpdatedDateTime`|`datetime`|日期和 risky 用户上次更新时间|
|`userDisplayName`|`string`|Risky 的用户显示名称|
|`userPrincipalName`|`string`|Risky 的用户主体名称|

## <a name="relationships"></a>Relationships

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|ID|UserObjectId| 与给定的风险事件相关联的用户的唯一标识符。|
|isGuest|isGuest| Risky 用户可以是家庭用户 (B2E) 或来宾用户 （B2B、 B2C）。|
|被|被| 用户可能也不能删除。 |
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
"riskState":  {"@odata.type": "microsoft.graph.riskState"}
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
