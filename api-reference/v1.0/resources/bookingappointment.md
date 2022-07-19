---
title: bookingAppointment 资源类型
description: 表示一个 bookingService 的客户约会，由一组工作人员执行，由Microsoft Bookings企业提供。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 20b466b734ef0f91445e950e3bfee173758e4b0d
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856314"
---
# <a name="bookingappointment-resource-type"></a>bookingAppointment 资源类型

命名空间：microsoft.graph
 
表示一个 [bookingService](bookingservice.md) 的客户约会，由一组工作人员执行，由Microsoft Bookings业务提供。

> [!NOTE]
> 如果使用应用程序权限创建自定义应用，则必须遵循 [业务规则验证](/graph/bookingsbusiness-business-rules)。

## <a name="methods"></a>方法

| 方法           | 返回类型    |Description|
|:---------------|:--------|:----------|
|[列出约会](../api/bookingbusiness-list-appointments.md) |  [bookingAppointment](bookingappointment.md) 集合 | 获取指定 [bookingbusiness](bookingbusiness.md) 中的 **bookingAppointment** 对象列表。 |
|[创建 bookingAppointment](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | 为指定的 [bookingbusiness](bookingbusiness.md) 创建新的 **bookingAppointment**。 |
|[获取 bookingAppointment](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |读取 **bookingAppointment** 对象的属性和关系。|
|[更新](../api/bookingappointment-update.md) | [bookingAppointment](bookingappointment.md)    |更新 **bookingAppointment** 对象。 |
|[删除](../api/bookingappointment-delete.md) | 无 |删除 **bookingAppointment** 对象。 |
|[Cancel](../api/bookingappointment-cancel.md)|无| 取消 **bookingAppointment** 对象。|

## <a name="properties"></a>属性

| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|additionalInformation|String|确认约会时发送给客户的其他信息。|
|客户|[bookingCustomerInformation](bookingcustomerinformation.md) 集合|它列出了约会的客户属性。 约会将包含客户信息列表，每个单位将指示属于该约会的客户的属性。 可选。|
|customerTimeZone|String|客户的时区。 有关可能值的列表，请参阅 [dateTimeTimeZone](datetimetimezone.md)。|
|duration|持续时间|约会的长度，以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。 |
|endDateTime|[dateTimeTimeZone](datetimetimezone.md)|约会结束的日期、时间和时区。|
|filledAttendeesCount|Int32|约会中的当前客户数 |
|id|String| **bookingAppointment** 的 ID。 只读。|
|isLocationOnline|Boolean|如果 `true`指示约会将联机进行。 默认值为 `false`。|
|joinWebUrl|String|约会的联机会议的 URL。|
|maximumAttendeesCount|Int32|约会中允许的最大客户数。 如果服务 **的最大AttendeesCount** 大于 1，则在创建或更新约会时传递有效的客户 ID。 若要创建客户，请使用 [Create bookingCustomer](../api/bookingbusiness-post-customers.md) 操作。 |
|optOutOfCustomerEmail|Boolean|如果 `true` 指示此约会的 [bookingCustomer](bookingcustomer.md) 不希望收到此约会的确认。|
|postBuffer|持续时间|例如，约会结束后要保留的时间，用于清理。 该值以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。 |
|preBuffer|持续时间|例如，在约会开始之前，为准备而保留的时间量。 该值以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。|
|价格|双精度|指定 [bookingService](bookingservice.md) 的约会的常规价格。|
|priceType|bookingPriceType| 一个设置，用于为服务的定价结构提供灵活性。 可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`、`unknownFutureValue`。|
|提醒|[bookingReminder](bookingreminder.md) 集合|为此约会发送的客户提醒的集合。 仅当按其 ID 读取此 **bookingAppointment** 时，此属性的值才可用。|
|selfServiceAppointmentId|String|如果约会是由客户直接在计划页上创建的，而不是由代表客户的工作人员创建的，则为约会提供额外的跟踪 ID。 仅当 maxAttendeeCount 为 1 时才支持约会。|
|服务 Id|String|与此约会关联的 [bookingService](bookingservice.md) 的 ID。|
|serviceLocation|[location](location.md)|服务的传送位置。|
|serviceName|String|与此约会关联的 **bookingService** 的名称。<br>创建新约会时，此属性是可选的。 如果未指定，则会从 **ServiceId** 属性与约会关联的服务中进行计算。|
|serviceNotes|String|[bookingStaffMember](bookingstaffmember.md) 中的备注。 仅当按其 ID 读取此 **bookingAppointment** 时，此属性的值才可用。|
|smsNotificationsEnabled|Boolean|如果 `true`指示 SMS 通知将发送给客户进行约会。 默认值为 `false`。|
|staffMemberIds|字符串集合|此约会中计划的每位 [bookingStaffMember](bookingstaffmember.md) 的 ID。|
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