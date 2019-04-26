---
title: locatedRiskEvent 资源类型
description: '基于位置数据的 Azure Active Directory 标识保护检测到的风险事件。 找到的风险事件类型包括:'
localization_priority: Normal
ms.openlocfilehash: 2c7503c08700a0d7c2d2ad67e8868901bdb008e2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345358"
---
# <a name="locatedriskevent-resource-type"></a>locatedRiskEvent 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

基于位置数据的[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)检测到的风险事件。 找到的风险事件类型包括:
* [来自匿名 IP 地址的登录](anonymousipriskevent.md)
* [来自受恶意软件感染的设备的登录](malwareriskevent.md)
* [无法移动到非常规位置](impossibletravelriskevent.md)
* [来自可疑 IP 地址的登录](suspiciousipriskevent.md)
* [来自不熟悉位置的登录](unfamiliarlocationriskevent.md)有关风险事件的完整信息, 请参阅[Azure AD Identity Protection 文档](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/)。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 locatedRiskEvent](../api/locatedriskevent-get.md) | [locatedRiskEvent](locatedriskevent.md) |读取 locatedRiskEvent 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| 风险事件关闭的日期和时间|
|createdDateTime|dateTimeOffset| 风险事件的创建日期和时间。 此值始终大于或等于风险事件本身的日期时间。 这是查询风险事件时用作筛选器的正确属性。|
|id|string| 只读|
|ipAddress|string| 登录的 IP 地址|
|location|string| 连接到登录 IP 地址的位置|
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
|impactedUser|[用户](user.md)| 只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "abstract": true,
   "keyProperty": "id",
   "baseType":"microsoft.graph.identityRiskEvent",
  "@odata.type": "microsoft.graph.locatedRiskEvent"
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
  "description": "locatedRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
