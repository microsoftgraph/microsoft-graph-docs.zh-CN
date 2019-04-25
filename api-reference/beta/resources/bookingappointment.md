---
title: bookingAppointment 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c5868788159f0602c1f8a263138c7ce9107c2c94
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535502"
---
# <a name="bookingappointment-resource-type"></a>bookingAppointment 资源类型

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
表示由 Microsoft 记帐业务提供的一组员工执行的[bookingService](bookingservice.md)的客户约会。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出约会](../api/bookingbusiness-list-appointments.md) |  [bookingAppointment](bookingappointment.md)集合 | 获取指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingAppointment**对象的列表。 |
|[创建 bookingAppointment](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | 为指定的[bookingbusiness](../resources/bookingbusiness.md)创建新的**bookingAppointment** 。 |
|[获取 bookingAppointment](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |读取**bookingAppointment**对象的属性和关系。|
|[更新](../api/bookingappointment-update.md) | [bookingAppointment](bookingappointment.md)    |更新**bookingAppointment**对象。 |
|[删除](../api/bookingappointment-delete.md) | 无 |删除**bookingAppointment**对象。 |
|[Cancel](../api/bookingappointment-cancel.md)|无| 取消**bookingAppointment**对象。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|customerEmailAddress|String|预订约会的[bookingCustomer](bookingcustomer.md)的 SMTP 地址。|
|customerId|String|此约会的[bookingCustomer](bookingcustomer.md)的 ID。 如果创建约会时未指定 ID, 则会创建一个新的**bookingCustomer**对象。 设置后, 应考虑**customerId**不可变。|
|customerLocation|[location](location.md)|表示预订约会的[bookingCustomer](bookingcustomer.md)的位置信息。|
|customerName|String|客户的名称。|
|customerNotes|String|来自与此约会相关联的客户的注释。 仅当按 ID 读取此**bookingAppointment**时, 才能获取该值。 <br> 只有在最初创建新客户的约会时, 才能设置该属性。 然后, 将从**customerId**表示的客户计算该值。|
|customerPhone|String|客户的电话号码。|
|duration|持续时间|约会的长度, 以[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示。 |
|end|[dateTimeTimeZone](datetimetimezone.md)|约会结束的日期、时间和时区。|
|id|String| **bookingAppointment**的 ID。 只读。|
|invoiceAmount|双精度|发票上的计费金额。|
|invoiceDate|[dateTimeTimeZone](datetimetimezone.md)|此约会的发票的日期、时间和时区。|
|invoiceId|String|发票的 ID。|
|invoiceStatus|string| 发票的状态。 可取值为：`draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。|
|invoiceUrl|String|Microsoft 预订中发票的 URL。|
|optOutOfCustomerEmail|布尔值|如果为 True, 则表示此约会的[bookingCustomer](bookingcustomer.md)不希望收到此约会的确认。|
|postBuffer|持续时间|在约会结束后保留的时间长度, 例如, 进行清理。 值以[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示。 |
|preBuffer|持续时间|在约会开始之前保留的时间量 (以供准备) 为例。 值以[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示。|
|特价|双精度|指定[bookingService](bookingservice.md)的约会的常规价格。|
|priceType|string| 一种设置, 可为服务的定价结构提供灵活性。 可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。|
|提醒|[bookingReminder](bookingreminder.md)集合|为此约会发送的客户提醒的集合。 此属性的值仅在按 ID 读取此**bookingAppointment**时可用。|
|selfServiceAppointmentId|String|约会的其他跟踪 ID, 如果约会是由客户在日程安排页面上直接创建的, 而不是代表客户由教职员工成员创建的。|
|服务 Id|String|与此约会相关联的[bookingService](bookingservice.md)的 ID。|
|serviceLocation|[location](location.md)|服务的传递位置。|
|serviceName|String|与此约会相关联的**bookingService**的名称。<br>创建新约会时, 此属性是可选的。 如果未指定, 则通过**serviceId**属性从与约会关联的服务计算。|
|serviceNotes|String|来自[bookingStaffMember](bookingstaffmember.md)的注释。 此属性的值仅在按 ID 读取此**bookingAppointment**时可用。|
|staffMemberIds|String collection|在此约会中计划的每个[bookingStaffMember](bookingstaffmember.md)的 ID。|
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
<!--
{
  "type": "#page.annotation",
  "description": "bookingAppointment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingappointment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
