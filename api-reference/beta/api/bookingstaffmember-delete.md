---
title: 删除 bookingStaffMember
description: 删除指定 bookingbusiness 中的教职员工成员。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: eb6b696ed722c675de792a5d7a46b44048ba4840
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419340"
---
# <a name="delete-bookingstaffmember"></a><span data-ttu-id="886a6-103">删除 bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="886a6-103">Delete bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="886a6-104">删除指定[bookingbusiness](../resources/bookingbusiness.md)中的[教职员工成员](../resources/bookingstaffmember.md)。</span><span class="sxs-lookup"><span data-stu-id="886a6-104">Delete a [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="886a6-105">权限</span><span class="sxs-lookup"><span data-stu-id="886a6-105">Permissions</span></span>
<span data-ttu-id="886a6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="886a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="886a6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="886a6-108">Permission type</span></span>      | <span data-ttu-id="886a6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="886a6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="886a6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="886a6-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="886a6-111">全部预订. 全部, 全部预订. 全部</span><span class="sxs-lookup"><span data-stu-id="886a6-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="886a6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="886a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="886a6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="886a6-113">Not supported.</span></span>   |
|<span data-ttu-id="886a6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="886a6-114">Application</span></span> | <span data-ttu-id="886a6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="886a6-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="886a6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="886a6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/staffMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="886a6-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="886a6-117">Request headers</span></span>
| <span data-ttu-id="886a6-118">名称</span><span class="sxs-lookup"><span data-stu-id="886a6-118">Name</span></span>       | <span data-ttu-id="886a6-119">说明</span><span class="sxs-lookup"><span data-stu-id="886a6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="886a6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="886a6-120">Authorization</span></span>  | <span data-ttu-id="886a6-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="886a6-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="886a6-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="886a6-122">Request body</span></span>
<span data-ttu-id="886a6-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="886a6-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="886a6-124">响应</span><span class="sxs-lookup"><span data-stu-id="886a6-124">Response</span></span>
<span data-ttu-id="886a6-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="886a6-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="886a6-127">示例</span><span class="sxs-lookup"><span data-stu-id="886a6-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="886a6-128">请求</span><span class="sxs-lookup"><span data-stu-id="886a6-128">Request</span></span>
<span data-ttu-id="886a6-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="886a6-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="886a6-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="886a6-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingstaffmember"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/5fae928f-6d2d-417a-ad96-4b0caeb362d6
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="886a6-131">C#</span><span class="sxs-lookup"><span data-stu-id="886a6-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingstaffmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="886a6-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="886a6-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingstaffmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="886a6-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="886a6-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingstaffmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="886a6-134">响应</span><span class="sxs-lookup"><span data-stu-id="886a6-134">Response</span></span>
<span data-ttu-id="886a6-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="886a6-135">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
