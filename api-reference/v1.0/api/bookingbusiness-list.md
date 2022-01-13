---
title: 列出 bookingBusinesses
description: 获取为租户创建的 bookingbusiness 对象的集合。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 936a34a17657ee7cfc97851772d4c9e8b1e85208
ms.sourcegitcommit: 086e9a2ccaef411f9471cca164a79197bb254521
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2022
ms.locfileid: "62014227"
---
# <a name="list-bookingbusinesses"></a>列出 bookingBusinesses

命名空间：microsoft.graph

获取为 [租户创建的 bookingBusiness](../resources/bookingbusiness.md) 对象的集合。

此操作仅返回集合中每个 Microsoft Bookings 公司的 **id** 和 **displayName。** 出于性能方面的考虑，它不会返回其他属性。 可以通过在 [GET](bookingbusiness-get.md)操作中指定 Microsoft Bookings 业务 **ID，获取** 其其他属性。


## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All   |
|委派（个人 Microsoft 帐户） | 不支持。   |
|应用程序 | 不支持。  |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /solutions/bookingBusinesses
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持使用 $count 和 $expand [OData](/graph/query-parameters) 查询参数来帮助自定义响应。

此方法还支持 `query` 接受字符串值的参数。 此参数将 GET 结果限定为匹配指定字符串的企业。 有关详细信息，请参阅 [示例](#request-2)。

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
## <a name="response"></a>响应
如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [bookingBusiness](../resources/bookingbusiness.md) 对象集合。

## <a name="examples"></a>示例

### <a name="example-1-get-bookings-businesses-in-a-tenant"></a>示例 1：获取租户中的 Bookings 业务
#### <a name="request-1"></a>请求 1
以下示例获取租户中的 Bookings 业务。

<!-- {
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/solutions/bookingBusinesses
```

#### <a name="response-1"></a>响应 1
下面介绍响应示例。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/solutions/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"Contosolunchdelivery@contoso.onmicrosoft.com",
            "displayName":"Contoso lunch delivery",
        },
        {
            "id":"Fabrikam@contoso.onmicrosoft.com",
            "displayName":"Fabrikam",
        }
    ]
}
```

### <a name="example-2-use-query-to-get-one-or-more-matching-bookings-businesses-in-a-tenant"></a>示例 2：使用"查询"获取租户中的一个或多个匹配的 Bookings 业务
#### <a name="request-2"></a>请求 2
以下示例演示如何使用 参数获取租户中一个或多个匹配的 `query` Bookings 企业。

<!-- {
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/solutions/bookingBusinesses?query=Adventure
```

#### <a name="response-2"></a>响应 2
下面展示了示例响应。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/solutions/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"AdventureWorksCycles@M365B960066.onmicrosoft.com",
            "displayName":"Adventure Works Cycles",
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List bookingBusinesses",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
