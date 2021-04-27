---
title: 获取 bookingCurrency
description: 获取可用于 Microsoft Bookings 业务的 bookingCurrency 对象的属性。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: f6702d108c3b705749021ad79d7e9fe6ceb944b1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047838"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="b70c5-103">获取 bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="b70c5-103">Get bookingCurrency</span></span>

<span data-ttu-id="b70c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b70c5-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b70c5-105">获取可用于 Microsoft Bookings 业务的 [bookingCurrency](../resources/bookingcurrency.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b70c5-105">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="b70c5-106">使用 **id** 属性（即货币代码）指定货币。</span><span class="sxs-lookup"><span data-stu-id="b70c5-106">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="b70c5-107">权限</span><span class="sxs-lookup"><span data-stu-id="b70c5-107">Permissions</span></span>
<span data-ttu-id="b70c5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b70c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b70c5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b70c5-110">Permission type</span></span>      | <span data-ttu-id="b70c5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b70c5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b70c5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b70c5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b70c5-113">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="b70c5-113">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="b70c5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b70c5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b70c5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b70c5-115">Not supported.</span></span>   |
|<span data-ttu-id="b70c5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b70c5-116">Application</span></span> | <span data-ttu-id="b70c5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b70c5-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="b70c5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b70c5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b70c5-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b70c5-119">Optional query parameters</span></span>
<span data-ttu-id="b70c5-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b70c5-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b70c5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b70c5-121">Request headers</span></span>
| <span data-ttu-id="b70c5-122">名称</span><span class="sxs-lookup"><span data-stu-id="b70c5-122">Name</span></span>      |<span data-ttu-id="b70c5-123">说明</span><span class="sxs-lookup"><span data-stu-id="b70c5-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b70c5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b70c5-124">Authorization</span></span>  | <span data-ttu-id="b70c5-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b70c5-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b70c5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b70c5-126">Request body</span></span>
<span data-ttu-id="b70c5-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b70c5-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b70c5-128">响应</span><span class="sxs-lookup"><span data-stu-id="b70c5-128">Response</span></span>
<span data-ttu-id="b70c5-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [bookingCurrency](../resources/bookingcurrency.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b70c5-129">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b70c5-130">示例</span><span class="sxs-lookup"><span data-stu-id="b70c5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b70c5-131">请求</span><span class="sxs-lookup"><span data-stu-id="b70c5-131">Request</span></span>
<span data-ttu-id="b70c5-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b70c5-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b70c5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b70c5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
# <a name="c"></a>[<span data-ttu-id="b70c5-134">C#</span><span class="sxs-lookup"><span data-stu-id="b70c5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcurrency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b70c5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b70c5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcurrency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b70c5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b70c5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcurrency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b70c5-137">Java</span><span class="sxs-lookup"><span data-stu-id="b70c5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingcurrency-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b70c5-138">响应</span><span class="sxs-lookup"><span data-stu-id="b70c5-138">Response</span></span>
<span data-ttu-id="b70c5-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b70c5-139">The following is an example of the response.</span></span> <span data-ttu-id="b70c5-140">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b70c5-140">Note: The response object shown here might be shortened for readability.</span></span>
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
