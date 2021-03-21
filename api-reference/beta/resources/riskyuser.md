---
title: riskyUser 资源类型
description: 表示处于风险中的 Azure AD 用户。 Azure AD 根据各种信号和机器学习持续评估用户风险。 此 API 为 Azure AD 中所有处于风险中的用户提供编程访问权限。
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
ms.openlocfilehash: d2e0942e92b1dcd648812503a923dac51a640be1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960318"
---
# <a name="riskyuser-resource-type"></a>riskyUser 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示处于风险中的 Azure AD 用户。 Azure AD 根据各种信号和机器学习持续评估用户风险。 此 API 为 Azure AD 中所有处于风险中的用户提供编程访问权限。

有关风险事件详细信息，请参阅 Azure [Active Directory Identity Protection。](/azure/active-directory/identity-protection/overview-identity-protection)

>**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。

## <a name="methods"></a>Methods

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 riskyUsers](../api/riskyusers-list.md) | [riskyUser](riskyuser.md) 集合|列出有风险的用户及其属性。|
|[获取 riskyUser](../api/riskyusers-get.md) | [riskyUser](riskyuser.md)|获取特定有风险的用户及其属性。|
|[列表历史记录](../api/riskyuser-list-history.md) | [riskyUserHistoryItem](riskyuserhistoryitem.md) 集合|获取 Azure AD 用户的风险历史记录。|
|[确认 riskyUsers 遭到入侵](../api/riskyusers-confirmcompromised.md)|无 |确认存在风险的用户是否遭到入侵。|
|[消除 riskyUsers](../api/riskyusers-dismiss.md)|无 | 消除风险用户的风险。|

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|id|string|处于风险中的用户的唯一 ID。|
|isDeleted|boolean|指示用户是否被删除。 可取值为：`true`、`false`。|
|isProcessing|boolean|指示后端是否正在处理用户的风险状态。|
|riskLastUpdatedDateTime|DateTimeOffset|上次更新有风险用户的日期和时间。  DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z`|
|riskLevel|riskLevel| 检测到的风险用户级别。 可能的值为 `low` `medium` `high` `hidden` `none` `unknownFutureValue` 、、、。  |
|riskState|riskState| 用户风险的状态。 可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。  |
|riskDetail|riskDetail| 可能的值为 `none` `adminGeneratedTemporaryPassword` `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` 、、、、、、、、、 `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` `unknownFutureValue` 。  |
|userDisplayName|string|有风险的用户显示名称。|
|userPrincipalName|string|有风险的用户主体名称。|

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
