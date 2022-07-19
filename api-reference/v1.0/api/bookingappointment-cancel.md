---
title: bookingAppointment：取消
description: 取消指定 bookingBusiness 中的指定 bookingAppointment，并向相关客户和员工发送消息。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 60244dcf48344136bb2c1aba92c3964ea34a4cb5
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856363"
---
# <a name="bookingappointment-cancel"></a>bookingAppointment：取消

命名空间：microsoft.graph

取消指定 [bookingBusiness](../resources/bookingbusiness.md) 中的指定 [bookingAppointment](../resources/bookingappointment.md)，并向相关客户和员工发送消息。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All   |
|委派（个人 Microsoft 帐户） | 不支持。   |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /solutions/bookingBusinesses/{id}/appointments/{id}/cancel

```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:---------------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|cancellationMessage|String|向客户确认 **约会** 已取消的消息。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

如果尝试取消不存在的 **约会** ，此方法将返回一个 `404 Not found`。

## <a name="example"></a>示例

下面是如何调用此 API 的示例。

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/appointments/AAMkADKoAAA=/cancel
Content-type: application/json

{
  "cancellationMessage": "Your appointment has been successfully cancelled. Please call us again."
}
```

### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingAppointment: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


