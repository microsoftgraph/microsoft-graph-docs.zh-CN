---
title: 获取 bookingCurrency
description: 获取可用于 Microsoft 预订业务的 bookingCurrency 对象的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: b005f051449538e438ed40b4a89c8355b6cbbace
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720205"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="8fe21-103">获取 bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="8fe21-103">Get bookingCurrency</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fe21-104">获取可用于 Microsoft 预订业务的[bookingCurrency](../resources/bookingcurrency.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8fe21-104">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="8fe21-105">使用**id**属性 (即货币代码) 指定货币。</span><span class="sxs-lookup"><span data-stu-id="8fe21-105">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="8fe21-106">权限</span><span class="sxs-lookup"><span data-stu-id="8fe21-106">Permissions</span></span>
<span data-ttu-id="8fe21-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8fe21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fe21-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8fe21-109">Permission type</span></span>      | <span data-ttu-id="8fe21-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8fe21-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fe21-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8fe21-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8fe21-112">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="8fe21-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="8fe21-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8fe21-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fe21-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8fe21-114">Not supported.</span></span>   |
|<span data-ttu-id="8fe21-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8fe21-115">Application</span></span> | <span data-ttu-id="8fe21-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8fe21-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="8fe21-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8fe21-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8fe21-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8fe21-118">Optional query parameters</span></span>
<span data-ttu-id="8fe21-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8fe21-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8fe21-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8fe21-120">Request headers</span></span>
| <span data-ttu-id="8fe21-121">名称</span><span class="sxs-lookup"><span data-stu-id="8fe21-121">Name</span></span>      |<span data-ttu-id="8fe21-122">说明</span><span class="sxs-lookup"><span data-stu-id="8fe21-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8fe21-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fe21-123">Authorization</span></span>  | <span data-ttu-id="8fe21-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8fe21-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fe21-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8fe21-125">Request body</span></span>
<span data-ttu-id="8fe21-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8fe21-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8fe21-127">响应</span><span class="sxs-lookup"><span data-stu-id="8fe21-127">Response</span></span>
<span data-ttu-id="8fe21-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[bookingCurrency](../resources/bookingcurrency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8fe21-128">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8fe21-129">示例</span><span class="sxs-lookup"><span data-stu-id="8fe21-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8fe21-130">请求</span><span class="sxs-lookup"><span data-stu-id="8fe21-130">Request</span></span>
<span data-ttu-id="8fe21-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8fe21-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8fe21-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8fe21-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8fe21-133">C#</span><span class="sxs-lookup"><span data-stu-id="8fe21-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcurrency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8fe21-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8fe21-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcurrency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8fe21-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="8fe21-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcurrency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8fe21-136">响应</span><span class="sxs-lookup"><span data-stu-id="8fe21-136">Response</span></span>
<span data-ttu-id="8fe21-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8fe21-137">The following is an example of the response.</span></span> <span data-ttu-id="8fe21-138">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8fe21-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8fe21-139">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8fe21-139">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCurrency"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 50

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingCurrencies/$entity",
    "id": "USD",
    "symbol": "$"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingCurrency",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
