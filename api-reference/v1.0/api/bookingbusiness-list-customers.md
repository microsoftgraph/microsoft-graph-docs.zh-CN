---
title: 列出客户
description: 获取业务中的 bookingCustomer 对象列表。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 1e621a17d2ec9a072d1b421942475916f8b25404
ms.sourcegitcommit: 086e9a2ccaef411f9471cca164a79197bb254521
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2022
ms.locfileid: "62014255"
---
# <a name="list-customers"></a>列出客户

命名空间：microsoft.graph

获取业务中的 [bookingCustomer](../resources/bookingcustomer.md) 对象列表。
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
GET /solutions/bookingBusinesses/{id}/customers
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持使用 $count 和 $expand [OData](/graph/query-parameters) 查询参数来帮助自定义响应。

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [bookingCustomer](../resources/bookingcustomer.md) 对象集合。
## <a name="example"></a>示例
### <a name="request"></a>请求
下面展示了示例请求。

<!-- {
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customers
```

### <a name="response"></a>响应
下面展示了示例响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/solutions/$metadata#bookingBusinesses('Contosolunchdelivery%40contoso.onmicrosoft.com')/customers",
    "value": [
        {
            "@odata.type": "#microsoft.graph.bookingCustomer",
            "id": "80b5ddda-1e3b-4c9d-abe2-d606cc075e2e",
            "displayName": "Adele Vance",
            "emailAddress": "adelev@proseware.com",
            "addresses": [],
            "phones": []
        },
        {
            "@odata.type": "#microsoft.graph.bookingCustomer",
            "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
            "displayName": "Adele Vance",
            "emailAddress": "adelev@proseware.com",
            "addresses": [
                {
                    "postOfficeBox":"",
                    "street":"4567 Main Street",
                    "city":"Buffalo",
                    "state":"NY",
                    "countryOrRegion":"USA",
                    "postalCode":"98052",
                    "type":"home"
                },
                {
                    "postOfficeBox":"",
                    "street":"4570 Main Street",
                    "city":"Buffalo",
                    "state":"NY",
                    "countryOrRegion":"USA",
                    "postalCode":"98054",
                    "type":"business"
                }
            ],
            "phones": [
                {
                    "number": "206-555-0100",
                    "type": "home"
                },
                {
                    "number": "206-555-0200",
                    "type": "business"
                }
            ]
        },
        {
            "@odata.type": "#microsoft.graph.bookingCustomer",
            "id": "829e3cb5-3d4d-4319-a8de-1953aedaa166",
            "displayName": "Bob Kelly",
            "emailAddress": "bobk@tailspintoys.com",
            "addresses": [],
            "phones": []
        },
        {
            "@odata.type": "#microsoft.graph.bookingCustomer",
            "id": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
            "displayName": "Jordan Miller",
            "emailAddress": "jordanm@contoso.com",
            "addresses": [],
            "phones": []
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List customers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
