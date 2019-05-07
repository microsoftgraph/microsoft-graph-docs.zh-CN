---
title: 删除 bookingBusiness
description: 删除 bookingBusiness 对象。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f296796d42e8d8461b91cdb0950149690b227eb6
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636343"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="ad309-103">删除 bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="ad309-103">Delete bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad309-104">删除[bookingBusiness](../resources/bookingbusiness.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ad309-104">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ad309-105">权限</span><span class="sxs-lookup"><span data-stu-id="ad309-105">Permissions</span></span>
<span data-ttu-id="ad309-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad309-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad309-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad309-108">Permission type</span></span>      | <span data-ttu-id="ad309-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad309-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad309-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad309-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ad309-111">预订。全部</span><span class="sxs-lookup"><span data-stu-id="ad309-111">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="ad309-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad309-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad309-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad309-113">Not supported.</span></span>   |
|<span data-ttu-id="ad309-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad309-114">Application</span></span> | <span data-ttu-id="ad309-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad309-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="ad309-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad309-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="ad309-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad309-117">Request headers</span></span>
| <span data-ttu-id="ad309-118">名称</span><span class="sxs-lookup"><span data-stu-id="ad309-118">Name</span></span>       | <span data-ttu-id="ad309-119">说明</span><span class="sxs-lookup"><span data-stu-id="ad309-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ad309-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad309-120">Authorization</span></span>  | <span data-ttu-id="ad309-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ad309-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad309-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad309-122">Request body</span></span>
<span data-ttu-id="ad309-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ad309-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="ad309-124">响应</span><span class="sxs-lookup"><span data-stu-id="ad309-124">Response</span></span>
<span data-ttu-id="ad309-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ad309-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad309-127">示例</span><span class="sxs-lookup"><span data-stu-id="ad309-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad309-128">请求</span><span class="sxs-lookup"><span data-stu-id="ad309-128">Request</span></span>
<span data-ttu-id="ad309-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ad309-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="ad309-130">响应</span><span class="sxs-lookup"><span data-stu-id="ad309-130">Response</span></span>
<span data-ttu-id="ad309-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ad309-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ad309-132">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ad309-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ad309-133">语言</span><span class="sxs-lookup"><span data-stu-id="ad309-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_bookingbusiness-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad309-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="ad309-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_bookingbusiness-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingbusiness-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
