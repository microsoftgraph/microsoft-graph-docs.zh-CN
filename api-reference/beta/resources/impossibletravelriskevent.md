---
title: impossibleTravelRiskEvent 资源类型
description: 由 Azure Active Directory Identity Protection 检测到的风险事件，其中两个帐户登录发生在用户非典型位置，在两次登录之间的持续时间内，无法在这两个位置之间进行。有关风险事件的完整信息，请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: e05760bc4e3c60d3d4079965cdf01b0d5f630a77
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547006"
---
# <a name="impossibletravelriskevent-resource-type-deprecated"></a>impossibleTravelRiskEvent 资源类型 (弃用) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
>**identityRiskEvents** API 已弃用，将在 2020 年 1 月 10 日停止返回数据。 有关详细信息，请参阅 [IdentityRiskEvents API 的弃用](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。

[由 Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection)检测到的风险事件，其中两个帐户登录发生在用户非典型位置，在两次登录之间的持续时间内，无法在这两个位置之间旅行。有关风险事件的完整信息，请参阅[Azure AD Identity Protection 文档](/azure/active-directory/identity-protection/overview-identity-protection)。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) | [impossibleTravelRiskEvent](impossibletravelriskevent.md) |读取 impossibleTravelRiskEvent 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| 风险事件关闭的日期和时间|
|createdDateTime|dateTimeOffset| 创建风险事件的日期和时间。 这始终大于或等于风险事件本身的 datetime。 这是在查询风险事件时用作筛选器的正确属性。|
|deviceInformation|string| 有关设备的信息|
|id|string| 只读|
|ipAddress|string| 第二次登录的 IP 地址|
|isAtypicalLocation|boolean| 如果其中一个位置对于用户来说不是典型位置|
|location|string| 附加到第二次登录的 IP 地址的位置|
|previousIPAddress|string| 首次登录的 IP 地址|
|previousLocation|string| 附加到首次登录的 IP 地址的位置|
|previousSigninDateTime|dateTimeOffset| 首次登录的日期和时间|
|riskEventDateTime|dateTimeOffset| 第二次登录的日期和时间|
|riskEventStatus|string| 可取值为：`active`、`remediated`、`dismissedAsFixed`、`dismissedAsFalsePositive`、`dismissedAsIgnore`、`loginBlocked`、`closedMfaAuto`、`closedMultipleReasons`。|
|riskLevel|string| 可取值为：`low`、`medium`、`high`。|
|riskEventType|string| 风险类型|
|userAgent|string| 浏览器的用户代理字符串|
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
