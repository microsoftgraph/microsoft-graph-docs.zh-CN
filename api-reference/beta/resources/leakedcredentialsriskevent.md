---
title: leakedCredentialsRiskEvent 资源类型
description: 检测到的 Azure Active Directory 标识保护其中已帐户的凭据检测到的风险事件。 Azure AD 身份保护文档中，可以找到有关风险事件的完整信息。
localization_priority: Normal
ms.openlocfilehash: 7a8f2a8cf72b713fab30887fcc4d81b8a88e71ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815979"
---
# <a name="leakedcredentialsriskevent-resource-type"></a>leakedCredentialsRiskEvent 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

检测到的[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)其中已帐户的凭据检测到的风险事件。 [Azure AD 身份保护文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)中，可以找到有关风险事件的完整信息。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) | [leakedCredentialsRiskEvent](leakedcredentialsriskevent.md) |读取属性和 leakedCredentialsRiskEvent 对象的关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| 日期和时间的风险事件已关闭|
|createdDateTime|dateTimeOffset| 日期和时间的风险事件的创建。 始终是大于或等于风险事件本身的 datetime。 这是正确的属性，以用作筛选器时查询风险事件。|
|id|string| 只读|
|riskEventDateTime|dateTimeOffset| 日期和风险事件发生的时间|
|riskEventStatus|string| 可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。|
|riskLevel|string| 可取值为：`low`、`medium`、`high`。|
|riskEventType|string| 风险类型|
|userDisplayName|string| 风险的用户的名称|
|userId|string| 风险的用户 id|
|userPrincipalName|string| 风险的用户的用户主体名称|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |Description|
|:---------------|:--------|:----------|
|impactedUser|[用户](user.md)| 只读。可为 NULL。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "leakedCredentialsRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
