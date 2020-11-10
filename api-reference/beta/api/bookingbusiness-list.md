---
title: 列出 Errorexceededfindcountlimit
description: 获取已为租户创建的 bookingbusiness 对象的集合。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: c1cf4042fbfbbc3364756c9363555215bff05e01
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960772"
---
# <a name="list-bookingbusinesses"></a><span data-ttu-id="2e4da-103">列出 Errorexceededfindcountlimit</span><span class="sxs-lookup"><span data-stu-id="2e4da-103">List bookingBusinesses</span></span>

<span data-ttu-id="2e4da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e4da-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e4da-105">获取已为租户创建的 [bookingbusiness](../resources/bookingbusiness.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="2e4da-105">Get a collection of [bookingbusiness](../resources/bookingbusiness.md) objects that has been created for the tenant.</span></span>

<span data-ttu-id="2e4da-106">此操作仅返回集合中每个预订业务的 **id** 和 **displayName** 。</span><span class="sxs-lookup"><span data-stu-id="2e4da-106">This operation returns only the **id** and **displayName** of each Bookings business in the collection.</span></span> <span data-ttu-id="2e4da-107">出于性能考虑，它不返回其他属性。</span><span class="sxs-lookup"><span data-stu-id="2e4da-107">For performance considerations, it does not return other properties.</span></span> <span data-ttu-id="2e4da-108">您可以通过在 [get](bookingbusiness-get.md)操作中指定其 **Id** 来获取预订业务的其他属性。</span><span class="sxs-lookup"><span data-stu-id="2e4da-108">You can get the other properties of a Bookings business by specifying its **id** in a [GET](bookingbusiness-get.md) operation.</span></span>

<span data-ttu-id="2e4da-109">您还可以通过在参数中指定字符串 `query` 以执行租户的业务中的子字符串匹配，从而查询预订业务。</span><span class="sxs-lookup"><span data-stu-id="2e4da-109">You can also query for Bookings businesses by specifying a string in a `query` parameter to do substring matching among the businesses of a tenant.</span></span> <span data-ttu-id="2e4da-110">请参阅以下[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="2e4da-110">See an [example](#request-2) below.</span></span>


## <a name="permissions"></a><span data-ttu-id="2e4da-111">权限</span><span class="sxs-lookup"><span data-stu-id="2e4da-111">Permissions</span></span>
<span data-ttu-id="2e4da-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e4da-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e4da-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e4da-114">Permission type</span></span>      | <span data-ttu-id="2e4da-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2e4da-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e4da-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e4da-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="2e4da-117">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="2e4da-117">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="2e4da-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e4da-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e4da-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e4da-119">Not supported.</span></span>   |
|<span data-ttu-id="2e4da-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e4da-120">Application</span></span> | <span data-ttu-id="2e4da-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e4da-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="2e4da-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e4da-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2e4da-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2e4da-123">Optional query parameters</span></span>
<span data-ttu-id="2e4da-124">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2e4da-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="2e4da-125">此方法还支持 `query` 接受字符串值的参数。</span><span class="sxs-lookup"><span data-stu-id="2e4da-125">This method also supports the `query` parameter which accepts a string value.</span></span> <span data-ttu-id="2e4da-126">此参数将 GET 结果限制为与指定的字符串匹配的企业。</span><span class="sxs-lookup"><span data-stu-id="2e4da-126">This parameter limits the GET results to businesses that match the specified string.</span></span> <span data-ttu-id="2e4da-127">您可以参阅下面的 [示例](#request-2) 。</span><span class="sxs-lookup"><span data-stu-id="2e4da-127">You can see an [example](#request-2) below.</span></span>


## <a name="request-headers"></a><span data-ttu-id="2e4da-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e4da-128">Request headers</span></span>
| <span data-ttu-id="2e4da-129">名称</span><span class="sxs-lookup"><span data-stu-id="2e4da-129">Name</span></span>      |<span data-ttu-id="2e4da-130">说明</span><span class="sxs-lookup"><span data-stu-id="2e4da-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2e4da-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e4da-131">Authorization</span></span>  | <span data-ttu-id="2e4da-132">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2e4da-132">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e4da-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e4da-133">Request body</span></span>
<span data-ttu-id="2e4da-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2e4da-134">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2e4da-135">响应</span><span class="sxs-lookup"><span data-stu-id="2e4da-135">Response</span></span>
<span data-ttu-id="2e4da-136">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [bookingBusiness](../resources/bookingbusiness.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2e4da-136">If successful, this method returns a `200 OK` response code and collection of [bookingBusiness](../resources/bookingbusiness.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2e4da-137">示例</span><span class="sxs-lookup"><span data-stu-id="2e4da-137">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="2e4da-138">请求 1</span><span class="sxs-lookup"><span data-stu-id="2e4da-138">Request 1</span></span>
<span data-ttu-id="2e4da-139">下面的示例获取租户中的预订企业。</span><span class="sxs-lookup"><span data-stu-id="2e4da-139">The following example gets the Bookings businesses in a tenant.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e4da-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e4da-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses
```
# <a name="c"></a>[<span data-ttu-id="2e4da-141">C#</span><span class="sxs-lookup"><span data-stu-id="2e4da-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingbusinesses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e4da-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e4da-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingbusinesses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e4da-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e4da-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingbusinesses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e4da-144">Java</span><span class="sxs-lookup"><span data-stu-id="2e4da-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingbusinesses-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="2e4da-145">响应 1</span><span class="sxs-lookup"><span data-stu-id="2e4da-145">Response 1</span></span>
<span data-ttu-id="2e4da-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2e4da-146">The following is an example of the response.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="2e4da-147">请求 2</span><span class="sxs-lookup"><span data-stu-id="2e4da-147">Request 2</span></span>
<span data-ttu-id="2e4da-148">下面的示例演示如何使用参数在 `query` 租户中获取一个或多个匹配的预订企业。</span><span class="sxs-lookup"><span data-stu-id="2e4da-148">The following example shows how to use the `query` parameter to get one or more matching Bookings businesses in the tenant.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e4da-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e4da-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
# <a name="c"></a>[<span data-ttu-id="2e4da-150">C#</span><span class="sxs-lookup"><span data-stu-id="2e4da-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/query-bookingbusinesses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e4da-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e4da-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/query-bookingbusinesses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e4da-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e4da-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/query-bookingbusinesses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e4da-153">Java</span><span class="sxs-lookup"><span data-stu-id="2e4da-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/query-bookingbusinesses-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="2e4da-154">响应 2</span><span class="sxs-lookup"><span data-stu-id="2e4da-154">Response 2</span></span>
<span data-ttu-id="2e4da-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2e4da-155">The following is an example of the response.</span></span>
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
  "suppressions": [
  ]
}
-->
