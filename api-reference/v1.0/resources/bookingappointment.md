---
title: bookingAppointment 资源类型
description: 表示由 Microsoft Bookings 业务提供的一组员工执行的 bookingService 的客户约会。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: c5e301d6ef48015feb417bf663709fd4024a3c4e
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367613"
---
# <a name="bookingappointment-resource-type"></a>bookingAppointment 资源类型

命名空间：microsoft.graph
 
表示由 Microsoft Bookings 业务提供的一组员工执行的 [bookingService](bookingservice.md) 的客户约会。


## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出约会](../api/bookingbusiness-list-appointments.md) |  [bookingAppointment](bookingappointment.md) 集合 | 获取指定 **bookingBusiness 中的 bookingAppointment** 对象 [列表](../resources/bookingbusiness.md)。 |
|[创建 bookingAppointment](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | 为指定的 [bookingBusiness](../resources/bookingbusiness.md) 创建新的 **bookingAppointment**。 |
|[获取 bookingAppointment](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |读取 **bookingAppointment 对象的属性和** 关系。|
|[更新](../api/bookingappointment-update.md) | [bookingAppointment](bookingappointment.md)    |更新 **bookingAppointment** 对象。 |
|[删除](../api/bookingappointment-delete.md) | 无 |删除 **bookingAppointment** 对象。 |
|[Cancel](../api/bookingappointment-cancel.md)|无| 取消 **bookingAppointment** 对象。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|additionalInformation|String|确认约会时发送给客户的其他信息。|
|customers|[bookingCustomerInformation](../resources/bookingcustomerinformation.md) 集合|它向下列出了约会的客户属性。 约会将包含客户信息列表，每个单元将指示属于该约会的客户的属性。 可选。|
|customerTimeZone|String|客户的时区。 有关可能值的列表，请参阅 [dateTimeTimeZone](datetimetimezone.md)。|
|duration|期限|约会的长度，以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。 |
|endDateTime|[dateTimeTimeZone](datetimetimezone.md)|约会结束的日期、时间和时区。|
|filledAttendeesCount|Int32|约会中的当前客户数 |
|id|String| **bookingAppointment 的** ID。 只读。|
|isLocationOnline|Boolean|如果 `true`为 ，则指示约会将联机进行。 默认值为 `false`。|
|joinWebUrl|String|约会的在线会议 URL。|
|maximumAttendeesCount|Int32|约会中允许的最大客户数。 如果 **服务的 maximumAttendeesCount** 大于 1，在创建或更新约会时传递有效的客户 ID。 若要创建客户，请使用 [创建 bookingCustomer](../api/bookingbusiness-post-customers.md) 操作。 |
|optOutOfCustomerEmail|Boolean|如果 `true` 指示此约会的 [bookingCustomer](bookingcustomer.md) 不希望收到有关此约会的确认。|
|postBuffer|期限|例如，约会结束后要保留的清理时间量。 该值以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。 |
|preBuffer|期限|例如，在约会开始前保留准备的时间量。 该值以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。|
|price|双精度|指定 [bookingService](bookingservice.md) 的约会的常规价格。|
|priceType|bookingPriceType| 为服务的定价结构提供灵活性的设置。 可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`、`unknownFutureValue`。|
|reminders|[bookingReminder](bookingreminder.md) 集合|为此约会发送的客户提醒集合。 此属性的值仅在按其 ID 读取 **此 bookingAppointment** 时可用。|
|selfServiceAppointmentId|String|约会的附加跟踪 ID（如果约会是由客户直接在日程安排页面上创建的，而不是由员工代表客户创建的）。 仅在 maxAttendeeCount 为 1 时才支持约会。|
|服务 Id|String|与此约会关联的 [bookingService](bookingservice.md) 的 ID。|
|serviceLocation|[location](location.md)|服务交付位置。|
|serviceName|String|与此约会 **关联的 bookingService** 的名称。<br>创建新约会时，此属性是可选的。 如果未指定，则通过 **serviceId** 属性从与约会关联的服务计算该约会。|
|serviceNotes|字符串|[bookingStaffMember 中的注释](bookingstaffmember.md)。 此属性的值仅在按其 ID 读取 **此 bookingAppointment** 时可用。|
|smsNotificationsEnabled|Boolean|如果 `true`为 ，表示将发送给客户进行约会的短信通知。 默认值为 `false`。|
|staffMemberIds|String 集合|在此约会中 [安排的每个 bookingStaffMember](bookingstaffmember.md) 的 ID。|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|约会开始的日期、时间和时区。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingAppointment"
}-->

```json
{
  "customers": [
    {
      "@odata.type": "microsoft.graph.bookingCustomerInformation"
    }
  ],
  "duration": "String (timestamp)",
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "id": "String (identifier)",
  "isLocationOnline": "Boolean",
  "joinWebUrl": "String",
  "optOutOfCustomerEmail": "Boolean",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "price": "Integer",
  "priceType": {"@odata.type": "microsoft.graph.bookingPriceType"},
  "reminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "selfServiceAppointmentId": "String",
  "serviceId": "String",
  "serviceLocation": {"@odata.type": "microsoft.graph.location"},
  "serviceName": "String",
  "serviceNotes": "String",
  "smsNotificationsEnabled": "Boolean",
  "staffMemberIds": ["String"],
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "maximumAttendeesCount": "Integer",
  "filledAttendeesCount": "Integer"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingAppointment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


