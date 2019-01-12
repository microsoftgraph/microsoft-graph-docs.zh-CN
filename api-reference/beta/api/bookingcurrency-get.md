---
title: 获取 bookingCurrency
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f408ab0110de5124bb4154d0107c801b026de29a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926349"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="cc7c1-104">获取 bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="cc7c1-104">Get bookingCurrency</span></span>

 > <span data-ttu-id="cc7c1-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cc7c1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc7c1-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cc7c1-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="cc7c1-107">获取可供 Microsoft 预订业务[bookingCurrency](../resources/bookingcurrency.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cc7c1-107">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="cc7c1-108">**Id**属性，它是货币代码，用于指定货币。</span><span class="sxs-lookup"><span data-stu-id="cc7c1-108">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc7c1-109">权限</span><span class="sxs-lookup"><span data-stu-id="cc7c1-109">Permissions</span></span>
<span data-ttu-id="cc7c1-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc7c1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc7c1-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc7c1-112">Permission type</span></span>      | <span data-ttu-id="cc7c1-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cc7c1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc7c1-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc7c1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cc7c1-115">Bookings.Read.All，BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="cc7c1-115">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="cc7c1-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc7c1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc7c1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc7c1-117">Not supported.</span></span>   |
|<span data-ttu-id="cc7c1-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc7c1-118">Application</span></span> | <span data-ttu-id="cc7c1-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc7c1-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="cc7c1-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc7c1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cc7c1-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cc7c1-121">Optional query parameters</span></span>
<span data-ttu-id="cc7c1-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cc7c1-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc7c1-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc7c1-123">Request headers</span></span>
| <span data-ttu-id="cc7c1-124">名称</span><span class="sxs-lookup"><span data-stu-id="cc7c1-124">Name</span></span>      |<span data-ttu-id="cc7c1-125">说明</span><span class="sxs-lookup"><span data-stu-id="cc7c1-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cc7c1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc7c1-126">Authorization</span></span>  | <span data-ttu-id="cc7c1-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="cc7c1-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc7c1-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc7c1-128">Request body</span></span>
<span data-ttu-id="cc7c1-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cc7c1-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="cc7c1-130">响应</span><span class="sxs-lookup"><span data-stu-id="cc7c1-130">Response</span></span>
<span data-ttu-id="cc7c1-131">如果成功，此方法返回`200 OK`响应正文中的响应代码和[bookingCurrency](../resources/bookingcurrency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cc7c1-131">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cc7c1-132">示例</span><span class="sxs-lookup"><span data-stu-id="cc7c1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc7c1-133">请求</span><span class="sxs-lookup"><span data-stu-id="cc7c1-133">Request</span></span>
<span data-ttu-id="cc7c1-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cc7c1-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
##### <a name="response"></a><span data-ttu-id="cc7c1-135">响应</span><span class="sxs-lookup"><span data-stu-id="cc7c1-135">Response</span></span>
<span data-ttu-id="cc7c1-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cc7c1-136">The following is an example of the response.</span></span> <span data-ttu-id="cc7c1-137">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cc7c1-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cc7c1-138">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cc7c1-138">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingCurrency",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
