---
title: bookingBusiness：取消发布
description: 使此业务的计划页对外部客户不可用。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 52886df6aebcab14bbf8b2983e21e0866d56b403
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786255"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="5caed-103">bookingBusiness：取消发布</span><span class="sxs-lookup"><span data-stu-id="5caed-103">bookingBusiness: unpublish</span></span>

<span data-ttu-id="5caed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5caed-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5caed-105">使此业务的计划页对外部客户不可用。</span><span class="sxs-lookup"><span data-stu-id="5caed-105">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="5caed-106">将 **isPublished** 属性设置为 false，将 **publicUrl** 属性设置为 null。</span><span class="sxs-lookup"><span data-stu-id="5caed-106">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="5caed-107">权限</span><span class="sxs-lookup"><span data-stu-id="5caed-107">Permissions</span></span>
<span data-ttu-id="5caed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5caed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5caed-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5caed-110">Permission type</span></span>      | <span data-ttu-id="5caed-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5caed-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5caed-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5caed-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="5caed-113">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="5caed-113">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="5caed-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5caed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5caed-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5caed-115">Not supported.</span></span>   |
|<span data-ttu-id="5caed-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5caed-116">Application</span></span> | <span data-ttu-id="5caed-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5caed-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5caed-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5caed-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="5caed-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5caed-119">Request headers</span></span>
| <span data-ttu-id="5caed-120">名称</span><span class="sxs-lookup"><span data-stu-id="5caed-120">Name</span></span>       | <span data-ttu-id="5caed-121">说明</span><span class="sxs-lookup"><span data-stu-id="5caed-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5caed-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5caed-122">Authorization</span></span>  | <span data-ttu-id="5caed-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5caed-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5caed-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="5caed-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5caed-125">响应</span><span class="sxs-lookup"><span data-stu-id="5caed-125">Response</span></span>
<span data-ttu-id="5caed-p102">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5caed-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5caed-128">示例</span><span class="sxs-lookup"><span data-stu-id="5caed-128">Example</span></span>
<span data-ttu-id="5caed-129">下面是如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5caed-129">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5caed-130">请求</span><span class="sxs-lookup"><span data-stu-id="5caed-130">Request</span></span>
<span data-ttu-id="5caed-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5caed-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5caed-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5caed-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```
# <a name="c"></a>[<span data-ttu-id="5caed-133">C#</span><span class="sxs-lookup"><span data-stu-id="5caed-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-unpublish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5caed-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5caed-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-unpublish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5caed-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5caed-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-unpublish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5caed-136">Java</span><span class="sxs-lookup"><span data-stu-id="5caed-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingbusiness-unpublish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5caed-137">响应</span><span class="sxs-lookup"><span data-stu-id="5caed-137">Response</span></span>
<span data-ttu-id="5caed-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5caed-138">The following is an example of the response.</span></span>
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
  "description": "bookingBusiness: unpublish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


