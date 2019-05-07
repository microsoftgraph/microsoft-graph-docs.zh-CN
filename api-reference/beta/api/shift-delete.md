---
title: 删除班次
description: 删除日程中的班次轮换。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: eee9b102ee64bb02b4a13b476a07781c5f3493c0
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638618"
---
# <a name="delete-shift"></a><span data-ttu-id="bd030-103">删除班次</span><span class="sxs-lookup"><span data-stu-id="bd030-103">Delete shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd030-104">删除日程中的[班次轮换](../resources/shift.md)。</span><span class="sxs-lookup"><span data-stu-id="bd030-104">Deletes a [shift](../resources/shift.md) from the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd030-105">权限</span><span class="sxs-lookup"><span data-stu-id="bd030-105">Permissions</span></span>

<span data-ttu-id="bd030-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd030-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd030-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd030-108">Permission type</span></span>      | <span data-ttu-id="bd030-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd030-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd030-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd030-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bd030-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd030-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bd030-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd030-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd030-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd030-113">Not supported.</span></span>    |
|<span data-ttu-id="bd030-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd030-114">Application</span></span> | <span data-ttu-id="bd030-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd030-115">Not supported.</span></span> |

> <span data-ttu-id="bd030-116">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="bd030-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="bd030-117">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="bd030-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="bd030-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd030-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="bd030-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd030-119">Request headers</span></span>

| <span data-ttu-id="bd030-120">标头</span><span class="sxs-lookup"><span data-stu-id="bd030-120">Header</span></span>       | <span data-ttu-id="bd030-121">值</span><span class="sxs-lookup"><span data-stu-id="bd030-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bd030-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd030-122">Authorization</span></span>  | <span data-ttu-id="bd030-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bd030-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bd030-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bd030-125">Content-Type</span></span>  | <span data-ttu-id="bd030-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd030-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bd030-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd030-127">Request body</span></span>
<span data-ttu-id="bd030-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bd030-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd030-129">响应</span><span class="sxs-lookup"><span data-stu-id="bd030-129">Response</span></span>

<span data-ttu-id="bd030-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="bd030-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd030-132">示例</span><span class="sxs-lookup"><span data-stu-id="bd030-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bd030-133">请求</span><span class="sxs-lookup"><span data-stu-id="bd030-133">Request</span></span>

<span data-ttu-id="bd030-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bd030-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "shift-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```

#### <a name="response"></a><span data-ttu-id="bd030-135">响应</span><span class="sxs-lookup"><span data-stu-id="bd030-135">Response</span></span>

<span data-ttu-id="bd030-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bd030-136">The following is an example of the response.</span></span> 

><span data-ttu-id="bd030-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bd030-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bd030-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="bd030-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bd030-140">语言</span><span class="sxs-lookup"><span data-stu-id="bd030-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/shift-delete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd030-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="bd030-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/shift-delete-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Deletes a shift from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/shift-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/shift-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
