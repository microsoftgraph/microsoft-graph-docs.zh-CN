---
title: 删除 bookingService
description: 删除指定 bookingbusiness 中的 bookingService 对象。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: e31f7afd39fd3bdf7029324df1fc09058bc85b26
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35257909"
---
# <a name="delete-bookingservice"></a><span data-ttu-id="fa054-103">删除 bookingService</span><span class="sxs-lookup"><span data-stu-id="fa054-103">Delete bookingService</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa054-104">删除指定[bookingbusiness](../resources/bookingbusiness.md)中的[bookingService](../resources/bookingservice.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fa054-104">Delete a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="fa054-105">权限</span><span class="sxs-lookup"><span data-stu-id="fa054-105">Permissions</span></span>
<span data-ttu-id="fa054-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa054-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa054-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa054-108">Permission type</span></span>      | <span data-ttu-id="fa054-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa054-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa054-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa054-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="fa054-111">全部预订. 全部, 全部预订. 全部</span><span class="sxs-lookup"><span data-stu-id="fa054-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="fa054-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa054-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa054-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa054-113">Not supported.</span></span>   |
|<span data-ttu-id="fa054-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa054-114">Application</span></span> | <span data-ttu-id="fa054-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa054-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="fa054-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa054-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/services/{id}

```
## <a name="request-headers"></a><span data-ttu-id="fa054-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa054-117">Request headers</span></span>
| <span data-ttu-id="fa054-118">名称</span><span class="sxs-lookup"><span data-stu-id="fa054-118">Name</span></span>       | <span data-ttu-id="fa054-119">说明</span><span class="sxs-lookup"><span data-stu-id="fa054-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fa054-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa054-120">Authorization</span></span>  | <span data-ttu-id="fa054-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fa054-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa054-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa054-122">Request body</span></span>
<span data-ttu-id="fa054-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fa054-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="fa054-124">响应</span><span class="sxs-lookup"><span data-stu-id="fa054-124">Response</span></span>
<span data-ttu-id="fa054-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fa054-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa054-127">示例</span><span class="sxs-lookup"><span data-stu-id="fa054-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa054-128">请求</span><span class="sxs-lookup"><span data-stu-id="fa054-128">Request</span></span>
<span data-ttu-id="fa054-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fa054-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingservice"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
##### <a name="response"></a><span data-ttu-id="fa054-130">响应</span><span class="sxs-lookup"><span data-stu-id="fa054-130">Response</span></span>
<span data-ttu-id="fa054-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fa054-131">The following is an example of the response.</span></span> <span data-ttu-id="fa054-132">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fa054-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fa054-133">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fa054-133">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fa054-134">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="fa054-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fa054-135">C#</span><span class="sxs-lookup"><span data-stu-id="fa054-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_bookingservice-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa054-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="fa054-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_bookingservice-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fa054-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="fa054-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_bookingservice-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingservice-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingservice-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingservice-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
