---
title: suspiciousIpRiskEvent 资源类型
description: Identity Protection 检测到的风险Azure Active Directory，其中帐户从可疑 IP 地址尝试登录。 有关风险事件的完整信息，请参阅 Azure AD Identity Protection 文档。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: 954f2e4f985371e8e19d97b880b7eaeef9c755cb
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547574"
---
# <a name="suspiciousipriskevent-resource-type-deprecated"></a>suspiciousIpRiskEvent 资源类型 (已弃) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
>**identityRiskEvents** API 已弃用，将在 2020 年 1 月 10 日停止返回数据。 有关详细信息，请参阅 [IdentityRiskEvents API 的弃用](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。

由 Azure Active Directory [Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection)检测到的风险事件，其中帐户从可疑 IP 地址尝试登录。 有关风险事件的完整信息，请参阅 [Azure AD Identity Protection 文档](/azure/active-directory/identity-protection/overview-identity-protection)。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 suspiciousIpRiskEvent](../api/suspiciousipriskevent-get.md) | [suspiciousIpRiskEvent](suspiciousipriskevent.md) |读取 suspiciousIpRiskEvent 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| 风险事件关闭的日期和时间|
|createdDateTime|dateTimeOffset| 创建风险事件的日期和时间。 这始终大于或等于风险事件本身的 datetime。 这是在查询风险事件时用作筛选器的正确属性。|
|id|string| 只读|
|ipAddress|string| 登录的 IP 地址|
|location|string| 附加到登录 IP 地址的位置|
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
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "ipAddress": "string",
  "location": "string",
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
  "description": "suspiciousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
