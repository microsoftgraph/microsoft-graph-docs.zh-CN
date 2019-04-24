---
title: identityRiskEvent 资源类型
description: 'Azure Active Directory 标识保护检测到的风险事件。 它是每个特定风险事件类型的基本类型:'
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: b5c36ab898805c0638cc199ff8cfb893444f04ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506389"
---
# <a name="identityriskevent-resource-type"></a>identityRiskEvent 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)检测到的风险事件。 它是每个特定风险事件类型的基本类型:

| 事件类型         | 说明|
|:---------------|:-----------|
|[anonymousipRiskEvent](anonymousipriskevent.md) | 来自匿名 IP 地址的登录。 |
|[malwareRiskEvent](malwareriskevent.md) | 来自恶意软件感染的设备的登录。 |
|[impossibleTravelRiskEvent](impossibletravelriskevent.md) | 无法传播到非典型位置。 |
|[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md) | 凭据泄露的用户。 |
|[suspiciousIpRiskEvent](suspiciousipriskevent.md) | 来自可疑 IP 地址的登录。 |
|[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md) | 来自不熟悉位置的登录。 |

有关风险事件的完整信息, 请参阅[Azure AD Identity Protection 文档](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events)。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 identityRiskEvent](../api/identityriskevent-get.md) | [identityRiskEvent](identityriskevent.md) |读取 identityRiskEvent 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| 风险事件关闭的日期和时间|
|createdDateTime|dateTimeOffset| 风险事件的创建日期和时间。 此值始终大于或等于风险事件本身的日期时间。 这是查询风险事件时用作筛选器的正确属性。|
|id|string| 只读|
|riskEventDateTime|dateTimeOffset| 风险事件发生的日期和时间|
|riskEventStatus|字符串| 可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。|
|riskLevel|string| 可取值为：`low`、`medium`、`high`。|
|riskEventType|字符串| 风险的类型|
|userDisplayName|字符串| 具有风险的用户的名称|
|userId|字符串| 用户面临风险的 id|
|userPrincipalName|字符串| 用户面临风险的用户主体名称|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|impactedUser|[用户](user.md)| 只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。 

<!-- {
  "blockType": "resource",
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
  "userPrincipalName": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/identityriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
