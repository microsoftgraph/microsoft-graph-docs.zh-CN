---
title: 列出 errorexceededfindcountlimit
description: 获取已为租户创建的 bookingbusiness 对象的集合。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3836584a5968afb1d077546838c58836b1623166
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322587"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="99708-103">列出 errorexceededfindcountlimit</span><span class="sxs-lookup"><span data-stu-id="99708-103">List bookingBusinesses</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99708-104">获取已为租户创建的[bookingbusiness](../resources/bookingbusiness.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="99708-104">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span>

<span data-ttu-id="99708-105">此操作仅返回集合中每个预订业务的**id**和**displayName** 。</span><span class="sxs-lookup"><span data-stu-id="99708-105">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="99708-106">出于性能考虑, 它不返回其他属性。</span><span class="sxs-lookup"><span data-stu-id="99708-106">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="99708-107">您可以通过在[get](bookingbusiness-get.md)操作中指定其**id**来获取预订业务的其他属性。</span><span class="sxs-lookup"><span data-stu-id="99708-107">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="99708-108">您还可以通过在`query`参数中指定字符串以执行租户的业务中的子字符串匹配, 从而查询预订业务。</span><span class="sxs-lookup"><span data-stu-id="99708-108">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="99708-109">请参阅以下[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="99708-109">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="99708-110">权限</span><span class="sxs-lookup"><span data-stu-id="99708-110">Permissions</span></span>
<span data-ttu-id="99708-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99708-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99708-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="99708-113">Permission type</span></span>      | <span data-ttu-id="99708-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99708-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99708-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99708-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="99708-116">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="99708-116">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="99708-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99708-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99708-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="99708-118">Not supported.</span></span>   |
|<span data-ttu-id="99708-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="99708-119">Application</span></span> | <span data-ttu-id="99708-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="99708-120">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="99708-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99708-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="99708-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="99708-122">Optional query parameters</span></span>
<span data-ttu-id="99708-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="99708-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="99708-124">此方法还支持接受`query`字符串值的参数。</span><span class="sxs-lookup"><span data-stu-id="99708-124">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="99708-125">此参数将 GET 结果限制为与指定的字符串匹配的企业。</span><span class="sxs-lookup"><span data-stu-id="99708-125">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="99708-126">您可以参阅下面的[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="99708-126">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="99708-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="99708-127">Request headers</span></span>
| <span data-ttu-id="99708-128">名称</span><span class="sxs-lookup"><span data-stu-id="99708-128">Name</span></span>      |<span data-ttu-id="99708-129">说明</span><span class="sxs-lookup"><span data-stu-id="99708-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="99708-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="99708-130">Authorization</span></span>  | <span data-ttu-id="99708-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="99708-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="99708-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="99708-132">Request body</span></span>
<span data-ttu-id="99708-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="99708-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="99708-134">响应</span><span class="sxs-lookup"><span data-stu-id="99708-134">Response</span></span>
<span data-ttu-id="99708-135">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[bookingBusiness](../resources/bookingbusiness.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="99708-135">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="99708-136">示例</span><span class="sxs-lookup"><span data-stu-id="99708-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="99708-137">请求 1</span><span class="sxs-lookup"><span data-stu-id="99708-137">Request 1</span></span>
<span data-ttu-id="99708-138">下面的示例获取租户中的预订企业。</span><span class="sxs-lookup"><span data-stu-id="99708-138">The following example gets the Bookings businesses in a tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
```
##### <a name="response-1"></a><span data-ttu-id="99708-139">响应 1</span><span class="sxs-lookup"><span data-stu-id="99708-139">Response 1</span></span>
<span data-ttu-id="99708-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="99708-140">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"Contosolunchdelivery@M365B489948.onmicrosoft.com",
            "displayName":"Contoso lunch delivery",
        },
        {
            "id":"Fabrikam@M365B489948.onmicrosoft.com",
            "displayName":"Fabrikam",
        }
    ]
}
```


##### <a name="request-2"></a><span data-ttu-id="99708-141">请求 2</span><span class="sxs-lookup"><span data-stu-id="99708-141">Request 2</span></span>
<span data-ttu-id="99708-142">下面的示例演示如何使用`query`参数在租户中获取一个或多个匹配的预订企业。</span><span class="sxs-lookup"><span data-stu-id="99708-142">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
##### <a name="response-2"></a><span data-ttu-id="99708-143">响应 2</span><span class="sxs-lookup"><span data-stu-id="99708-143">Response 2</span></span>
<span data-ttu-id="99708-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="99708-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"AdventureWorksCycles@M365B960066.onmicrosoft.com",
            "displayName":"Adventure Works Cycles",
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List bookingBusinesses",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
