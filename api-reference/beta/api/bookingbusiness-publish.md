---
title: 'bookingBusiness: 发布'
description: 使此业务的日程安排页面对外部客户可用。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f533a9759db0b2e47c57b1ab55282804f4acf235
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258000"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="bdd44-103">bookingBusiness: 发布</span><span class="sxs-lookup"><span data-stu-id="bdd44-103">bookingBusiness: publish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdd44-104">使此业务的日程安排页面对外部客户可用。</span><span class="sxs-lookup"><span data-stu-id="bdd44-104">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="bdd44-105">将**isPublished**属性设置为 true, 并将**publicUrl**属性设置为计划页面的 URL。</span><span class="sxs-lookup"><span data-stu-id="bdd44-105">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdd44-106">权限</span><span class="sxs-lookup"><span data-stu-id="bdd44-106">Permissions</span></span>
<span data-ttu-id="bdd44-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bdd44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdd44-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bdd44-109">Permission type</span></span>      | <span data-ttu-id="bdd44-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bdd44-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdd44-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bdd44-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="bdd44-112">预订. 全部</span><span class="sxs-lookup"><span data-stu-id="bdd44-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="bdd44-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bdd44-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdd44-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bdd44-114">Not supported.</span></span>   |
|<span data-ttu-id="bdd44-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bdd44-115">Application</span></span> | <span data-ttu-id="bdd44-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bdd44-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="bdd44-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bdd44-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="bdd44-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bdd44-118">Request headers</span></span>
| <span data-ttu-id="bdd44-119">名称</span><span class="sxs-lookup"><span data-stu-id="bdd44-119">Name</span></span>       | <span data-ttu-id="bdd44-120">说明</span><span class="sxs-lookup"><span data-stu-id="bdd44-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bdd44-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdd44-121">Authorization</span></span>  | <span data-ttu-id="bdd44-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bdd44-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdd44-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="bdd44-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="bdd44-124">响应</span><span class="sxs-lookup"><span data-stu-id="bdd44-124">Response</span></span>
<span data-ttu-id="bdd44-p102">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="bdd44-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdd44-127">示例</span><span class="sxs-lookup"><span data-stu-id="bdd44-127">Example</span></span>
<span data-ttu-id="bdd44-128">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="bdd44-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bdd44-129">请求</span><span class="sxs-lookup"><span data-stu-id="bdd44-129">Request</span></span>
<span data-ttu-id="bdd44-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bdd44-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```

##### <a name="response"></a><span data-ttu-id="bdd44-131">响应</span><span class="sxs-lookup"><span data-stu-id="bdd44-131">Response</span></span>
<span data-ttu-id="bdd44-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bdd44-132">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bdd44-133">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="bdd44-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bdd44-134">C#</span><span class="sxs-lookup"><span data-stu-id="bdd44-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/bookingbusiness_publish-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bdd44-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="bdd44-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/bookingbusiness_publish-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bdd44-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="bdd44-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/bookingbusiness_publish-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingbusiness-publish.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-publish.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-publish.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
