---
title: 删除 bookingBusiness
description: 删除 bookingBusiness 对象。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 1067a26591747be3f08f0c92855543e33f399fe6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960907"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="b3be0-103">删除 bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="b3be0-103">Delete bookingBusiness</span></span>

<span data-ttu-id="b3be0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3be0-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3be0-105">删除 [bookingBusiness](../resources/bookingbusiness.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b3be0-105">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b3be0-106">权限</span><span class="sxs-lookup"><span data-stu-id="b3be0-106">Permissions</span></span>
<span data-ttu-id="b3be0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3be0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3be0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3be0-109">Permission type</span></span>      | <span data-ttu-id="b3be0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b3be0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3be0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3be0-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="b3be0-112">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="b3be0-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="b3be0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3be0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3be0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3be0-114">Not supported.</span></span>   |
|<span data-ttu-id="b3be0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3be0-115">Application</span></span> | <span data-ttu-id="b3be0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3be0-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="b3be0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3be0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}

```
## <a name="request-headers"></a><span data-ttu-id="b3be0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3be0-118">Request headers</span></span>
| <span data-ttu-id="b3be0-119">名称</span><span class="sxs-lookup"><span data-stu-id="b3be0-119">Name</span></span>       | <span data-ttu-id="b3be0-120">说明</span><span class="sxs-lookup"><span data-stu-id="b3be0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b3be0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3be0-121">Authorization</span></span>  | <span data-ttu-id="b3be0-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b3be0-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3be0-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3be0-123">Request body</span></span>
<span data-ttu-id="b3be0-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b3be0-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b3be0-125">响应</span><span class="sxs-lookup"><span data-stu-id="b3be0-125">Response</span></span>
<span data-ttu-id="b3be0-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b3be0-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3be0-128">示例</span><span class="sxs-lookup"><span data-stu-id="b3be0-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3be0-129">请求</span><span class="sxs-lookup"><span data-stu-id="b3be0-129">Request</span></span>
<span data-ttu-id="b3be0-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b3be0-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b3be0-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3be0-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
# <a name="c"></a>[<span data-ttu-id="b3be0-132">C#</span><span class="sxs-lookup"><span data-stu-id="b3be0-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3be0-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3be0-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3be0-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3be0-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3be0-135">Java</span><span class="sxs-lookup"><span data-stu-id="b3be0-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b3be0-136">响应</span><span class="sxs-lookup"><span data-stu-id="b3be0-136">Response</span></span>
<span data-ttu-id="b3be0-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b3be0-137">The following is an example of the response.</span></span>
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


