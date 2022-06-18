---
title: bookingService 资源类型
description: 表示有关 bookingBusiness 提供的特定服务的信息，例如服务名称、价格以及通常提供此类服务的员工。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: d8c8fb849bbc452d343cb37b86e8cfae925606ae
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160704"
---
# <a name="bookingservice-resource-type"></a>bookingService 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
表示有关 [bookingBusiness](bookingbusiness.md) 提供的特定服务的信息，例如服务名称、价格以及通常提供此类服务的员工。

继承自 [bookingNamedEntity](bookingNamedEntity.md)。

## <a name="methods"></a>方法

| 方法           | 返回类型    |Description|
|:---------------|:--------|:----------|
|[列出服务](../api/bookingbusiness-list-services.md) | [bookingService](bookingservice.md) 集合 | 获取指定 [bookingbusiness](../resources/bookingbusiness.md) 中的 **bookingService** 对象列表。|
|[创建 bookingService](../api/bookingbusiness-post-services.md) | [bookingService](bookingservice.md) | 为指定的 [bookingBusiness](../resources/bookingbusiness.md) 创建 **bookingService**。 |
|[获取 bookingService](../api/bookingservice-get.md) | [bookingService](bookingservice.md) |获取指定 [bookingbusiness](../resources/bookingbusiness.md) 中 **bookingService** 对象的属性和关系。|
|[更新](../api/bookingservice-update.md) | 无   |更新指定 [bookingbusiness](../resources/bookingbusiness.md) 中的 **bookingService** 对象。 |
|[删除](../api/bookingservice-delete.md) | 无 |删除指定 [bookingbusiness](../resources/bookingbusiness.md) 中的 **bookingService** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|additionalInformation|String|确认约会时发送给客户的其他信息。|
|customQuestions|[bookingQuestionAssignment](../resources/bookingquestionassignment.md) 集合| 包含与特定服务关联的一组自定义问题。 |
|defaultDuration|期限|服务的默认长度，以天数、小时数、分钟数和秒数表示。 例如，P11D23H59M59.99999999999999999S。 |
|defaultLocation|[location](location.md)|服务的默认物理位置。|
|defaultPrice|双精度|服务的默认货币价格。|
|defaultPriceType|bookingPriceType|服务收费的默认方式。 可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`、`unknownFutureValue`。|
|defaultReminders|[bookingReminder](bookingreminder.md) 集合|此服务的约会的默认提醒集。 仅当按其 ID 读取此 **bookingService** 时，此属性的值才可用。|
|description|String|服务的文本说明。|
|displayName|String|服务名称。|
|id|String|该服务的 ID，采用 GUID 格式。 只读。|
|isAnonymousJoinEnabled|布尔|`True` 如果为此服务预订的约会生成 anonymousJoinWebUrl (webrtcUrl) 。
|isHiddenFromCustomers|布尔|True 表示此服务不可供客户预订。|
|isLocationOnline|布尔|True 表示服务的约会将联机进行。 默认值为 false。|
|languageTag|String|自助服务预订页的语言。
|maximumAttendeesCount|Int32|服务中允许的最大客户数。 如果服务 **的最大AttendeesCount** 大于 1，则在创建或更新约会时传递有效的客户 ID。  若要创建客户，请使用 [Create bookingCustomer](../api/bookingbusiness-post-customers.md) 操作。  |
|notes|String|有关此服务的其他信息。|
|postBuffer|期限|此服务的约会结束后和下一个客户约会可以预订之前的缓冲时间。|
|preBuffer|期限|此服务的约会开始之前的缓冲时间。|
|schedulePolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|一组策略，用于确定应如何创建和管理此类服务的约会。|
|smsNotificationsEnabled|布尔|True 表示可以向客户发送短信通知以进行服务的约会。 默认值为 false。|
|staffMemberIds|字符串集合|表示提供此服务 [的员工](bookingstaffmember.md) 。 |
|WebUrl|String|客户用于访问服务的 URL。|

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
  "additionalInformation": "String",
  "defaultDuration": "String (timestamp)",
  "defaultLocation": {"@odata.type": "microsoft.graph.location"},
  "defaultPrice": 1024,
  "defaultPriceType": {"@odata.type": "microsoft.graph.bookingPriceType"},
  "defaultReminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "languageTag": "String",
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
  "isAnonymousJoinEnabled": "Boolean",
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


