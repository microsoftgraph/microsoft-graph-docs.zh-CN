---
title: bookingBusiness：发布
description: 使此业务的日程安排页面对外部客户可用。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: a1f2a9bf6e7617cf991a37acada452c6c19b05d4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43382411"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="98318-103">bookingBusiness：发布</span><span class="sxs-lookup"><span data-stu-id="98318-103">bookingBusiness: publish</span></span>

<span data-ttu-id="98318-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98318-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98318-105">使此业务的日程安排页面对外部客户可用。</span><span class="sxs-lookup"><span data-stu-id="98318-105">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="98318-106">将**isPublished**属性设置为 true，并将**publicUrl**属性设置为计划页面的 URL。</span><span class="sxs-lookup"><span data-stu-id="98318-106">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="98318-107">权限</span><span class="sxs-lookup"><span data-stu-id="98318-107">Permissions</span></span>
<span data-ttu-id="98318-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98318-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98318-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="98318-110">Permission type</span></span>      | <span data-ttu-id="98318-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="98318-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98318-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98318-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="98318-113">预订. 全部</span><span class="sxs-lookup"><span data-stu-id="98318-113">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="98318-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98318-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98318-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="98318-115">Not supported.</span></span>   |
|<span data-ttu-id="98318-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="98318-116">Application</span></span> | <span data-ttu-id="98318-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="98318-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="98318-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98318-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="98318-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="98318-119">Request headers</span></span>
| <span data-ttu-id="98318-120">名称</span><span class="sxs-lookup"><span data-stu-id="98318-120">Name</span></span>       | <span data-ttu-id="98318-121">说明</span><span class="sxs-lookup"><span data-stu-id="98318-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="98318-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="98318-122">Authorization</span></span>  | <span data-ttu-id="98318-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="98318-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="98318-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="98318-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="98318-125">响应</span><span class="sxs-lookup"><span data-stu-id="98318-125">Response</span></span>
<span data-ttu-id="98318-p102">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="98318-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98318-128">示例</span><span class="sxs-lookup"><span data-stu-id="98318-128">Example</span></span>
<span data-ttu-id="98318-129">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="98318-129">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="98318-130">请求</span><span class="sxs-lookup"><span data-stu-id="98318-130">Request</span></span>
<span data-ttu-id="98318-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="98318-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="98318-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="98318-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```
# <a name="c"></a>[<span data-ttu-id="98318-133">C#</span><span class="sxs-lookup"><span data-stu-id="98318-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98318-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98318-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98318-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98318-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="98318-136">响应</span><span class="sxs-lookup"><span data-stu-id="98318-136">Response</span></span>
<span data-ttu-id="98318-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="98318-137">The following is an example of the response.</span></span>
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
