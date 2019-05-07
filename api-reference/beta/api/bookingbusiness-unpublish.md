---
title: 'bookingBusiness: 取消发布'
description: 使此业务的计划页面对外部客户不可用。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: dc0d94094273579321a614c9ff2192f331550421
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636189"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="c2cf0-103">bookingBusiness: 取消发布</span><span class="sxs-lookup"><span data-stu-id="c2cf0-103">bookingBusiness: unpublish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2cf0-104">使此业务的计划页面对外部客户不可用。</span><span class="sxs-lookup"><span data-stu-id="c2cf0-104">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="c2cf0-105">将**isPublished**属性设置为 false, 并将**publicUrl**属性设置为 null。</span><span class="sxs-lookup"><span data-stu-id="c2cf0-105">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2cf0-106">权限</span><span class="sxs-lookup"><span data-stu-id="c2cf0-106">Permissions</span></span>
<span data-ttu-id="c2cf0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2cf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2cf0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2cf0-109">Permission type</span></span>      | <span data-ttu-id="c2cf0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2cf0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2cf0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2cf0-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="c2cf0-112">预订。全部</span><span class="sxs-lookup"><span data-stu-id="c2cf0-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c2cf0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2cf0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2cf0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2cf0-114">Not supported.</span></span>   |
|<span data-ttu-id="c2cf0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2cf0-115">Application</span></span> | <span data-ttu-id="c2cf0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2cf0-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c2cf0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2cf0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="c2cf0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2cf0-118">Request headers</span></span>
| <span data-ttu-id="c2cf0-119">名称</span><span class="sxs-lookup"><span data-stu-id="c2cf0-119">Name</span></span>       | <span data-ttu-id="c2cf0-120">说明</span><span class="sxs-lookup"><span data-stu-id="c2cf0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c2cf0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2cf0-121">Authorization</span></span>  | <span data-ttu-id="c2cf0-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c2cf0-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2cf0-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2cf0-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c2cf0-124">响应</span><span class="sxs-lookup"><span data-stu-id="c2cf0-124">Response</span></span>
<span data-ttu-id="c2cf0-p102">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c2cf0-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2cf0-127">示例</span><span class="sxs-lookup"><span data-stu-id="c2cf0-127">Example</span></span>
<span data-ttu-id="c2cf0-128">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c2cf0-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c2cf0-129">请求</span><span class="sxs-lookup"><span data-stu-id="c2cf0-129">Request</span></span>
<span data-ttu-id="c2cf0-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c2cf0-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```

##### <a name="response"></a><span data-ttu-id="c2cf0-131">响应</span><span class="sxs-lookup"><span data-stu-id="c2cf0-131">Response</span></span>
<span data-ttu-id="c2cf0-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c2cf0-132">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c2cf0-133">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c2cf0-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c2cf0-134">语言</span><span class="sxs-lookup"><span data-stu-id="c2cf0-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/bookingbusiness_unpublish-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2cf0-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2cf0-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/bookingbusiness_unpublish-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingbusiness-unpublish.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-unpublish.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
