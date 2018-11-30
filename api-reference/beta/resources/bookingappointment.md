---
title: bookingAppointment 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.openlocfilehash: d7ae5aa0a8a228bc4453742147ca9c858e093a8a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041868"
---
# <a name="bookingappointment-resource-type"></a>bookingAppointment 资源类型

 > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。
 
代表[bookingService](bookingservice.md)，由一组人员成员，由 Microsoft 预订业务执行客户约会。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列表约会](../api/bookingbusiness-list-appointments.md) |  [bookingAppointment](bookingappointment.md)集合 | 指定[bookingbusiness](../resources/bookingbusiness.md)中获取**bookingAppointment**对象的列表。 |
|[创建 bookingAppointment](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | 创建新**bookingAppointment**的指定[bookingbusiness](../resources/bookingbusiness.md)。 |
|[获取 bookingAppointment](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |读取的属性和**bookingAppointment**对象的关系。|
|[Update](../api/bookingappointment-update.md) | [bookingAppointment](bookingappointment.md)    |更新**bookingAppointment**对象。 |
|[删除](../api/bookingappointment-delete.md) | 无 |删除**bookingAppointment**对象。 |
|[取消](../api/bookingappointment-cancel.md)|无| 取消**bookingAppointment**对象。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|customerEmailAddress|字符串|预订约会[bookingCustomer](bookingcustomer.md) SMTP 地址。|
|customerId|字符串|该约会的[bookingCustomer](bookingcustomer.md)的 ID。 如果未指定 ID 创建约会时，将创建一个新的**bookingCustomer**对象。 设置后，您应考虑**customerId**变。|
|customerLocation|[location](location.md)|代表[bookingCustomer](bookingcustomer.md)预订约会的位置信息。|
|customerName|字符串|客户的名称。|
|customerNotes|字符串|从与此约会关联的客户的备注。 您可以获取仅当读取此**bookingAppointment**其 id 值 <br> 仅在最初使用新的客户创建约会时，您可以设置该属性。 此时，从由**customerId**客户计算的值。|
|customerPhone|字符串|客户的电话号码。|
|duration|Duration|约会中[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式的长度。 |
|end|[dateTimeTimeZone](datetimetimezone.md)|日期、 时间和约会的结束的时区。|
|id|字符串| **BookingAppointment**的 ID。 只读。|
|invoiceAmount|双精度数|记帐的发票量。|
|invoiceDate|[dateTimeTimeZone](datetimetimezone.md)|日期、 时间和此约会的发票的时区。|
|invoiceId|字符串|发票的 ID。|
|invoiceStatus|string| 发票的状态。 可取值为：`draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。|
|invoiceUrl|字符串|在 Microsoft 预订发票的 URL。|
|optOutOfCustomerEmail|布尔|True 表示该约会的[bookingCustomer](bookingcustomer.md)不希望接收该约会的确认。|
|后|Duration|保留后的清理，例如约会结束的时间量。 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示的值。 |
|缓冲区|Duration|保留之前的准备，例如约会开始的时间量。 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示的值。|
|价格|双精度数|指定[bookingService](bookingservice.md)约会正则价格。|
|priceType|string| 为服务定价结构提供灵活性设置。 可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。|
|提醒|[bookingReminder](bookingreminder.md)集合|客户提醒发送该约会的集合。 此属性的值时，可仅读取此**bookingAppointment**由其 id。|
|selfServiceAppointmentId|字符串|约会，如果约会的已创建直接通过计划页上的客户而不是由员工成员客户替的其他跟踪 ID。|
|服务 Id|字符串|与此约会相关联的[bookingService](bookingservice.md) ID。|
|serviceLocation|[location](location.md)|传递服务的位置的位置。|
|serviceName|字符串|与此约会关联**bookingService**的名称。<br>创建一个新的约会时，此属性是可选的。 如果未指定，它是从与约会**serviceId**属性关联的服务进行计算。|
|serviceNotes|字符串|从[bookingStaffMember](bookingstaffmember.md)备注。 此属性的值时，可仅读取此**bookingAppointment**由其 id。|
|staffMemberIds|String 集合|每个[bookingStaffMember](bookingstaffmember.md)此约会中安排的 ID。|
|start|[dateTimeTimeZone](datetimetimezone.md)|日期、 时间和时区约会的开始。|

## <a name="relationships"></a>Relationships
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
  "duration": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "id": "String (identifier)",
  "invoiceAmount": 1024,
  "invoiceDate": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "invoiceId": "String",
  "invoiceStatus": "string",
  "invoiceUrl": "String",
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
  "staffMemberIds": ["String"],
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingAppointment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->