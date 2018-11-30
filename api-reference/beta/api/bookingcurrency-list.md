---
title: 列表 bookingCurrencies
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.openlocfilehash: 146fc1197a8ef206e78304d81c30878a67eeafad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041425"
---
# <a name="list-bookingcurrencies"></a>列表 bookingCurrencies

 > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。
 
获取供 Microsoft 预订业务[bookingCurrency](../resources/bookingcurrency.md)对象的列表。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Bookings.Read.All，BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All Bookings.Manage.All   |
|委派（个人 Microsoft 帐户） | 不支持。   |
|应用程序 | 不支持。  | 

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持用于帮助自定义的响应，其中包括 $count、 $filter、 $select、 $skip 和 $top 的[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
## <a name="response"></a>响应
如果成功，此方法返回`200 OK`响应代码和响应正文中的[bookingCurrency](../resources/bookingcurrency.md)对象的集合。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
##### <a name="response"></a>响应
下面展示了示例响应。 注意： 为了简单起见截断如下所示的响应对象。 从实际的呼叫，将返回所有的受支持的货币和属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCurrency",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingCurrencies",
    "value":[
        {
            "id":"AED",
            "symbol":"د.إ.‏"
        },
        {
            "id":"AFN",
            "symbol":"؋"
        },
        {
            "id":"ALL",
            "symbol":"Lekë"
        },
        {
            "id":"AMD",
            "symbol":"֏"
        },
        {
            "id":"USD",
            "symbol":"$"
        },
        {
            "id":"YER",
            "symbol":"ر.ي.‏"
        },
        {
            "id":"ZAR",
            "symbol":"R"
        },
        {
            "id":"ZMW",
            "symbol":"K"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List bookingCurrencies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->