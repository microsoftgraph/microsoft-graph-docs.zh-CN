---
title: bookingService 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 53c5bc6be0953c68dc431be04b17f582715582c0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448365"
---
# <a name="bookingservice-resource-type"></a>bookingService 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
表示有关[bookingBusiness](bookingbusiness.md)提供的特定服务的信息，如服务名称、价格和通常提供此类服务的人员。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出服务](../api/bookingbusiness-list-services.md) | [bookingService](bookingservice.md)集合 | 获取指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingService**对象的列表。|
|[创建 bookingService](../api/bookingbusiness-post-services.md) | [bookingService](bookingservice.md) | 为指定的[bookingbusiness](../resources/bookingbusiness.md)创建**bookingService** 。 |
|[获取 bookingService](../api/bookingservice-get.md) | [bookingService](bookingservice.md) |获取指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingService**对象的属性和关系。|
|[更新](../api/bookingservice-update.md) | [bookingService](bookingservice.md)    |更新指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingService**对象。 |
|[删除](../api/bookingservice-delete.md) | 无 |删除指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingService**对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|defaultDuration|持续时间|服务的默认长度，以天数、小时数、分钟数和秒数表示。 例如，P11D23H59M 59.999999999999 S。 |
|defaultLocation|[位置](location.md)|服务的默认物理位置。|
|defaultPrice|双精度|服务的默认货币价格。|
|defaultPriceType|string|服务收费的默认方式。 可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。|
|defaultReminders|[bookingReminder](bookingreminder.md)集合|此服务的约会的默认提醒集。 此属性的值仅在按 ID 读取此**bookingService**时可用。|
|description|String|服务的文本说明。|
|displayName|字符串|服务名称。|
|emailAddress|String|电子邮件地址|
|id|字符串|该服务的 ID （采用 GUID 格式）。 只读。|
|isHiddenFromCustomers|Boolean|如果为 True，则表示此服务不可供客户预订。|
|notes|String|有关此服务的其他信息。|
|postBuffer|持续时间|此服务的约会结束后以及下一个客户约会可以被预订前要缓冲的时间。|
|preBuffer|持续时间|在此服务的约会开始之前要缓冲的时间。|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|确定应如何创建和管理此类服务的约会的一组策略。|
|staffMemberIds|String 集合|代表提供此服务的[教职员工成员](bookingstaffmember.md)。 |

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingService"
}-->

```json
{
  "defaultDuration": "String (timestamp)",
  "defaultLocation": {"@odata.type": "microsoft.graph.location"},
  "defaultPrice": 1024,
  "defaultPriceType": "string",
  "defaultReminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "description": "String",
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "isHiddenFromCustomers": true,
  "notes": "String",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "staffMemberIds": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
