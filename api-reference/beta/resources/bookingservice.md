---
title: bookingService 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 790adf49cfda1f787665a48e1b06bd77da27e1f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925159"
---
# <a name="bookingservice-resource-type"></a>bookingService 资源类型

 > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。
 
代表由[bookingBusiness](bookingbusiness.md)，如的服务名称、 价格和通常提供了此类服务的人员提供的特定服务的信息。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列表服务](../api/bookingbusiness-list-services.md) | [bookingService](bookingservice.md)集合 | 指定[bookingbusiness](../resources/bookingbusiness.md)中获取**bookingService**对象的列表。|
|[创建 bookingService](../api/bookingbusiness-post-services.md) | [bookingService](bookingservice.md) | 创建用于指定[bookingbusiness](../resources/bookingbusiness.md) **bookingService** 。 |
|[获取 bookingService](../api/bookingservice-get.md) | [bookingService](bookingservice.md) |指定[bookingbusiness](../resources/bookingbusiness.md)中获取的属性和**bookingService**对象的关系。|
|[更新](../api/bookingservice-update.md) | [bookingService](bookingservice.md)    |更新中指定[bookingbusiness](../resources/bookingbusiness.md) **bookingService**对象。 |
|[删除](../api/bookingservice-delete.md) | 无 |删除在指定[bookingbusiness](../resources/bookingbusiness.md) **bookingService**对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|defaultDuration|Duration|默认服务中的天、 小时、 分钟和秒数字表示的长度。 例如，P11D23H59M59.999999999999S。 |
|defaultLocation|[location](location.md)|服务的默认物理位置。|
|defaultPrice|Double|该服务默认货币价格。|
|defaultPriceType|string|负责服务的默认方式。 可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。|
|defaultReminders|[bookingReminder](bookingreminder.md)集合|默认设置的该服务的约会的提醒。 此属性的值时，可仅读取此**bookingService**由其 id。|
|说明|字符串|服务的文本说明。|
|displayName|字符串|服务名称。|
|emailAddress|String|电子邮件地址|
|id|字符串|该服务，以 GUID 格式的 ID。 只读。|
|isHiddenFromCustomers|Boolean|True 表示该服务不是预定的客户。|
|notes|String|有关此服务的其他信息。|
|后|Duration|此服务的时间为缓冲区之后为约会结束，且在下一步之前客户约会可以为预约。|
|缓冲区|Duration|缓冲区之前可以启动此服务的约会的时间。|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|确定如何创建和管理服务此类型的约会的策略集。|
|staffMemberIds|String 集合|表示这些[员工](bookingstaffmember.md)提供此服务。 |

## <a name="relationships"></a>Relationships
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
<!-- {
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
