---
title: 列表 bookingBusinesses
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 270bda6aca601951ea56a9ddf9364d1459496699
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849208"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="d24a5-104">列表 bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="d24a5-104">List bookingBusinesses</span></span>

 > <span data-ttu-id="d24a5-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d24a5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d24a5-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d24a5-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="d24a5-107">获取租户已创建[bookingbusiness](../resources/bookingbusiness.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="d24a5-107">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span> 

<span data-ttu-id="d24a5-108">此操作返回集合中的**id**和的每个预订业务的**displayName** 。</span><span class="sxs-lookup"><span data-stu-id="d24a5-108">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="d24a5-109">出于性能考虑，它不返回其他属性。</span><span class="sxs-lookup"><span data-stu-id="d24a5-109">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="d24a5-110">您可以通过[GET](bookingbusiness-get.md)操作中指定其**id**获取预订业务的其他属性。</span><span class="sxs-lookup"><span data-stu-id="d24a5-110">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="d24a5-111">此外可以通过指定的字符串中查询的预订企业`query`参数执行子字符串匹配的租户企业之间。</span><span class="sxs-lookup"><span data-stu-id="d24a5-111">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="d24a5-112">请参阅下面[的示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="d24a5-112">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="d24a5-113">权限</span><span class="sxs-lookup"><span data-stu-id="d24a5-113">Permissions</span></span>
<span data-ttu-id="d24a5-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d24a5-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d24a5-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="d24a5-116">Permission type</span></span>      | <span data-ttu-id="d24a5-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d24a5-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d24a5-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d24a5-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="d24a5-119">Bookings.Read.All，BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="d24a5-119">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d24a5-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d24a5-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d24a5-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="d24a5-121">Not supported.</span></span>   |
|<span data-ttu-id="d24a5-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="d24a5-122">Application</span></span> | <span data-ttu-id="d24a5-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="d24a5-123">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="d24a5-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d24a5-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d24a5-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d24a5-125">Optional query parameters</span></span>
<span data-ttu-id="d24a5-126">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d24a5-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d24a5-127">此方法还支持`query`参数接受一个字符串值。</span><span class="sxs-lookup"><span data-stu-id="d24a5-127">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="d24a5-128">此参数获取将结果限制为与指定的字符串匹配的企业。</span><span class="sxs-lookup"><span data-stu-id="d24a5-128">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="d24a5-129">您可以看到下面[的示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="d24a5-129">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="d24a5-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="d24a5-130">Request headers</span></span>
| <span data-ttu-id="d24a5-131">名称</span><span class="sxs-lookup"><span data-stu-id="d24a5-131">Name</span></span>      |<span data-ttu-id="d24a5-132">说明</span><span class="sxs-lookup"><span data-stu-id="d24a5-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d24a5-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="d24a5-133">Authorization</span></span>  | <span data-ttu-id="d24a5-134">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d24a5-134">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d24a5-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="d24a5-135">Request body</span></span>
<span data-ttu-id="d24a5-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d24a5-136">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d24a5-137">响应</span><span class="sxs-lookup"><span data-stu-id="d24a5-137">Response</span></span>
<span data-ttu-id="d24a5-138">如果成功，此方法返回`200 OK`响应代码和响应正文中的[bookingBusiness](../resources/bookingbusiness.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="d24a5-138">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d24a5-139">示例</span><span class="sxs-lookup"><span data-stu-id="d24a5-139">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="d24a5-140">请求 1</span><span class="sxs-lookup"><span data-stu-id="d24a5-140">Request 1</span></span>
<span data-ttu-id="d24a5-141">下面的示例获取租户中的预定企业。</span><span class="sxs-lookup"><span data-stu-id="d24a5-141">The following example gets the Bookings businesses in a tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
```
##### <a name="response-1"></a><span data-ttu-id="d24a5-142">响应 1</span><span class="sxs-lookup"><span data-stu-id="d24a5-142">Response 1</span></span>
<span data-ttu-id="d24a5-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d24a5-143">The following is an example of the response.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="d24a5-144">请求 2</span><span class="sxs-lookup"><span data-stu-id="d24a5-144">Request 2</span></span>
<span data-ttu-id="d24a5-145">下面的示例演示如何使用`query`参数获取租户中的一个或多个匹配预订企业。</span><span class="sxs-lookup"><span data-stu-id="d24a5-145">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
##### <a name="response-2"></a><span data-ttu-id="d24a5-146">响应 2</span><span class="sxs-lookup"><span data-stu-id="d24a5-146">Response 2</span></span>
<span data-ttu-id="d24a5-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d24a5-147">The following is an example of the response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List bookingBusinesses",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
