---
title: 'bookingBusiness: 发布'
description: 使此业务的日程安排页面对外部客户可用。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 03859185e2f43b471844ae7c4373d8b4a68ea348
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318220"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="31216-103">bookingBusiness: 发布</span><span class="sxs-lookup"><span data-stu-id="31216-103">bookingBusiness: publish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31216-104">使此业务的日程安排页面对外部客户可用。</span><span class="sxs-lookup"><span data-stu-id="31216-104">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="31216-105">将**isPublished**属性设置为 true, 并将**publicUrl**属性设置为计划页面的 URL。</span><span class="sxs-lookup"><span data-stu-id="31216-105">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="31216-106">权限</span><span class="sxs-lookup"><span data-stu-id="31216-106">Permissions</span></span>
<span data-ttu-id="31216-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31216-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31216-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="31216-109">Permission type</span></span>      | <span data-ttu-id="31216-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31216-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31216-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31216-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="31216-112">预订. 全部</span><span class="sxs-lookup"><span data-stu-id="31216-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="31216-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31216-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31216-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="31216-114">Not supported.</span></span>   |
|<span data-ttu-id="31216-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="31216-115">Application</span></span> | <span data-ttu-id="31216-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="31216-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="31216-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31216-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="31216-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="31216-118">Request headers</span></span>
| <span data-ttu-id="31216-119">名称</span><span class="sxs-lookup"><span data-stu-id="31216-119">Name</span></span>       | <span data-ttu-id="31216-120">说明</span><span class="sxs-lookup"><span data-stu-id="31216-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="31216-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="31216-121">Authorization</span></span>  | <span data-ttu-id="31216-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="31216-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="31216-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="31216-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="31216-124">响应</span><span class="sxs-lookup"><span data-stu-id="31216-124">Response</span></span>
<span data-ttu-id="31216-p102">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="31216-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31216-127">示例</span><span class="sxs-lookup"><span data-stu-id="31216-127">Example</span></span>
<span data-ttu-id="31216-128">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="31216-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="31216-129">请求</span><span class="sxs-lookup"><span data-stu-id="31216-129">Request</span></span>
<span data-ttu-id="31216-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="31216-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="31216-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="31216-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="31216-132">C#</span><span class="sxs-lookup"><span data-stu-id="31216-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="31216-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31216-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="31216-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="31216-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="31216-135">Java</span><span class="sxs-lookup"><span data-stu-id="31216-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingbusiness-publish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="31216-136">响应</span><span class="sxs-lookup"><span data-stu-id="31216-136">Response</span></span>
<span data-ttu-id="31216-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="31216-137">The following is an example of the response.</span></span>
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
