---
title: 删除 bookingBusiness
description: 删除 bookingBusiness 对象。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 80935b618ae4a6badadd5eb2bbc49199326c6e6f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43367411"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="b7922-103">删除 bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="b7922-103">Delete bookingBusiness</span></span>

<span data-ttu-id="b7922-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7922-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7922-105">删除[bookingBusiness](../resources/bookingbusiness.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b7922-105">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7922-106">权限</span><span class="sxs-lookup"><span data-stu-id="b7922-106">Permissions</span></span>
<span data-ttu-id="b7922-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7922-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7922-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7922-109">Permission type</span></span>      | <span data-ttu-id="b7922-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b7922-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7922-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7922-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="b7922-112">预订. 全部</span><span class="sxs-lookup"><span data-stu-id="b7922-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="b7922-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7922-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7922-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7922-114">Not supported.</span></span>   |
|<span data-ttu-id="b7922-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7922-115">Application</span></span> | <span data-ttu-id="b7922-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7922-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="b7922-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7922-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}

```
## <a name="request-headers"></a><span data-ttu-id="b7922-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7922-118">Request headers</span></span>
| <span data-ttu-id="b7922-119">名称</span><span class="sxs-lookup"><span data-stu-id="b7922-119">Name</span></span>       | <span data-ttu-id="b7922-120">说明</span><span class="sxs-lookup"><span data-stu-id="b7922-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b7922-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7922-121">Authorization</span></span>  | <span data-ttu-id="b7922-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b7922-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7922-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7922-123">Request body</span></span>
<span data-ttu-id="b7922-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b7922-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b7922-125">响应</span><span class="sxs-lookup"><span data-stu-id="b7922-125">Response</span></span>
<span data-ttu-id="b7922-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b7922-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7922-128">示例</span><span class="sxs-lookup"><span data-stu-id="b7922-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7922-129">请求</span><span class="sxs-lookup"><span data-stu-id="b7922-129">Request</span></span>
<span data-ttu-id="b7922-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b7922-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b7922-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7922-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
# <a name="c"></a>[<span data-ttu-id="b7922-132">C#</span><span class="sxs-lookup"><span data-stu-id="b7922-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b7922-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7922-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b7922-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7922-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b7922-135">响应</span><span class="sxs-lookup"><span data-stu-id="b7922-135">Response</span></span>
<span data-ttu-id="b7922-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b7922-136">The following is an example of the response.</span></span>
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
