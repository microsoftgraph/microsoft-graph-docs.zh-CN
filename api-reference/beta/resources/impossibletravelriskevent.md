---
title: impossibleTravelRiskEvent 资源类型
description: Azure Active Directory 标识保护检测到的风险事件, 其中两个帐户登录从用户的非典型位置发生, 并且在登录之间的持续时间之间无法进行移动。有关详细信息, 请参阅可在 Azure AD Identity Protection 文档中找到风险事件。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2b66755924022b4fa30637cc8e97c4f944ad2d79
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005770"
---
# <a name="impossibletravelriskevent-resource-type"></a>impossibleTravelRiskEvent 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)检测到的风险事件, 其中两个帐户登录从用户的非典型位置发生, 并且在登录之间的持续时间之间无法进行移动。完成有关风险事件的信息可以在[AZURE AD Identity Protection 文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)中找到。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) | [impossibleTravelRiskEvent](impossibletravelriskevent.md) |读取 impossibleTravelRiskEvent 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| 风险事件关闭的日期和时间|
|createdDateTime|dateTimeOffset| 风险事件的创建日期和时间。 此值始终大于或等于风险事件本身的日期时间。 这是查询风险事件时用作筛选器的正确属性。|
|deviceInformation|string| 有关设备的信息|
|id|string| 只读|
|ipAddress|string| 第二次登录的 IP 地址|
|isAtypicalLocation|boolean| 如果其中一个位置对用户是典型的|
|location|string| 连接到第二次登录的 IP 地址的位置|
|previousIPAddress|string| 第一次登录的 IP 地址|
|previousLocation|string| 第一次登录的 IP 地址所连接的位置|
|previousSigninDateTime|dateTimeOffset| 首次登录的日期和时间|
|riskEventDateTime|dateTimeOffset| 第二次登录的日期和时间|
|riskEventStatus|string| 可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。|
|riskLevel|string| 可取值为：`low`、`medium`、`high`。|
|riskEventType|string| 风险的类型|
|userAgent|string| 浏览器的用户代理字符串|
|userDisplayName|string| 具有风险的用户的名称|
|userId|string| 用户面临风险的 id|
|userPrincipalName|string| 用户面临风险的用户主体名称|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|impactedUser|[用户](user.md)| 只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
  "userPrincipalName": "string",
  "riskEventType": "string"
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
  "suppressions": []
}
-->
