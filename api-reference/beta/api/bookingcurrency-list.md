---
title: 列表 bookingCurrencies
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 809ee9222f8ae997633becbe13f87539dd816b1f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849215"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="2cb97-104">列表 bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="2cb97-104">List bookingCurrencies</span></span>

 > <span data-ttu-id="2cb97-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2cb97-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2cb97-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2cb97-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="2cb97-107">获取供 Microsoft 预订业务[bookingCurrency](../resources/bookingcurrency.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="2cb97-107">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="2cb97-108">权限</span><span class="sxs-lookup"><span data-stu-id="2cb97-108">Permissions</span></span>
<span data-ttu-id="2cb97-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2cb97-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cb97-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2cb97-111">Permission type</span></span>      | <span data-ttu-id="2cb97-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2cb97-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2cb97-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2cb97-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2cb97-114">Bookings.Read.All，BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="2cb97-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="2cb97-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2cb97-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2cb97-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2cb97-116">Not supported.</span></span>   |
|<span data-ttu-id="2cb97-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2cb97-117">Application</span></span> | <span data-ttu-id="2cb97-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2cb97-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="2cb97-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2cb97-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2cb97-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2cb97-120">Optional query parameters</span></span>
<span data-ttu-id="2cb97-121">此方法支持用于帮助自定义的响应，其中包括 $count、 $filter、 $select、 $skip 和 $top 的[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="2cb97-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2cb97-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="2cb97-122">Request headers</span></span>
| <span data-ttu-id="2cb97-123">名称</span><span class="sxs-lookup"><span data-stu-id="2cb97-123">Name</span></span>      |<span data-ttu-id="2cb97-124">说明</span><span class="sxs-lookup"><span data-stu-id="2cb97-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2cb97-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cb97-125">Authorization</span></span>  | <span data-ttu-id="2cb97-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2cb97-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cb97-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2cb97-127">Request body</span></span>
<span data-ttu-id="2cb97-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2cb97-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2cb97-129">响应</span><span class="sxs-lookup"><span data-stu-id="2cb97-129">Response</span></span>
<span data-ttu-id="2cb97-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[bookingCurrency](../resources/bookingcurrency.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="2cb97-130">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2cb97-131">示例</span><span class="sxs-lookup"><span data-stu-id="2cb97-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2cb97-132">请求</span><span class="sxs-lookup"><span data-stu-id="2cb97-132">Request</span></span>
<span data-ttu-id="2cb97-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2cb97-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
##### <a name="response"></a><span data-ttu-id="2cb97-134">响应</span><span class="sxs-lookup"><span data-stu-id="2cb97-134">Response</span></span>
<span data-ttu-id="2cb97-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2cb97-135">The following is an example of the response.</span></span> <span data-ttu-id="2cb97-136">注意： 为了简单起见截断如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2cb97-136">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="2cb97-137">从实际的呼叫，将返回所有的受支持的货币和属性。</span><span class="sxs-lookup"><span data-stu-id="2cb97-137">All of the supported currencies and properties will be returned from an actual call.</span></span>
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
