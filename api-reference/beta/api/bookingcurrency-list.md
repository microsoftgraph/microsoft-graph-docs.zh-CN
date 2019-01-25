---
title: 列表 bookingCurrencies
description: 获取供 Microsoft 预订业务 bookingCurrency 对象的列表。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c29ad5780deac5e5e338052c72661f834e483054
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513219"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="75900-103">列表 bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="75900-103">List bookingCurrencies</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75900-104">获取供 Microsoft 预订业务[bookingCurrency](../resources/bookingcurrency.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="75900-104">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="75900-105">权限</span><span class="sxs-lookup"><span data-stu-id="75900-105">Permissions</span></span>
<span data-ttu-id="75900-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75900-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75900-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="75900-108">Permission type</span></span>      | <span data-ttu-id="75900-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="75900-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75900-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75900-110">Delegated (work or school account)</span></span> | <span data-ttu-id="75900-111">Bookings.Read.All，BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="75900-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="75900-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75900-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75900-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="75900-113">Not supported.</span></span>   |
|<span data-ttu-id="75900-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="75900-114">Application</span></span> | <span data-ttu-id="75900-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="75900-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="75900-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75900-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="75900-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="75900-117">Optional query parameters</span></span>
<span data-ttu-id="75900-118">此方法支持用于帮助自定义的响应，其中包括 $count、 $filter、 $select、 $skip 和 $top 的[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="75900-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75900-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="75900-119">Request headers</span></span>
| <span data-ttu-id="75900-120">名称</span><span class="sxs-lookup"><span data-stu-id="75900-120">Name</span></span>      |<span data-ttu-id="75900-121">说明</span><span class="sxs-lookup"><span data-stu-id="75900-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="75900-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="75900-122">Authorization</span></span>  | <span data-ttu-id="75900-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="75900-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="75900-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="75900-124">Request body</span></span>
<span data-ttu-id="75900-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="75900-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="75900-126">响应</span><span class="sxs-lookup"><span data-stu-id="75900-126">Response</span></span>
<span data-ttu-id="75900-127">如果成功，此方法返回`200 OK`响应代码和响应正文中的[bookingCurrency](../resources/bookingcurrency.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="75900-127">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="75900-128">示例</span><span class="sxs-lookup"><span data-stu-id="75900-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75900-129">请求</span><span class="sxs-lookup"><span data-stu-id="75900-129">Request</span></span>
<span data-ttu-id="75900-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="75900-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
##### <a name="response"></a><span data-ttu-id="75900-131">响应</span><span class="sxs-lookup"><span data-stu-id="75900-131">Response</span></span>
<span data-ttu-id="75900-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="75900-132">The following is an example of the response.</span></span> <span data-ttu-id="75900-133">注意： 为了简单起见截断如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="75900-133">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="75900-134">从实际的呼叫，将返回所有的受支持的货币和属性。</span><span class="sxs-lookup"><span data-stu-id="75900-134">All of the supported currencies and properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingcurrency-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
