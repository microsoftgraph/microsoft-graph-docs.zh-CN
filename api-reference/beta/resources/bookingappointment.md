---
title: bookingAppointment 资源类型
description: 表示一个 bookingService 的客户约会，由一组工作人员执行，由Microsoft Bookings企业提供。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 18183d9f0694da1c2897cff92a5af7863b3df9c2
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160369"
---
# <a name="bookingappointment-resource-type"></a>bookingAppointment 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
表示一个 [bookingService](bookingservice.md) 的客户约会，由一组工作人员执行，由Microsoft Bookings业务提供。

> [!NOTE]
> 如果使用应用程序权限创建自定义应用，则必须遵循 [业务规则验证](/graph/bookingsbusiness-business-rules)。

## <a name="methods"></a>方法

| 方法           | 返回类型    |Description|
|:---------------|:--------|:----------|
|[列出约会](../api/bookingbusiness-list-appointments.md) |  [bookingAppointment](bookingappointment.md) 集合 | 获取指定 [bookingbusiness](bookingbusiness.md) 中的 **bookingAppointment** 对象列表。 |
|[创建 bookingAppointment](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | 为指定的 [bookingbusiness](bookingbusiness.md) 创建新的 **bookingAppointment**。 |
|[获取 bookingAppointment](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |读取 **bookingAppointment** 对象的属性和关系。|
|[更新](../api/bookingappointment-update.md) | 无   |更新 **bookingAppointment** 对象。 |
|[删除](../api/bookingappointment-delete.md) | 无 |删除 **bookingAppointment** 对象。 |
|[Cancel](../api/bookingappointment-cancel.md)|无| 取消 **bookingAppointment** 对象。|

## <a name="properties"></a>属性

| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|additionalInformation|String|确认约会时发送给客户的其他信息。|
|anonymousJoinWebUrl|String|要匿名加入的会议 URL。
|customerEmailAddress|String|预订约会的 [bookingCustomer](bookingcustomer.md) 的 SMTP 地址。|
|customerId|String|此约会的 [bookingCustomer](bookingcustomer.md) 的 ID。 如果在创建约会时未指定 ID，则会创建新的 **bookingCustomer** 对象。 设置后，应考虑 **customerId** 不可变。|
|customerLocation|[location](location.md)|表示预订约会的 [bookingCustomer](bookingcustomer.md) 的位置信息。|
|customerName|String|客户的名称。|
|customerNotes|String|与此约会关联的客户的说明。 仅当按其 ID 读取此 **bookingAppointment** 时，才可以获取该值。 <br> 只有在最初与新客户创建约会时，才能设置此属性。 之后，该值将从 **customerId** 代表的客户计算。|
|customerPhone|String|客户的电话号码。|
|客户|[bookingCustomerInformation](bookingcustomerinformation.md) 集合|它列出了约会的客户属性。 约会将包含客户信息列表，每个单位将指示属于该约会的客户的属性。 可选。|
|customerTimeZone|String|客户的时区。 有关可能值的列表，请参阅 [dateTimeTimeZone](datetimetimezone.md)。|
|duration|期限|约会的长度，以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。 |
|end|[dateTimeTimeZone](datetimetimezone.md)|约会结束的日期、时间和时区。|
|filledAttendeesCount|Int32|约会中的当前客户数。 |
|id|String| **bookingAppointment** 的 ID。 只读。|
|invoiceAmount|双精度|发票上的计费金额。|
|invoiceDate|[dateTimeTimeZone](datetimetimezone.md)|此约会的发票的日期、时间和时区。|
|invoiceId|String|发票的 ID。|
|invoiceStatus|string| 发票的状态。 可取值为：`draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。|
|invoiceUrl|String|Microsoft Bookings中的发票 URL。|
|isLocationOnline|布尔|True 表示约会将联机进行。 默认值为 false。|
|joinWebUrl|String|约会的联机会议的 URL。|
|maximumAttendeesCount|Int32|约会中允许的最大客户数。 如果服务 **的最大AttendeesCount** 大于 1，则在创建或更新约会时传递有效的客户 ID。 若要创建客户，请使用 [Create bookingCustomer](../api/bookingbusiness-post-customers.md) 操作。 |
|optOutOfCustomerEmail|布尔|True 表示此约会的 [bookingCustomer](bookingcustomer.md) 不希望收到此约会的确认。|
|postBuffer|期限|例如，约会结束后要保留的时间，用于清理。 该值以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。 |
|preBuffer|期限|例如，在约会开始之前，为准备而保留的时间量。 该值以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。|
|价格|双精度|指定 [bookingService](bookingservice.md) 的约会的常规价格。|
|priceType|bookingPriceType| 一个设置，用于为服务的定价结构提供灵活性。 可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`、`unknownFutureValue`。|
|提醒|[bookingReminder](bookingreminder.md) 集合|为此约会发送的客户提醒的集合。 仅当按其 ID 读取此 **bookingAppointment** 时，此属性的值才可用。|
|selfServiceAppointmentId|String|如果约会是由客户直接在计划页上创建的，而不是由代表客户的工作人员创建的，则为约会提供额外的跟踪 ID。|
|服务 Id|String|与此约会关联的 [bookingService](bookingservice.md) 的 ID。|
|serviceLocation|[location](location.md)|服务的传送位置。|
|serviceName|String|与此约会关联的 **bookingService** 的名称。<br>创建新约会时，此属性是可选的。 如果未指定，则会从 **ServiceId** 属性与约会关联的服务中进行计算。|
|serviceNotes|String|[bookingStaffMember](bookingstaffmember.md) 中的备注。 仅当按其 ID 读取此 **bookingAppointment** 时，此属性的值才可用。|
|smsNotificationsEnabled|布尔|True 表示短信通知将发送给客户进行约会。 默认值为 false。|
|staffMemberIds|字符串集合|此约会中计划的每位 [bookingStaffMember](bookingstaffmember.md) 的 ID。|
|start|[dateTimeTimeZone](datetimetimezone.md)|约会开始的日期、时间和时区。|

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
  "customerEmailAddress": "String",
  "customerId": "String",
  "customerLocation": {"@odata.type": "microsoft.graph.location"},
  "customerName": "String",
  "customerNotes": "String",
  "customerPhone": "String",
  "customerTimeZone": "String",
  "customers": [
    {
      "@odata.type": "microsoft.graph.bookingCustomerInformation"
    }
  ],
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
  "anonymousJoinWebUrl": "String",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "price": 1024,
  "priceType": {"@odata.type": "microsoft.graph.bookingPriceType"},
  "reminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "selfServiceAppointmentId": "String",
  "serviceId": "String",
  "serviceLocation": {"@odata.type": "microsoft.graph.location"},
  "serviceName": "String",
  "serviceNotes": "String",
  "smsNotificationsEnabled": "Boolean",
  "staffMemberIds": ["String"],
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
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


