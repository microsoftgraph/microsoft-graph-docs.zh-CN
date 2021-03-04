---
title: identityRiskEvent 资源类型
description: Azure Active Directory Identity Protection 检测到的风险事件。 它是每个特定风险事件类型的基类型：
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: acb48ce5ef63abf5ec2a09d8a3365a744bb8a668
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440288"
---
# <a name="identityriskevent-resource-type-deprecated"></a>identityRiskEvent 资源类型 (已弃) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
>**identityRiskEvents** API 已弃用，将在 2020 年 1 月 10 日停止返回数据。 有关详细信息，请参阅 [IdentityRiskEvents API 的弃用](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。

Azure [Active Directory Identity Protection 检测到的风险事件](/azure/active-directory/identity-protection/overview-identity-protection)。 它是每个特定风险事件类型的基类型：

| 事件类型         | 说明|
|:---------------|:-----------|
|[anonymousipRiskEvent](anonymousipriskevent.md) | 从匿名 IP 地址登录。 |
|[malwareRiskEvent](malwareriskevent.md) | 从受恶意软件感染的设备登录。 |
|[impossibleTravelRiskEvent](impossibletravelriskevent.md) | 无法到达非典型位置。 |
|[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md) | 凭据泄露的用户。 |
|[suspiciousIpRiskEvent](suspiciousipriskevent.md) | 从可疑 IP 地址登录。 |
|[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md) | 从不熟悉的位置登录。 |

有关风险事件的完整信息，请参阅 [Azure AD Identity Protection 文档](/azure/active-directory/active-directory-reporting-risk-events)。

## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 identityRiskEvent](../api/identityriskevent-get.md) | [identityRiskEvent](identityriskevent.md) |读取 identityRiskEvent 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| 风险事件关闭的日期和时间|
|createdDateTime|dateTimeOffset| 创建风险事件的日期和时间。 这始终大于或等于风险事件本身的日期时间。 这是在查询风险事件时用作筛选器的正确属性。|
|id|string| 只读|
|riskEventDateTime|dateTimeOffset| 发生风险事件的日期和时间|
|riskEventStatus|string| 可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。|
|riskLevel|string| 可取值为：`low`、`medium`、`high`。|
|riskEventType|string| 风险类型|
|userDisplayName|string| 处于风险中的用户的名称|
|userId|string| 处于风险中的用户的 ID|
|userPrincipalName|string| 处于风险中的用户的用户主体名称|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|impactedUser|[user](user.md)| 只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identityRiskEvent"
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
  "userPrincipalName": "string",
  "riskEventType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
