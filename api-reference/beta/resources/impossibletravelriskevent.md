---
title: impossibleTravelRiskEvent 资源类型
description: 检测到的 Azure Active Directory 标识保护其中两个帐户登录发生从用户在典型的位置，并将不可能要登录宏的完整信息之间的工期中的位置之间的差旅风险事件Azure AD 身份保护文档中找不到风险事件。
localization_priority: Normal
ms.openlocfilehash: 517a09963570ce2c4a9e58edf7b73babaaff0426
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529381"
---
# <a name="impossibletravelriskevent-resource-type"></a>impossibleTravelRiskEvent 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检测到的[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)其中两个帐户登录发生从用户在典型的位置，并将不可能要登录宏完成之间的工期中的位置之间的差旅风险事件[Azure AD 身份保护文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)中，可以找到有关风险事件的信息。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) | [impossibleTravelRiskEvent](impossibletravelriskevent.md) |读取属性和 impossibleTravelRiskEvent 对象的关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| 日期和时间的风险事件已关闭|
|createdDateTime|dateTimeOffset| 日期和时间的风险事件的创建。 始终是大于或等于风险事件本身的 datetime。 这是正确的属性，以用作筛选器时查询风险事件。|
|deviceInformation|string| 有关设备的信息|
|id|string| 只读|
|ipAddress|string| IP 地址的第二个登录|
|isAtypicalLocation|布尔| 如果在位置之一是用户在典型|
|location|字符串| 挂接到第二个登录的 IP 地址的位置|
|previousIPAddress|string| 首次登录 IP 地址|
|previousLocation|string| 挂接到首次登录的 IP 地址的位置|
|previousSigninDateTime|dateTimeOffset| 日期和时间的首次登录|
|riskEventDateTime|dateTimeOffset| 日期和时间的第二个登录|
|riskEventStatus|string| 可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。|
|riskLevel|string| 可取值为：`low`、`medium`、`high`。|
|riskEventType|string| 风险类型|
|UserAgent|string| 浏览器的用户代理字符串|
|userDisplayName|string| 风险的用户的名称|
|userId|string| 风险的用户 id|
|userPrincipalName|string| 风险的用户的用户主体名称|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|impactedUser|[user](user.md)| 只读。可为 NULL。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "deviceInformation": "string",
  "id": "string (identifier)",
  "ipAddress": "string",
  "isAtypicalLocation": true,
  "location": "string",
  "previousIPAddress": "string",
  "previousLocation": "string",
  "previousSigninDateTime": "String (timestamp)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userAgent": "string",
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
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/impossibletravelriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
