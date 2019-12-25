---
title: 删除班次
description: 删除日程中的班次轮换。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5a00b5aa562efca2210e2e32b8ecab7565aae570
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868777"
---
# <a name="delete-shift"></a><span data-ttu-id="6c67c-103">删除班次</span><span class="sxs-lookup"><span data-stu-id="6c67c-103">Delete shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c67c-104">删除日程中的[班次轮换](../resources/shift.md)。</span><span class="sxs-lookup"><span data-stu-id="6c67c-104">Deletes a [shift](../resources/shift.md) from the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c67c-105">权限</span><span class="sxs-lookup"><span data-stu-id="6c67c-105">Permissions</span></span>

<span data-ttu-id="6c67c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c67c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c67c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c67c-108">Permission type</span></span>      | <span data-ttu-id="6c67c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6c67c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c67c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c67c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6c67c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c67c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6c67c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c67c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c67c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c67c-113">Not supported.</span></span>    |
|<span data-ttu-id="6c67c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c67c-114">Application</span></span> | <span data-ttu-id="6c67c-115">Schedule. All *、schedule、all*</span><span class="sxs-lookup"><span data-stu-id="6c67c-115">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="6c67c-116">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="6c67c-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="6c67c-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="6c67c-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6c67c-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="6c67c-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6c67c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c67c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="6c67c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c67c-120">Request headers</span></span>

| <span data-ttu-id="6c67c-121">标头</span><span class="sxs-lookup"><span data-stu-id="6c67c-121">Header</span></span>       | <span data-ttu-id="6c67c-122">值</span><span class="sxs-lookup"><span data-stu-id="6c67c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6c67c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c67c-123">Authorization</span></span>  | <span data-ttu-id="6c67c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6c67c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6c67c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c67c-126">Request body</span></span>
<span data-ttu-id="6c67c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6c67c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c67c-128">响应</span><span class="sxs-lookup"><span data-stu-id="6c67c-128">Response</span></span>

<span data-ttu-id="6c67c-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6c67c-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c67c-131">示例</span><span class="sxs-lookup"><span data-stu-id="6c67c-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6c67c-132">请求</span><span class="sxs-lookup"><span data-stu-id="6c67c-132">Request</span></span>

<span data-ttu-id="6c67c-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6c67c-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6c67c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c67c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6c67c-135">C#</span><span class="sxs-lookup"><span data-stu-id="6c67c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c67c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c67c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6c67c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c67c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6c67c-138">响应</span><span class="sxs-lookup"><span data-stu-id="6c67c-138">Response</span></span>

<span data-ttu-id="6c67c-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6c67c-139">The following is an example of the response.</span></span> 

><span data-ttu-id="6c67c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6c67c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
