---
title: 获取 bookingCurrency
description: 获取可用于 Microsoft 预订业务的 bookingCurrency 对象的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 4a7e63b0a5e5f5765056fa58696d13a0c3135573
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441128"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="366ee-103">获取 bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="366ee-103">Get bookingCurrency</span></span>

<span data-ttu-id="366ee-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="366ee-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="366ee-105">获取可用于 Microsoft 预订业务的[bookingCurrency](../resources/bookingcurrency.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="366ee-105">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="366ee-106">使用**id**属性（即货币代码）指定货币。</span><span class="sxs-lookup"><span data-stu-id="366ee-106">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="366ee-107">权限</span><span class="sxs-lookup"><span data-stu-id="366ee-107">Permissions</span></span>
<span data-ttu-id="366ee-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="366ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="366ee-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="366ee-110">Permission type</span></span>      | <span data-ttu-id="366ee-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="366ee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="366ee-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="366ee-112">Delegated (work or school account)</span></span> | <span data-ttu-id="366ee-113">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="366ee-113">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="366ee-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="366ee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="366ee-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="366ee-115">Not supported.</span></span>   |
|<span data-ttu-id="366ee-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="366ee-116">Application</span></span> | <span data-ttu-id="366ee-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="366ee-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="366ee-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="366ee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="366ee-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="366ee-119">Optional query parameters</span></span>
<span data-ttu-id="366ee-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="366ee-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="366ee-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="366ee-121">Request headers</span></span>
| <span data-ttu-id="366ee-122">名称</span><span class="sxs-lookup"><span data-stu-id="366ee-122">Name</span></span>      |<span data-ttu-id="366ee-123">说明</span><span class="sxs-lookup"><span data-stu-id="366ee-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="366ee-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="366ee-124">Authorization</span></span>  | <span data-ttu-id="366ee-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="366ee-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="366ee-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="366ee-126">Request body</span></span>
<span data-ttu-id="366ee-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="366ee-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="366ee-128">响应</span><span class="sxs-lookup"><span data-stu-id="366ee-128">Response</span></span>
<span data-ttu-id="366ee-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[bookingCurrency](../resources/bookingcurrency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="366ee-129">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="366ee-130">示例</span><span class="sxs-lookup"><span data-stu-id="366ee-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="366ee-131">请求</span><span class="sxs-lookup"><span data-stu-id="366ee-131">Request</span></span>
<span data-ttu-id="366ee-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="366ee-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="366ee-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="366ee-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
# <a name="c"></a>[<span data-ttu-id="366ee-134">C#</span><span class="sxs-lookup"><span data-stu-id="366ee-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcurrency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="366ee-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="366ee-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcurrency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="366ee-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="366ee-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcurrency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="366ee-137">响应</span><span class="sxs-lookup"><span data-stu-id="366ee-137">Response</span></span>
<span data-ttu-id="366ee-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="366ee-138">The following is an example of the response.</span></span> <span data-ttu-id="366ee-139">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="366ee-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="366ee-140">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="366ee-140">All of the properties will be returned from an actual call.</span></span>
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
