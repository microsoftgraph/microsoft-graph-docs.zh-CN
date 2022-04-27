---
title: riskyUser 资源类型
description: 表示Azure AD有风险的用户。 Azure AD根据各种信号和机器学习不断评估用户风险。 此 API 提供对Azure AD中所有有风险用户的编程访问权限。
author: cloudhandler
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
ms.openlocfilehash: ff09c334f4d7301b54d70fd2527b1884bb67019e
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060533"
---
# <a name="riskyuser-resource-type"></a>riskyUser 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示Azure AD有风险的用户。 Azure AD根据各种信号和机器学习不断评估用户风险。 此 API 提供对Azure AD中所有有风险用户的编程访问权限。

有关风险事件的详细信息，请[参阅Azure Active Directory标识保护](/azure/active-directory/identity-protection/overview-identity-protection)。

>[!NOTE]
> 1. 使用 riskyUsers API 需要Azure AD Premium P2许可证。
> 2. 风险用户数据的可用性受[Azure AD数据保留策略](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data)的控制。

## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 riskyUsers](../api/riskyusers-list.md) | [riskyUser](riskyuser.md) 集合|列出有风险的用户及其属性。|
|[获取 riskyUser](../api/riskyusers-get.md) | [riskyUser](riskyuser.md)|获取特定有风险的用户及其属性。|
|[列出历史记录](../api/riskyuser-list-history.md) | [riskyUserHistoryItem](riskyuserhistoryitem.md) 集合|获取Azure AD用户的风险历史记录。|
|[确认 riskyUsers 遭到入侵](../api/riskyusers-confirmcompromised.md)|无 |确认有风险的用户已泄露。|
|[消除 riskyUsers](../api/riskyusers-dismiss.md)|无 | 消除有风险的用户的风险。|

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|id|string|有风险的用户的唯一 ID。|
|isDeleted|boolean|指示是否删除用户。 可取值为：`true`、`false`。|
|isProcessing|布尔|指示后端是否正在处理用户的风险状态。|
|riskLastUpdatedDateTime|DateTimeOffset|风险用户上次更新的日期和时间。  DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|riskLevel|riskLevel| 检测到的风险用户的级别。 可能的值是`low`， ， `high``medium`， `hidden`， ， `none`。 `unknownFutureValue`  |
|riskState|riskState| 用户风险的状态。 可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。  |
|riskDetail|riskDetail| 可能的值是`none`，`adminGeneratedTemporaryPassword`、、`userPerformedSecuredPasswordReset``userPerformedSecuredPasswordChange`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy``adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、 `adminConfirmedUserCompromised``unknownFutureValue`  |
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
