---
title: bookingAppointment 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 7ecd369607f260c8ebfd456ab7accaa0394e0af0
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696964"
---
# <a name="bookingappointment-resource-type"></a>bookingAppointment 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
表示由 Microsoft Bookings 业务提供的一组员工执行的 [bookingService](bookingservice.md)的客户约会。


## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出约会](../api/bookingbusiness-list-appointments.md) |  [bookingAppointment](bookingappointment.md) 集合 | 获取指定的 [bookingbusiness](../resources/bookingbusiness.md)中的 **bookingAppointment** 对象列表。 |
|[创建 bookingAppointment](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | 为指定的 **bookingbusiness 创建新的 bookingAppointment。** [](../resources/bookingbusiness.md) |
|[获取 bookingAppointment](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |读取 **bookingAppointment 对象的属性和** 关系。|
|[更新](../api/bookingappointment-update.md) | [bookingAppointment](bookingappointment.md)    |更新 **bookingAppointment** 对象。 |
|[删除](../api/bookingappointment-delete.md) | 无 |删除 **bookingAppointment** 对象。 |
|[Cancel](../api/bookingappointment-cancel.md)|无| 取消 **bookingAppointment** 对象。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|customerEmailAddress|String|预订约会 [的 bookingCustomer](bookingcustomer.md) 的 SMTP 地址。|
|customerId|String|此约会的 [bookingCustomer](bookingcustomer.md) 的 ID。 如果在创建约会时未指定任何 ID，则创建一个新的 **bookingCustomer** 对象。 设置后，你应考虑 **customerId** 不可变。|
|customerLocation|[location](location.md)|表示预订约会的 [bookingCustomer](bookingcustomer.md) 的位置信息。|
|customerName|String|客户的名称。|
|customerNotes|String|与此约会关联的客户的备注。 只有在通过 ID 读取 **此 bookingAppointment 时，才能** 获取该值。 <br> 只有在最初创建新客户的约会时，才能设置此属性。 此后，该值从 **customerId** 表示的客户计算。|
|customerPhone|字符串|客户的电话号码。|
|customerTimeZone|String|客户的时区。 有关可能值的列表，请参阅 [dateTimeTimeZone](datetimetimezone.md)。|
|duration|期限|约会的长度，以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。 |
|end|[dateTimeTimeZone](datetimetimezone.md)|约会结束的日期、时间和时区。|
|id|String| **bookingAppointment** 的 ID。 只读。|
|invoiceAmount|双精度|发票上的计费金额。|
|invoiceDate|[dateTimeTimeZone](datetimetimezone.md)|此约会的发票的日期、时间和时区。|
|invoiceId|String|发票的 ID。|
|invoiceStatus|string| 发票的状态。 可取值为：`draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。|
|invoiceUrl|String|Microsoft Bookings 中发票的 URL。|
|isLocationOnline|布尔值|如果为 True，则表明该约会将在线进行。 默认值为 false。|
|joinWebUrl|String|约会的在线会议 URL。|
|optOutOfCustomerEmail|布尔值|True 表示此约会的 [bookingCustomer](bookingcustomer.md) 不希望收到有关此约会的确认。|
|postBuffer|期限|例如，约会结束后要保留的清理时间量。 该值以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。 |
|preBuffer|期限|例如，在约会开始前保留准备的时间量。 该值以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。|
|price|双精度|指定 [bookingService](bookingservice.md)的约会的常规价格。|
|priceType|string| 为服务的定价结构提供灵活性的设置。 可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。|
|reminders|[bookingReminder](bookingreminder.md) 集合|为此约会发送的客户提醒集合。 此属性的值仅在按其 ID 读取此 **bookingAppointment** 时可用。|
|selfServiceAppointmentId|String|约会的附加跟踪 ID（如果约会是由客户直接在日程安排页面上创建的，而不是由员工代表客户创建的）。|
|服务 Id|String|与此约会关联的 [bookingService](bookingservice.md) 的 ID。|
|serviceLocation|[location](location.md)|服务交付位置。|
|serviceName|String|与此约会关联的 **bookingService** 的名称。<br>创建新约会时，此属性是可选的。 如果未指定，则通过 **serviceId** 属性从与约会关联的服务计算该约会。|
|serviceNotes|String|[bookingStaffMember 中的注释](bookingstaffmember.md)。 此属性的值仅在按其 ID 读取此 **bookingAppointment** 时可用。|
|smsNotificationsEnabled|布尔值|如果为 True，则表明将发送给客户进行约会的短信通知。 默认值为 false。|
|staffMemberIds|String collection|在此约会中 [安排的每个 bookingStaffMember](bookingstaffmember.md) 的 ID。|
|start|[dateTimeTimeZone](datetimetimezone.md)|约会开始的日期、时间和时区。|

## <a name="relationships"></a>关系
无


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
  "customerEmailAddress": "String",
  "customerId": "String",
  "customerLocation": {"@odata.type": "microsoft.graph.location"},
  "customerName": "String",
  "customerNotes": "String",
  "customerPhone": "String",
  "customerTimeZone": "String",
  "duration": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "id": "String (identifier)",
  "invoiceAmount": 1024,
  "invoiceDate": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "invoiceId": "String",
  "invoiceStatus": "string",
  "invoiceUrl": "String",
  "isLocationOnline": "Boolean",
  "joinWebUrl": "String",
  "optOutOfCustomerEmail": true,
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "price": 1024,
  "priceType": "string",
  "reminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "selfServiceAppointmentId": "String",
  "serviceId": "String",
  "serviceLocation": {"@odata.type": "microsoft.graph.location"},
  "serviceName": "String",
  "serviceNotes": "String",
  "smsNotificationsEnabled": "Boolean",
  "staffMemberIds": ["String"],
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
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


