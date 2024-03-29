---
title: bookingService 资源类型
description: 表示有关 bookingBusiness 提供的特定服务的信息，例如服务名称、价格和通常提供此类服务的员工。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 7a9c45bc79c71b3a35be7e07ef3ab4dcc9365ba0
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63368236"
---
# <a name="bookingservice-resource-type"></a>bookingService 资源类型

命名空间：microsoft.graph
 
表示有关 [bookingBusiness](bookingbusiness.md) 提供的特定服务的信息，例如服务名称、价格和通常提供此类服务的员工。

## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出服务](../api/bookingbusiness-list-services.md) | [bookingService](bookingservice.md) 集合 | 获取指定 [bookingbusiness 中的 bookingService 对象列表](../resources/bookingbusiness.md)。|
|[创建 bookingService](../api/bookingbusiness-post-services.md) | [bookingService](bookingservice.md) | 为指定的  [bookingbusiness 创建 bookingService](../resources/bookingbusiness.md)。 |
|[获取 bookingService](../api/bookingservice-get.md) | [bookingService](bookingservice.md) |获取指定 **bookingbusiness 中的 bookingService** 对象 [的属性和关系](../resources/bookingbusiness.md)。|
|[更新](../api/bookingservice-update.md) | [bookingService](bookingservice.md)    |更新 **指定** [bookingbusiness 中的 bookingService 对象](../resources/bookingbusiness.md)。 |
|[删除](../api/bookingservice-delete.md) | 无 |删除 **指定** [bookingbusiness 中的 bookingService 对象](../resources/bookingbusiness.md)。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|additionalInformation|String|确认约会时发送给客户的其他信息。|
|customQuestions|[bookingQuestionAssignment](../resources/bookingquestionassignment.md) 集合| 包含与特定服务关联的一组自定义问题。 |
|defaultDuration|期限|服务的默认长度，以天数、小时数、分钟数和秒数表示。 例如，P11D23H59M59.9999999999S。 |
|defaultLocation|[location](location.md)|服务的默认物理位置。|
|defaultPrice|双精度|服务的默认货币价格。|
|defaultPriceType|bookingPriceType|服务收费的默认方式。 可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`、`unknownFutureValue`。|
|defaultReminders|[bookingReminder](bookingreminder.md) 集合|此服务约会的默认提醒集。 此属性的值仅在按其 ID 读取 **此 bookingService** 时可用。|
|说明|String|服务的文本说明。|
|displayName|String|服务名称。|
|id|String|该服务的 ID，采用 GUID 格式。 只读。|
|isHiddenFromCustomers|Boolean|True 表示客户无法预订此服务。|
|isLocationOnline|Boolean|如果为 True，则表明该服务的约会将联机进行。 默认值为 false。|
|maximumAttendeesCount|Int32|服务中允许的最大客户数。 如果 **服务的 maximumAttendeesCount** 大于 1，在创建或更新约会时传递有效的客户 ID。 若要创建客户，请使用 [创建 bookingCustomer](../api/bookingbusiness-post-customers.md) 操作。 |
|notes|String|有关此服务的其他信息。|
|postBuffer|期限|此服务的约会结束后以及下一个客户约会可以预订之前进行缓冲的时间。|
|preBuffer|期限|在此服务的约会可以启动之前缓冲的时间。|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|用于确定如何创建和管理这种类型的服务的约会的策略集。|
|smsNotificationsEnabled|Boolean|如果为 True，则表明可以针对服务约会将短信通知发送给客户。 默认值为 false。|
|staffMemberIds|String 集合|表示 [提供此服务](bookingstaffmember.md) 的员工。 |
|webUrl|String|客户用于访问服务的 URL。|

## <a name="relationships"></a>关系
无。


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
  "additionalInformation": "String",
  "defaultDuration": "String (timestamp)",
  "defaultLocation": {"@odata.type": "microsoft.graph.location"},
  "defaultPrice": 1024,
  "defaultPriceType": {"@odata.type": "microsoft.graph.bookingPriceType"},
  "defaultReminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isHiddenFromCustomers": true,
  "isLocationOnline": "Boolean",
  "notes": "String",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "smsNotificationsEnabled": "Boolean",
  "staffMemberIds": ["String"],
  "customQuestions": [
    {
      "@odata.type": "microsoft.graph.bookingQuestionAssignment"
    }
  ],
  "maximumAttendeesCount": "Integer",
  "webUrl": "String"
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


