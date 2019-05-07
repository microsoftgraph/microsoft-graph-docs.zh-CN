---
title: 删除 bookingStaffMember
description: 删除指定 bookingbusiness 中的教职员工成员。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 18c9f187b81f997781b22c4b537fb564edde37e6
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635937"
---
# <a name="delete-bookingstaffmember"></a><span data-ttu-id="20f42-103">删除 bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="20f42-103">Delete bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20f42-104">删除指定[bookingbusiness](../resources/bookingbusiness.md)中的[教职员工成员](../resources/bookingstaffmember.md)。</span><span class="sxs-lookup"><span data-stu-id="20f42-104">Delete a [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="20f42-105">权限</span><span class="sxs-lookup"><span data-stu-id="20f42-105">Permissions</span></span>
<span data-ttu-id="20f42-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20f42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20f42-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="20f42-108">Permission type</span></span>      | <span data-ttu-id="20f42-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20f42-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20f42-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20f42-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="20f42-111">全部预订。全部, 全部预订。全部</span><span class="sxs-lookup"><span data-stu-id="20f42-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="20f42-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20f42-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20f42-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="20f42-113">Not supported.</span></span>   |
|<span data-ttu-id="20f42-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="20f42-114">Application</span></span> | <span data-ttu-id="20f42-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="20f42-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="20f42-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20f42-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/staffMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="20f42-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="20f42-117">Request headers</span></span>
| <span data-ttu-id="20f42-118">名称</span><span class="sxs-lookup"><span data-stu-id="20f42-118">Name</span></span>       | <span data-ttu-id="20f42-119">说明</span><span class="sxs-lookup"><span data-stu-id="20f42-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="20f42-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="20f42-120">Authorization</span></span>  | <span data-ttu-id="20f42-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="20f42-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="20f42-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="20f42-122">Request body</span></span>
<span data-ttu-id="20f42-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="20f42-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="20f42-124">响应</span><span class="sxs-lookup"><span data-stu-id="20f42-124">Response</span></span>
<span data-ttu-id="20f42-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="20f42-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20f42-127">示例</span><span class="sxs-lookup"><span data-stu-id="20f42-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20f42-128">请求</span><span class="sxs-lookup"><span data-stu-id="20f42-128">Request</span></span>
<span data-ttu-id="20f42-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="20f42-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingstaffmember"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/5fae928f-6d2d-417a-ad96-4b0caeb362d6
```
##### <a name="response"></a><span data-ttu-id="20f42-130">响应</span><span class="sxs-lookup"><span data-stu-id="20f42-130">Response</span></span>
<span data-ttu-id="20f42-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="20f42-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="20f42-132">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="20f42-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="20f42-133">语言</span><span class="sxs-lookup"><span data-stu-id="20f42-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_bookingstaffmember-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20f42-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="20f42-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_bookingstaffmember-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingstaffmember-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingstaffmember-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
