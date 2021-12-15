---
title: 更新 bookingappointment
description: 更新指定 bookingbusiness 中的 bookingAppointment 对象的属性。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: e3505c94f9ef16e7e19846ceaae9a8cdc3fc10dc
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525741"
---
# <a name="update-bookingappointment"></a>更新 bookingappointment

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新指定的[bookingBusiness](../resources/bookingbusiness.md)中的[bookingAppointment](../resources/bookingappointment.md)对象的属性。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All   |
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
| Authorization  | Bearer {code}。 必需。|

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|customerEmailAddress|String|预订约会 [的 bookingCustomer](../resources/bookingcustomer.md) 的 SMTP 地址。|
|customerId|String|此约会的 [bookingCustomer](../resources/bookingcustomer.md) 的 ID。 如果在创建约会时未指定任何 ID，则创建一个新的 **bookingCustomer** 对象。 设置后，你应考虑 **customerId** 不可变。|
|customerLocation|[location](../resources/location.md)|表示预订约会的 [bookingCustomer](../resources/bookingcustomer.md) 的位置信息。|
|customerName|String|客户的名称。|
|customerNotes|String|与此约会关联的客户的备注。 只有在通过 ID 读取 **此 bookingAppointment 时，才能** 获取该值。 <br> 只有在最初创建新客户的约会时，才能设置此属性。 此后，该值从 **customerId** 表示的客户计算。|
|customerPhone|String|客户的电话号码。|
|customers|[bookingCustomerInformation](../resources/bookingcustomerinformation.md) 集合|它向下列出了约会的客户属性。 约会将包含客户信息列表，每个单元将指示属于该约会的客户的属性。 可选。|
|customerTimeZone|String|客户的时区。 有关可能值的列表，请参阅 [dateTimeTimeZone](../resources/datetimetimezone.md)。|
|duration|期限|约会的长度，以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。 |
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|约会结束的日期、时间和时区。|
|invoiceAmount|双精度|发票上的计费金额。|
|invoiceDate|[dateTimeTimeZone](../resources/datetimetimezone.md)|此约会的发票的日期、时间和时区。|
|invoiceId|String|发票的 ID。|
|invoiceStatus|string| 发票的状态。 可取值为：`draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。|
|invoiceUrl|String|Microsoft Bookings 中发票的 URL。|
|filledAttendeesCount|Int32|约会中的当前客户数。 必填。|
|isLocationOnline|Boolean|如果为 True，则表明该约会将在线进行。 默认值为 false。|
|maximumAttendeesCount|Int32|约会中允许的最大客户数。 必填。|
|optOutOfCustomerEmail|Boolean|True 表示此约会的 [bookingCustomer](../resources/bookingcustomer.md) 不希望收到有关此约会的确认。|
|postBuffer|期限|例如，约会结束后要保留的清理时间量。 该值以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。 |
|preBuffer|期限|例如，在约会开始前保留准备的时间量。 该值以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。|
|price|双精度|指定 [bookingService](../resources/bookingservice.md)的约会的常规价格。|
|priceType|bookingPriceType| 为服务的定价结构提供灵活性的设置。 可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`、`unknownFutureValue`。|
|reminders|[bookingReminder](../resources/bookingreminder.md) 集合|为此约会发送的客户提醒集合。 此属性的值仅在按其 ID 读取此 **bookingAppointment** 时可用。|
|selfServiceAppointmentId|String|约会的附加跟踪 ID（如果约会是由客户直接在日程安排页面上创建的，而不是由员工代表客户创建的）。|
|服务 Id|String|与此约会关联的 [bookingService](../resources/bookingservice.md) 的 ID。|
|serviceLocation|[location](../resources/location.md)|服务交付位置。|
|serviceName|String|与此约会关联的 **bookingService** 的名称。<br>创建新约会时，此属性是可选的。 如果未指定，则通过 **serviceId** 属性从与约会关联的服务计算该约会。|
|serviceNotes|String|[bookingStaffMember 中的注释](../resources/bookingstaffmember.md)。 此属性的值仅在按其 ID 读取此 **bookingAppointment** 时可用。|
|smsNotificationsEnabled|Boolean|如果为 True，则表明将发送给客户进行约会的短信通知。 默认值为 false。|
|staffMemberIds|String collection|在此约会中 [安排的每个 bookingStaffMember](../resources/bookingstaffmember.md) 的 ID。|
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)|约会开始的日期、时间和时区。|


## <a name="response"></a>响应
如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。
## <a name="example"></a>示例
### <a name="request"></a>请求
以下示例将服务日期更改一天并更新发票日期。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingappointment"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/appointments/AAMkADKnAAA=
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingappointment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-bookingappointment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>响应
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
  ]
}
-->


