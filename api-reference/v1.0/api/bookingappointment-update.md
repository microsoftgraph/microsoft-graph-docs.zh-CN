---
title: 更新 bookingAppointment
description: 更新指定 bookingBusiness 中的 bookingAppointment 对象的属性。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: d1b2e9863f8cc98cd2d17b9867817bb804dc3217
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367970"
---
# <a name="update-bookingappointment"></a>更新 bookingAppointment

命名空间：microsoft.graph

更新指定 [bookingBusiness 中的 bookingAppointment](../resources/bookingappointment.md) 对象 [的属性](../resources/bookingbusiness.md)。
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
PATCH /solutions/bookingBusinesses/{id}/appointments/{id}
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:-----------|
| Authorization  | Bearer {code}。 必需。|

## <a name="request-body"></a>请求正文

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|customers|[bookingCustomerInformation](../resources/bookingcustomerinformation.md) 集合|它向下列出了约会的客户属性。 约会将包含客户信息列表，每个单元将指示属于该约会的客户的属性。 可选。|
|customerTimeZone|String|客户的时区。 有关可能值的列表，请参阅 [dateTimeTimeZone](../resources/datetimetimezone.md)。|
|duration|期限|约会的长度，以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。 |
|endDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|约会结束的日期、时间和时区。|
|filledAttendeesCount|Int32|约会中的当前客户数。 必需项。|
|isLocationOnline|Boolean|如果 `true`为 ，则指示约会将联机进行。 默认值为 false。|
|maximumAttendeesCount|Int32|约会中允许的最大客户数。 必需项。 |
|optOutOfCustomerEmail|Boolean|如果 `true`为 ，表示此约会的 [bookingCustomer](../resources/bookingcustomer.md) 不希望收到有关此约会的确认。|
|postBuffer|期限|例如，约会结束后要保留的清理时间量。 该值以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。 |
|preBuffer|期限|例如，在约会开始前保留准备的时间量。 该值以 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式表示。|
|price|双精度|指定 [bookingService](../resources/bookingservice.md) 的约会的常规价格。|
|priceType|bookingPriceType| 为服务的定价结构提供灵活性的设置。 可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`、`unknownFutureValue`。|
|reminders|[bookingReminder](../resources/bookingreminder.md) 集合|为此约会发送的客户提醒集合。 此属性的值仅在按其 ID 读取 **此 bookingAppointment** 时可用。|
|selfServiceAppointmentId|String|约会的附加跟踪 ID（如果约会是由客户直接在日程安排页面上创建的，而不是由员工代表客户创建的）。 仅在 maxAttendeeCount 为 1 时才支持约会。|
|服务 Id|String|与此约会关联的 [bookingService](../resources/bookingservice.md) 的 ID。|
|serviceLocation|[location](../resources/location.md)|服务交付位置。|
|serviceName|字符串|与此约会 **关联的 bookingService** 的名称。<br>创建新约会时，此属性是可选的。 如果未指定，则通过 **serviceId** 属性从与约会关联的服务计算该约会。|
|serviceNotes|String|[bookingStaffMember 中的注释](../resources/bookingstaffmember.md)。 此属性的值仅在按其 ID 读取 **此 bookingAppointment** 时可用。|
|smsNotificationsEnabled|Boolean|如果 `true`为 ，表示将发送给客户进行约会的短信通知。 默认值为 false。|
|staffMemberIds|字符串集合|在此约会中 [安排的每个 bookingStaffMember](../resources/bookingstaffmember.md) 的 ID。|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|约会开始的日期、时间和时区。|

> [!NOTE]
> 如果服务中允许 (**maximumAttedeesCount**) 数 [大于](../resources/bookingservice.md) 1：
> - 确保客户存在于 Booking Calendar 中。 如果没有，则使用 Create [bookingCustomer](bookingbusiness-post-customers.md) 操作创建。
> - 创建或更新约会时传递有效的客户 ID。 如果客户 ID 无效，该客户将不会包含在约会对象中。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求
以下示例将服务日期更改一天。

<!-- {
  "blockType": "request"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/appointments/AAMkADKnAAA=
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingAppointment",
    "endDateTime":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "startDateTime":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:00:00.0000000+00:00",
        "timeZone":"UTC"
    }
}
```

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


