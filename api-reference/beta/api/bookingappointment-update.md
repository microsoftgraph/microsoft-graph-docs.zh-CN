---
title: 更新 bookingappointment
description: 更新中指定 bookingbusiness bookingAppointment 对象的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cde8a309e3544f5ed5cdf84f7c50d33e95084526
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529234"
---
# <a name="update-bookingappointment"></a>更新 bookingappointment

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新中指定[bookingbusiness](../resources/bookingbusiness.md) [bookingAppointment](../resources/bookingappointment.md)对象的属性。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All，Bookings.Manage.All   |
|委派（个人 Microsoft 帐户） | 不支持。   |
|应用程序 | 不支持。  |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-request-headers"></a>可选的请求标头
| 名称       | 说明|
|:-----------|:-----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|customerEmailAddress|String|预订约会[bookingCustomer](../resources/bookingcustomer.md) SMTP 地址。|
|customerId|String|该约会的[bookingCustomer](../resources/bookingcustomer.md)的 ID。 如果未指定 ID 创建约会时，将创建一个新的**bookingCustomer**对象。 设置后，您应考虑**customerId**变。|
|customerLocation|[location](../resources/location.md)|代表[bookingCustomer](../resources/bookingcustomer.md)预订约会的位置信息。|
|customerName|String|客户的名称。|
|customerNotes|String|从与此约会关联的客户的备注。 您可以获取仅当读取此**bookingAppointment**其 id 值 <br> 仅在最初使用新的客户创建约会时，您可以设置该属性。 此时，从由**customerId**客户计算的值。|
|customerPhone|String|客户的电话号码。|
|duration|持续时间|约会中[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式的长度。 |
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|日期、 时间和约会的结束的时区。|
|invoiceAmount|双精度|记帐的发票量。|
|invoiceDate|[dateTimeTimeZone](../resources/datetimetimezone.md)|日期、 时间和此约会的发票的时区。|
|invoiceId|String|发票的 ID。|
|invoiceStatus|string| 发票的状态。 可取值为：`draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。|
|invoiceUrl|String|在 Microsoft 预订发票的 URL。|
|optOutOfCustomerEmail|Boolean|True 表示该约会的[bookingCustomer](../resources/bookingcustomer.md)不希望接收该约会的确认。|
|后|持续时间|保留后的清理，例如约会结束的时间量。 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示的值。 |
|缓冲区|持续时间|保留之前的准备，例如约会开始的时间量。 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示的值。|
|Price|双精度|指定[bookingService](../resources/bookingservice.md)约会正则价格。|
|priceType|string| 为服务定价结构提供灵活性设置。 可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。|
|提醒|[bookingReminder](../resources/bookingreminder.md)集合|客户提醒发送该约会的集合。 此属性的值时，可仅读取此**bookingAppointment**由其 id。|
|selfServiceAppointmentId|String|约会，如果约会的已创建直接通过计划页上的客户而不是由员工成员客户替的其他跟踪 ID。|
|服务 Id|String|与此约会相关联的[bookingService](../resources/bookingservice.md) ID。|
|serviceLocation|[location](../resources/location.md)|传递服务的位置的位置。|
|service_name|String|与此约会关联**bookingService**的名称。<br>创建一个新的约会时，此属性是可选的。 如果未指定，它是从与约会**serviceId**属性关联的服务进行计算。|
|serviceNotes|String|从[bookingStaffMember](../resources/bookingstaffmember.md)备注。 此属性的值时，可仅读取此**bookingAppointment**由其 id。|
|staffMemberIds|String 集合|每个[bookingStaffMember](../resources/bookingstaffmember.md)此约会中安排的 ID。|
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)|日期、 时间和时区约会的开始。|


## <a name="response"></a>响应
如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。
## <a name="example"></a>示例
##### <a name="request"></a>请求
以下示例更改服务通过一天的日期和更新的发票日期。
<!-- {
  "blockType": "request",
  "name": "update_bookingappointment"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingAppointment",
    "end":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceDate":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "start":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:00:00.0000000+00:00",
        "timeZone":"UTC"
    }
}
```
##### <a name="response"></a>响应
下面展示了示例响应。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingappointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingappointment-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
