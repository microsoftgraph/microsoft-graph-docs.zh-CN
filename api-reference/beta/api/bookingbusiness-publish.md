---
title: bookingBusiness：发布
description: 使外部客户可以使用此业务的计划页。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: d60a88324cd86cd599fc9986dfa3b6d1a4f737ea
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786585"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="db123-103">bookingBusiness：发布</span><span class="sxs-lookup"><span data-stu-id="db123-103">bookingBusiness: publish</span></span>

<span data-ttu-id="db123-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db123-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db123-105">使外部客户可以使用此业务的计划页。</span><span class="sxs-lookup"><span data-stu-id="db123-105">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="db123-106">将 **isPublished** 属性设置为 true，将 **publicUrl** 属性设置为计划页的 URL。</span><span class="sxs-lookup"><span data-stu-id="db123-106">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="db123-107">权限</span><span class="sxs-lookup"><span data-stu-id="db123-107">Permissions</span></span>
<span data-ttu-id="db123-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db123-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db123-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="db123-110">Permission type</span></span>      | <span data-ttu-id="db123-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db123-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db123-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db123-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="db123-113">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="db123-113">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="db123-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db123-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db123-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="db123-115">Not supported.</span></span>   |
|<span data-ttu-id="db123-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="db123-116">Application</span></span> | <span data-ttu-id="db123-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="db123-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="db123-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db123-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="db123-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="db123-119">Request headers</span></span>
| <span data-ttu-id="db123-120">名称</span><span class="sxs-lookup"><span data-stu-id="db123-120">Name</span></span>       | <span data-ttu-id="db123-121">说明</span><span class="sxs-lookup"><span data-stu-id="db123-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="db123-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db123-122">Authorization</span></span>  | <span data-ttu-id="db123-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="db123-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="db123-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="db123-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="db123-125">响应</span><span class="sxs-lookup"><span data-stu-id="db123-125">Response</span></span>
<span data-ttu-id="db123-p102">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="db123-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db123-128">示例</span><span class="sxs-lookup"><span data-stu-id="db123-128">Example</span></span>
<span data-ttu-id="db123-129">下面是如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="db123-129">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="db123-130">请求</span><span class="sxs-lookup"><span data-stu-id="db123-130">Request</span></span>
<span data-ttu-id="db123-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="db123-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db123-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="db123-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```
# <a name="c"></a>[<span data-ttu-id="db123-133">C#</span><span class="sxs-lookup"><span data-stu-id="db123-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db123-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db123-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db123-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db123-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db123-136">Java</span><span class="sxs-lookup"><span data-stu-id="db123-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingbusiness-publish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="db123-137">响应</span><span class="sxs-lookup"><span data-stu-id="db123-137">Response</span></span>
<span data-ttu-id="db123-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="db123-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingBusiness: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


