---
title: bookingBusiness：发布
description: 使此业务的日程安排页面对外部客户可用。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: a29904342e44a7642335333fa39f95866df1609d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988003"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="71664-103">bookingBusiness：发布</span><span class="sxs-lookup"><span data-stu-id="71664-103">bookingBusiness: publish</span></span>

<span data-ttu-id="71664-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71664-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71664-105">使此业务的日程安排页面对外部客户可用。</span><span class="sxs-lookup"><span data-stu-id="71664-105">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="71664-106">将 **isPublished** 属性设置为 true，并将 **publicUrl** 属性设置为计划页面的 URL。</span><span class="sxs-lookup"><span data-stu-id="71664-106">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="71664-107">权限</span><span class="sxs-lookup"><span data-stu-id="71664-107">Permissions</span></span>
<span data-ttu-id="71664-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71664-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71664-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="71664-110">Permission type</span></span>      | <span data-ttu-id="71664-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71664-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71664-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71664-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="71664-113">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="71664-113">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="71664-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71664-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71664-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="71664-115">Not supported.</span></span>   |
|<span data-ttu-id="71664-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="71664-116">Application</span></span> | <span data-ttu-id="71664-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="71664-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="71664-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71664-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="71664-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="71664-119">Request headers</span></span>
| <span data-ttu-id="71664-120">名称</span><span class="sxs-lookup"><span data-stu-id="71664-120">Name</span></span>       | <span data-ttu-id="71664-121">说明</span><span class="sxs-lookup"><span data-stu-id="71664-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="71664-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71664-122">Authorization</span></span>  | <span data-ttu-id="71664-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="71664-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="71664-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="71664-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="71664-125">响应</span><span class="sxs-lookup"><span data-stu-id="71664-125">Response</span></span>
<span data-ttu-id="71664-p102">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="71664-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71664-128">示例</span><span class="sxs-lookup"><span data-stu-id="71664-128">Example</span></span>
<span data-ttu-id="71664-129">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="71664-129">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="71664-130">请求</span><span class="sxs-lookup"><span data-stu-id="71664-130">Request</span></span>
<span data-ttu-id="71664-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="71664-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="71664-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="71664-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```
# <a name="c"></a>[<span data-ttu-id="71664-133">C#</span><span class="sxs-lookup"><span data-stu-id="71664-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71664-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71664-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71664-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71664-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="71664-136">响应</span><span class="sxs-lookup"><span data-stu-id="71664-136">Response</span></span>
<span data-ttu-id="71664-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="71664-137">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
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


