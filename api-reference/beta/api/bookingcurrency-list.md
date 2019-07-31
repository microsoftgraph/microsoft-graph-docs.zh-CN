---
title: 列出 bookingCurrencies
description: 获取可用于 Microsoft 预订业务的 bookingCurrency 对象的列表。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 5fbc7f2bf36646435e8d98ec26e31726c1a9c0ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944995"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="78bd2-103">列出 bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="78bd2-103">List bookingCurrencies</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78bd2-104">获取可用于 Microsoft 预订业务的[bookingCurrency](../resources/bookingcurrency.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="78bd2-104">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="78bd2-105">权限</span><span class="sxs-lookup"><span data-stu-id="78bd2-105">Permissions</span></span>
<span data-ttu-id="78bd2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78bd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78bd2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="78bd2-108">Permission type</span></span>      | <span data-ttu-id="78bd2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78bd2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78bd2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78bd2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="78bd2-111">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="78bd2-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="78bd2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78bd2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78bd2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="78bd2-113">Not supported.</span></span>   |
|<span data-ttu-id="78bd2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="78bd2-114">Application</span></span> | <span data-ttu-id="78bd2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="78bd2-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="78bd2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78bd2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="78bd2-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="78bd2-117">Optional query parameters</span></span>
<span data-ttu-id="78bd2-118">此方法支持[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters), 以帮助自定义响应, 包括 $count、$filter、$select、$skip 和 $top。</span><span class="sxs-lookup"><span data-stu-id="78bd2-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78bd2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="78bd2-119">Request headers</span></span>
| <span data-ttu-id="78bd2-120">名称</span><span class="sxs-lookup"><span data-stu-id="78bd2-120">Name</span></span>      |<span data-ttu-id="78bd2-121">说明</span><span class="sxs-lookup"><span data-stu-id="78bd2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="78bd2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="78bd2-122">Authorization</span></span>  | <span data-ttu-id="78bd2-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="78bd2-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="78bd2-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="78bd2-124">Request body</span></span>
<span data-ttu-id="78bd2-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="78bd2-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="78bd2-126">响应</span><span class="sxs-lookup"><span data-stu-id="78bd2-126">Response</span></span>
<span data-ttu-id="78bd2-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[bookingCurrency](../resources/bookingcurrency.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="78bd2-127">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="78bd2-128">示例</span><span class="sxs-lookup"><span data-stu-id="78bd2-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78bd2-129">请求</span><span class="sxs-lookup"><span data-stu-id="78bd2-129">Request</span></span>
<span data-ttu-id="78bd2-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="78bd2-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="78bd2-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="78bd2-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="78bd2-132">C#</span><span class="sxs-lookup"><span data-stu-id="78bd2-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcurrencies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="78bd2-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="78bd2-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcurrencies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="78bd2-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="78bd2-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcurrencies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="78bd2-135">Java</span><span class="sxs-lookup"><span data-stu-id="78bd2-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingcurrencies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="78bd2-136">响应</span><span class="sxs-lookup"><span data-stu-id="78bd2-136">Response</span></span>
<span data-ttu-id="78bd2-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="78bd2-137">The following is an example of the response.</span></span> <span data-ttu-id="78bd2-138">注意: 为简洁起见, 此处显示的响应对象将被截断。</span><span class="sxs-lookup"><span data-stu-id="78bd2-138">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="78bd2-139">所有受支持的货币和属性都将从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="78bd2-139">All of the supported currencies and properties will be returned from an actual call.</span></span>
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
