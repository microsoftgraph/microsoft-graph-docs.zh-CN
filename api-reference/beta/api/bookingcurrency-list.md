---
title: 列出 bookingCurrencies
description: 获取可用于 Microsoft 预订业务的 bookingCurrency 对象的列表。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 644351aa2dff960590940cddfad3abbdda5d2b1d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987923"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="3099a-103">列出 bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="3099a-103">List bookingCurrencies</span></span>

<span data-ttu-id="3099a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3099a-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3099a-105">获取可用于 Microsoft 预订业务的 [bookingCurrency](../resources/bookingcurrency.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="3099a-105">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="3099a-106">权限</span><span class="sxs-lookup"><span data-stu-id="3099a-106">Permissions</span></span>
<span data-ttu-id="3099a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3099a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3099a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3099a-109">Permission type</span></span>      | <span data-ttu-id="3099a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3099a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3099a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3099a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3099a-112">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="3099a-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="3099a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3099a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3099a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3099a-114">Not supported.</span></span>   |
|<span data-ttu-id="3099a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3099a-115">Application</span></span> | <span data-ttu-id="3099a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3099a-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3099a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3099a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3099a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3099a-118">Optional query parameters</span></span>
<span data-ttu-id="3099a-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) ，以帮助自定义响应，包括 $count、$filter、$select、$skip 和 $top。</span><span class="sxs-lookup"><span data-stu-id="3099a-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3099a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3099a-120">Request headers</span></span>
| <span data-ttu-id="3099a-121">名称</span><span class="sxs-lookup"><span data-stu-id="3099a-121">Name</span></span>      |<span data-ttu-id="3099a-122">说明</span><span class="sxs-lookup"><span data-stu-id="3099a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3099a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3099a-123">Authorization</span></span>  | <span data-ttu-id="3099a-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3099a-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3099a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3099a-125">Request body</span></span>
<span data-ttu-id="3099a-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3099a-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3099a-127">响应</span><span class="sxs-lookup"><span data-stu-id="3099a-127">Response</span></span>
<span data-ttu-id="3099a-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [bookingCurrency](../resources/bookingcurrency.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3099a-128">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3099a-129">示例</span><span class="sxs-lookup"><span data-stu-id="3099a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3099a-130">请求</span><span class="sxs-lookup"><span data-stu-id="3099a-130">Request</span></span>
<span data-ttu-id="3099a-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3099a-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3099a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3099a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingCurrencies
```
# <a name="c"></a>[<span data-ttu-id="3099a-133">C#</span><span class="sxs-lookup"><span data-stu-id="3099a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcurrencies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3099a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3099a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcurrencies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3099a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3099a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcurrencies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3099a-136">响应</span><span class="sxs-lookup"><span data-stu-id="3099a-136">Response</span></span>
<span data-ttu-id="3099a-137">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="3099a-137">The following is an example of the response.</span></span> <span data-ttu-id="3099a-138">注意：为简洁起见，此处显示的响应对象将被截断。</span><span class="sxs-lookup"><span data-stu-id="3099a-138">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="3099a-139">所有受支持的货币和属性都将从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3099a-139">All of the supported currencies and properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List bookingCurrencies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


