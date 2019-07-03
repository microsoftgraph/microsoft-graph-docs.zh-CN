---
title: 删除 bookingBusiness
description: 删除 bookingBusiness 对象。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 28bb8b19c4bd2fd20ec5f028357c81ccb52055f3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439327"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="f63b4-103">删除 bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="f63b4-103">Delete bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f63b4-104">删除[bookingBusiness](../resources/bookingbusiness.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f63b4-104">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f63b4-105">权限</span><span class="sxs-lookup"><span data-stu-id="f63b4-105">Permissions</span></span>
<span data-ttu-id="f63b4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f63b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f63b4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f63b4-108">Permission type</span></span>      | <span data-ttu-id="f63b4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f63b4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f63b4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f63b4-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f63b4-111">预订. 全部</span><span class="sxs-lookup"><span data-stu-id="f63b4-111">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f63b4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f63b4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f63b4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f63b4-113">Not supported.</span></span>   |
|<span data-ttu-id="f63b4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f63b4-114">Application</span></span> | <span data-ttu-id="f63b4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f63b4-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f63b4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f63b4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="f63b4-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f63b4-117">Request headers</span></span>
| <span data-ttu-id="f63b4-118">名称</span><span class="sxs-lookup"><span data-stu-id="f63b4-118">Name</span></span>       | <span data-ttu-id="f63b4-119">说明</span><span class="sxs-lookup"><span data-stu-id="f63b4-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f63b4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f63b4-120">Authorization</span></span>  | <span data-ttu-id="f63b4-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f63b4-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f63b4-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="f63b4-122">Request body</span></span>
<span data-ttu-id="f63b4-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f63b4-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f63b4-124">响应</span><span class="sxs-lookup"><span data-stu-id="f63b4-124">Response</span></span>
<span data-ttu-id="f63b4-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f63b4-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f63b4-127">示例</span><span class="sxs-lookup"><span data-stu-id="f63b4-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f63b4-128">请求</span><span class="sxs-lookup"><span data-stu-id="f63b4-128">Request</span></span>
<span data-ttu-id="f63b4-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f63b4-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f63b4-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f63b4-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f63b4-131">C#</span><span class="sxs-lookup"><span data-stu-id="f63b4-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f63b4-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="f63b4-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f63b4-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="f63b4-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f63b4-134">响应</span><span class="sxs-lookup"><span data-stu-id="f63b4-134">Response</span></span>
<span data-ttu-id="f63b4-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f63b4-135">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
