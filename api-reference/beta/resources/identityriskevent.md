---
title: identityRiskEvent 资源类型
description: Azure Active Directory 标识保护检测到的风险事件。 它是每个特定风险事件类型的基本类型：
author: cloudhandler
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 47b8b7590be2d4b235bb04fe079b58cf65cb4ae7
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866789"
---
# <a name="identityriskevent-resource-type"></a>identityRiskEvent 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
>**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。 有关详细信息，请参阅[弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。

[Azure Active Directory 标识保护](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/)检测到的风险事件。 它是每个特定风险事件类型的基本类型：

| 事件类型         | 说明|
|:---------------|:-----------|
|[anonymousipRiskEvent](anonymousipriskevent.md) | 来自匿名 IP 地址的登录。 |
|[malwareRiskEvent](malwareriskevent.md) | 来自恶意软件感染的设备的登录。 |
|[impossibleTravelRiskEvent](impossibletravelriskevent.md) | 无法传播到非典型位置。 |
|[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md) | 凭据泄露的用户。 |
|[suspiciousIpRiskEvent](suspiciousipriskevent.md) | 来自可疑 IP 地址的登录。 |
|[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md) | 来自不熟悉位置的登录。 |

有关风险事件的完整信息，请参阅[AZURE AD Identity Protection 文档](/azure/active-directory/active-directory-reporting-risk-events)。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 identityRiskEvent](../api/identityriskevent-get.md) | [identityRiskEvent](identityriskevent.md) |读取 identityRiskEvent 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| 风险事件关闭的日期和时间|
|createdDateTime|dateTimeOffset| 风险事件的创建日期和时间。 此值始终大于或等于风险事件本身的日期时间。 这是查询风险事件时用作筛选器的正确属性。|
|id|字符串| 只读|
|riskEventDateTime|dateTimeOffset| 风险事件发生的日期和时间|
|riskEventStatus|string| 可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。|
|riskLevel|string| 可取值为：`low`、`medium`、`high`。|
|riskEventType|string| 风险的类型|
|userDisplayName|string| 具有风险的用户的名称|
|userId|string| 用户面临风险的 id|
|userPrincipalName|string| 用户面临风险的用户主体名称|

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
