---
title: 获取 bookingCurrency
description: 获取可用于 Microsoft 预订业务的 bookingCurrency 对象的属性。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 3d7dcc7abace1963b865638b66bb6dcf25f48723
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313175"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="9bd49-103">获取 bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="9bd49-103">Get bookingCurrency</span></span>

<span data-ttu-id="9bd49-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bd49-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bd49-105">获取可用于 Microsoft 预订业务的 [bookingCurrency](../resources/bookingcurrency.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9bd49-105">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="9bd49-106">使用 **id** 属性（即货币代码）指定货币。</span><span class="sxs-lookup"><span data-stu-id="9bd49-106">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="9bd49-107">权限</span><span class="sxs-lookup"><span data-stu-id="9bd49-107">Permissions</span></span>
<span data-ttu-id="9bd49-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9bd49-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bd49-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9bd49-110">Permission type</span></span>      | <span data-ttu-id="9bd49-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9bd49-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bd49-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9bd49-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9bd49-113">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="9bd49-113">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="9bd49-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9bd49-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bd49-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bd49-115">Not supported.</span></span>   |
|<span data-ttu-id="9bd49-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9bd49-116">Application</span></span> | <span data-ttu-id="9bd49-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bd49-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9bd49-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9bd49-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9bd49-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9bd49-119">Optional query parameters</span></span>
<span data-ttu-id="9bd49-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9bd49-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9bd49-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="9bd49-121">Request headers</span></span>
| <span data-ttu-id="9bd49-122">名称</span><span class="sxs-lookup"><span data-stu-id="9bd49-122">Name</span></span>      |<span data-ttu-id="9bd49-123">说明</span><span class="sxs-lookup"><span data-stu-id="9bd49-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9bd49-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bd49-124">Authorization</span></span>  | <span data-ttu-id="9bd49-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9bd49-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bd49-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9bd49-126">Request body</span></span>
<span data-ttu-id="9bd49-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9bd49-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9bd49-128">响应</span><span class="sxs-lookup"><span data-stu-id="9bd49-128">Response</span></span>
<span data-ttu-id="9bd49-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [bookingCurrency](../resources/bookingcurrency.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9bd49-129">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9bd49-130">示例</span><span class="sxs-lookup"><span data-stu-id="9bd49-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9bd49-131">请求</span><span class="sxs-lookup"><span data-stu-id="9bd49-131">Request</span></span>
<span data-ttu-id="9bd49-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9bd49-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9bd49-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bd49-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
# <a name="c"></a>[<span data-ttu-id="9bd49-134">C#</span><span class="sxs-lookup"><span data-stu-id="9bd49-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcurrency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9bd49-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bd49-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcurrency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9bd49-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9bd49-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcurrency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9bd49-137">响应</span><span class="sxs-lookup"><span data-stu-id="9bd49-137">Response</span></span>
<span data-ttu-id="9bd49-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9bd49-138">The following is an example of the response.</span></span> <span data-ttu-id="9bd49-139">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9bd49-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9bd49-140">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9bd49-140">All of the properties will be returned from an actual call.</span></span>
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