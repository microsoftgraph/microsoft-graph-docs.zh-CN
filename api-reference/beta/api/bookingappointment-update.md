---
title: 更新 bookingAppointment
description: 更新指定 bookingBusiness 中 bookingAppointment 对象的属性。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: fcbbb774d3981a1174493e2305c78e2042988985
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2022
ms.locfileid: "64755549"
---
# <a name="update-bookingappointment"></a>更新 bookingAppointment

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新指定 [bookingBusiness](../resources/bookingbusiness.md) 中 [bookingAppointment](../resources/bookingappointment.md) 对象的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  BookingsAppointment.ReadWrite.All，Bookings。ReadWrite.All，Bookings。Manage.All   |
|委派（个人 Microsoft 帐户） | 不支持。   |
|Application | BookingsAppointment.ReadWrite.All，Bookings。Read.All  |

> [!NOTE]
> 如果使用应用程序权限创建自定义应用，则必须遵循 [业务规则验证](/graph/bookingsbusiness-business-rules)。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```

## <a name="optional-request-headers"></a>可选的请求标头

| 名称       | 说明|
|:-----------|:-----------|
| Authorization  | 持有者 {code}。必需。|

## <a name="request-body"></a>请求正文

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|customerEmailAddress|String|预订约会的 [bookingCustomer](../resources/bookingcustomer.md) 的 SMTP 地址。|
|customerId|String|此约会的 [bookingCustomer](../resources/bookingcustomer.md) 的 ID。 如果在创建约会时未指定 ID，则会创建新的 **bookingCustomer** 对象。 设置后，应考虑 **customerId** 不可变。|
|customerLocation|[location](../resources/location.md)|表示预订约会的 [bookingCustomer](../resources/bookingcustomer.md) 的位置信息。|
|customerName|String|客户的名称。|
|customerNotes|String|与此约会关联的客户的说明。 仅当按其 ID 读取此 **bookingAppointment** 时，才可以获取该值。 <br> 只有在最初与新客户创建约会时，才能设置此属性。 之后，该值将从 **customerId** 代表的客户计算。|
|customerPhone|String|客户的电话号码。|
|客户|[bookingCustomerInformation](../resources/bookingcustomerinformation.md) 集合|它列出了约会的客户属性。 约会将包含客户信息列表，每个单位将指示属于该约会的客户的属性。 可选。|
|customerTimeZone|String|客户的时区。 有关可能值的列表，请参阅 [dateTimeTimeZone](../resources/datetimetimezone.md)。|
|duration|期限|约会的长度，以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。 |
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|约会结束的日期、时间和时区。|
|invoiceAmount|双精度|发票上的计费金额。|
|invoiceDate|[dateTimeTimeZone](../resources/datetimetimezone.md)|此约会的发票的日期、时间和时区。|
|invoiceId|String|发票的 ID。|
|invoiceStatus|string| 发票的状态。 可取值为：`draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。|
|invoiceUrl|String|Microsoft Bookings中的发票 URL。|
|filledAttendeesCount|Int32|约会中的当前客户数。 必需。|
|isLocationOnline|Boolean|True 表示约会将联机进行。 默认值为 false。|
|maximumAttendeesCount|Int32|约会中允许的最大客户数。 必需。 |
|optOutOfCustomerEmail|Boolean|True 表示此约会的 [bookingCustomer](../resources/bookingcustomer.md) 不希望收到此约会的确认。|
|postBuffer|期限|例如，约会结束后要保留的时间，用于清理。 该值以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。 |
|preBuffer|期限|例如，在约会开始之前，为准备而保留的时间量。 该值以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。|
|价格|双精度|指定 [bookingService](../resources/bookingservice.md) 的约会的常规价格。|
|priceType|bookingPriceType| 一个设置，用于为服务的定价结构提供灵活性。 可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`、`unknownFutureValue`。|
|提醒|[bookingReminder](../resources/bookingreminder.md) 集合|为此约会发送的客户提醒的集合。 仅当按其 ID 读取此 **bookingAppointment** 时，此属性的值才可用。|
|selfServiceAppointmentId|String|如果约会是由客户直接在计划页上创建的，而不是由代表客户的工作人员创建的，则为约会提供额外的跟踪 ID。|
|服务 Id|String|与此约会关联的 [bookingService](../resources/bookingservice.md) 的 ID。|
|serviceLocation|[location](../resources/location.md)|服务的传送位置。|
|serviceName|String|与此约会关联的 **bookingService** 的名称。<br>创建新约会时，此属性是可选的。 如果未指定，则会从 **ServiceId** 属性与约会关联的服务中进行计算。|
|serviceNotes|String|[bookingStaffMember](../resources/bookingstaffmember.md) 中的备注。 仅当按其 ID 读取此 **bookingAppointment** 时，此属性的值才可用。|
|smsNotificationsEnabled|Boolean|True 表示将向客户发送短信通知以进行约会。 默认值为 false。|
|staffMemberIds|String collection|此约会中计划的每位 [bookingStaffMember](../resources/bookingstaffmember.md) 的 ID。|
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)|约会开始的日期、时间和时区。|

> [!NOTE]
> 如果服务中允许的最大客户数 (**最大AttedeesCount**) 大于 1：[](../resources/bookingservice.md)
> - 确保客户存在于“预订日历”中。 如果不这样做，请使用 [Create bookingCustomer 操作创建](bookingbusiness-post-customers.md) 。
> - 创建或更新约会时传递有效的客户 ID。 如果客户 ID 无效，则该客户不会包含在约会对象中。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。 它不会在响应正文中返回任何内容。

## <a name="example"></a>示例

### <a name="request"></a>请求

以下示例将服务日期更改为一天，并更新发票日期。

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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-bookingappointment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-bookingappointment-powershell-snippets.md)]
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


