---
title: 更新 bookingCustomer
description: 更新 bookingCustomer 对象的属性。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 901fb2a6ae8908c3da084bd49b469992389e4a0b
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856006"
---
# <a name="update-bookingcustomer"></a>更新 bookingCustomer

命名空间：microsoft.graph

更新 [bookingCustomer](../resources/bookingcustomer.md) 对象的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All   |
|委派（个人 Microsoft 帐户） | 不支持。   |
|应用程序 | BookingsAppointment.ReadWrite.All、Bookings.Read.All  |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /solutions/bookingBusinesses/{id}/customers/{id}
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:-----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>请求正文

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|地址|[physicalAddress](../resources/physicaladdress.md) 集合|与客户关联的地址。 v1.0 不支持 physicalAddress 的属性 **类型** 。 在内部，我们将地址映射到类型 `others`。|
|displayName|String|客户的名称。|
|emailAddress|String|客户的 SMTP 地址。|
|phones|[phone](../resources/phone.md) collection|与客户关联的电话号码，包括家庭、业务和移动号码。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [bookingCustomer](../resources/bookingcustomer.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.bookingCustomer",
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```

### <a name="response"></a>响应

这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.bookingCustomer",
    "@odata.context": "https://graph.microsoft.com/v1.0/solutions/$metadata#bookingBusinesses('Contosolunchdelivery%40contoso.onmicrosoft.com')/customers/$entity",
    "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingcustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


