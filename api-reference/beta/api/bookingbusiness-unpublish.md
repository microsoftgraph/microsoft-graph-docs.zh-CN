---
title: 'bookingBusiness: 取消发布'
description: 使此业务的计划页面对外部客户不可用。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: df4f9fb74ab0cc82394a90b938f1b7478c99cd07
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865513"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="e246a-103">bookingBusiness: 取消发布</span><span class="sxs-lookup"><span data-stu-id="e246a-103">bookingBusiness: unpublish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e246a-104">使此业务的计划页面对外部客户不可用。</span><span class="sxs-lookup"><span data-stu-id="e246a-104">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="e246a-105">将**isPublished**属性设置为 false, 并将**publicUrl**属性设置为 null。</span><span class="sxs-lookup"><span data-stu-id="e246a-105">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="e246a-106">权限</span><span class="sxs-lookup"><span data-stu-id="e246a-106">Permissions</span></span>
<span data-ttu-id="e246a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e246a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e246a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e246a-109">Permission type</span></span>      | <span data-ttu-id="e246a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e246a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e246a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e246a-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="e246a-112">预订. 全部</span><span class="sxs-lookup"><span data-stu-id="e246a-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="e246a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e246a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e246a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e246a-114">Not supported.</span></span>   |
|<span data-ttu-id="e246a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e246a-115">Application</span></span> | <span data-ttu-id="e246a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e246a-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="e246a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e246a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="e246a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e246a-118">Request headers</span></span>
| <span data-ttu-id="e246a-119">名称</span><span class="sxs-lookup"><span data-stu-id="e246a-119">Name</span></span>       | <span data-ttu-id="e246a-120">说明</span><span class="sxs-lookup"><span data-stu-id="e246a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e246a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e246a-121">Authorization</span></span>  | <span data-ttu-id="e246a-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e246a-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e246a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e246a-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e246a-124">响应</span><span class="sxs-lookup"><span data-stu-id="e246a-124">Response</span></span>
<span data-ttu-id="e246a-p102">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e246a-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e246a-127">示例</span><span class="sxs-lookup"><span data-stu-id="e246a-127">Example</span></span>
<span data-ttu-id="e246a-128">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e246a-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e246a-129">请求</span><span class="sxs-lookup"><span data-stu-id="e246a-129">Request</span></span>
<span data-ttu-id="e246a-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e246a-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e246a-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e246a-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e246a-132">C#</span><span class="sxs-lookup"><span data-stu-id="e246a-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-unpublish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e246a-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="e246a-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-unpublish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e246a-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="e246a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-unpublish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e246a-135">Java</span><span class="sxs-lookup"><span data-stu-id="e246a-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingbusiness-unpublish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e246a-136">响应</span><span class="sxs-lookup"><span data-stu-id="e246a-136">Response</span></span>
<span data-ttu-id="e246a-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e246a-137">The following is an example of the response.</span></span>
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
  "description": "bookingBusiness: unpublish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
