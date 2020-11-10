---
title: 更新 bookingappointment
description: 更新指定 bookingbusiness 中的 bookingAppointment 对象的属性。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 1e5ecedaefe5eaf0cdd355bbdf5547bfae38c683
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960916"
---
# <a name="update-bookingappointment"></a>更新 bookingappointment

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新指定[bookingbusiness](../resources/bookingbusiness.md)中的[bookingAppointment](../resources/bookingappointment.md)对象的属性。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  BookingsAppointment，全部，全部登记，全部，预订。 All   |
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
|customerEmailAddress|String|预订约会的 [bookingCustomer](../resources/bookingcustomer.md) 的 SMTP 地址。|
|customerId|String|此约会的 [bookingCustomer](../resources/bookingcustomer.md) 的 ID。 如果创建约会时未指定 ID，则会创建一个新的 **bookingCustomer** 对象。 设置后，应考虑 **customerId** 不可变。|
|customerLocation|[location](../resources/location.md)|表示预订约会的 [bookingCustomer](../resources/bookingcustomer.md) 的位置信息。|
|customerName|String|客户的名称。|
|customerNotes|String|来自与此约会相关联的客户的注释。 仅当按 ID 读取此 **bookingAppointment** 时，才能获取该值。 <br> 只有在最初创建新客户的约会时，才能设置该属性。 然后，将从 **customerId** 表示的客户计算该值。|
|customerPhone|String|客户的电话号码。|
|duration|持续时间|约会的长度，以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。 |
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|约会结束的日期、时间和时区。|
|invoiceAmount|双精度|发票上的计费金额。|
|invoiceDate|[dateTimeTimeZone](../resources/datetimetimezone.md)|此约会的发票的日期、时间和时区。|
|invoiceId|String|发票的 ID。|
|invoiceStatus|string| 发票的状态。 可取值为：`draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。|
|invoiceUrl|String|Microsoft 预订中发票的 URL。|
|optOutOfCustomerEmail|Boolean|如果为 True，则表示此约会的 [bookingCustomer](../resources/bookingcustomer.md) 不希望收到此约会的确认。|
|postBuffer|持续时间|在约会结束后保留的时间长度，例如，进行清理。 值以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。 |
|preBuffer|持续时间|在约会开始之前保留的时间量（以供准备）为例。 值以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。|
|特价|双精度|指定 [bookingService](../resources/bookingservice.md)的约会的常规价格。|
|priceType|string| 一种设置，可为服务的定价结构提供灵活性。 可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。|
|提醒|[bookingReminder](../resources/bookingreminder.md) 集合|为此约会发送的客户提醒的集合。 此属性的值仅在按 ID 读取此 **bookingAppointment** 时可用。|
|selfServiceAppointmentId|String|约会的其他跟踪 ID，如果约会是由客户在日程安排页面上直接创建的，而不是代表客户由教职员工成员创建的。|
|服务 Id|String|与此约会相关联的 [bookingService](../resources/bookingservice.md) 的 ID。|
|serviceLocation|[location](../resources/location.md)|服务的传递位置。|
|serviceName|String|与此约会相关联的 **bookingService** 的名称。<br>创建新约会时，此属性是可选的。 如果未指定，则通过 **serviceId** 属性从与约会关联的服务计算。|
|serviceNotes|String|来自 [bookingStaffMember](../resources/bookingstaffmember.md)的注释。 此属性的值仅在按 ID 读取此 **bookingAppointment** 时可用。|
|staffMemberIds|String collection|在此约会中计划的每个 [bookingStaffMember](../resources/bookingstaffmember.md) 的 ID。|
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)|约会开始的日期、时间和时区。|


## <a name="response"></a>响应
如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面的示例将服务日期更改为一天，并同时更新发票日期。

# <a name="http"></a>[HTTP](#tab/http)
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

---

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
  ]
}
-->


