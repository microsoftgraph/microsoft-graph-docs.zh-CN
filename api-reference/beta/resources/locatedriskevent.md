---
title: locatedRiskEvent 资源类型
description: Azure Active Directory Identity Protection 根据位置数据检测到的风险事件。 定位的风险事件类型包括：
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: cloudhandler
ms.openlocfilehash: 902dc864ea16bd677d0499711faa078131ca015d
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469456"
---
# <a name="locatedriskevent-resource-type"></a>locatedRiskEvent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure [Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) 根据位置数据检测到的风险事件。 定位的风险事件类型包括：
* [从匿名 IP 地址登录](anonymousipriskevent.md)
* [来自感染了恶意软件的设备登录](malwareriskevent.md)
* [不可能到达非典型位置](impossibletravelriskevent.md)
* [从可疑 IP 地址登录](suspiciousipriskevent.md)
* [从不熟悉的位置登录](unfamiliarlocationriskevent.md) 有关风险事件的完整信息，请参阅 [Azure AD Identity Protection 文档](/azure/active-directory/identity-protection/overview-identity-protection)。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 locatedRiskEvent](../api/locatedriskevent-get.md) | [locatedRiskEvent](locatedriskevent.md) |读取 locatedRiskEvent 对象的属性和关系。|

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