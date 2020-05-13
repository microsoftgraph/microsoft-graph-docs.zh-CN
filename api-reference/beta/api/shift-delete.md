---
title: 删除班次
description: 删除日程中的班次轮换。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c0ee4a22d2fc4d206e9ded8419c7fb3317255ece
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "42453320"
---
# <a name="delete-shift"></a><span data-ttu-id="b609b-103">删除班次</span><span class="sxs-lookup"><span data-stu-id="b609b-103">Delete shift</span></span>

<span data-ttu-id="b609b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b609b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b609b-105">删除日程中的[班次轮换](../resources/shift.md)。</span><span class="sxs-lookup"><span data-stu-id="b609b-105">Deletes a [shift](../resources/shift.md) from the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="b609b-106">权限</span><span class="sxs-lookup"><span data-stu-id="b609b-106">Permissions</span></span>

<span data-ttu-id="b609b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b609b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b609b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b609b-109">Permission type</span></span>      | <span data-ttu-id="b609b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b609b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b609b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b609b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b609b-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b609b-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b609b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b609b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b609b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b609b-114">Not supported.</span></span>    |
|<span data-ttu-id="b609b-115">Application</span><span class="sxs-lookup"><span data-stu-id="b609b-115">Application</span></span> | <span data-ttu-id="b609b-116">Schedule. All *、schedule、all*</span><span class="sxs-lookup"><span data-stu-id="b609b-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="b609b-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="b609b-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="b609b-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="b609b-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b609b-119">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="b609b-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b609b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b609b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="b609b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b609b-121">Request headers</span></span>

| <span data-ttu-id="b609b-122">标头</span><span class="sxs-lookup"><span data-stu-id="b609b-122">Header</span></span>       | <span data-ttu-id="b609b-123">值</span><span class="sxs-lookup"><span data-stu-id="b609b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b609b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b609b-124">Authorization</span></span>  | <span data-ttu-id="b609b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b609b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b609b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b609b-127">Request body</span></span>
<span data-ttu-id="b609b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b609b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b609b-129">响应</span><span class="sxs-lookup"><span data-stu-id="b609b-129">Response</span></span>

<span data-ttu-id="b609b-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b609b-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b609b-132">示例</span><span class="sxs-lookup"><span data-stu-id="b609b-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b609b-133">请求</span><span class="sxs-lookup"><span data-stu-id="b609b-133">Request</span></span>

<span data-ttu-id="b609b-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b609b-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b609b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b609b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="b609b-136">C#</span><span class="sxs-lookup"><span data-stu-id="b609b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b609b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b609b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b609b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b609b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b609b-139">响应</span><span class="sxs-lookup"><span data-stu-id="b609b-139">Response</span></span>

<span data-ttu-id="b609b-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b609b-140">The following is an example of the response.</span></span> 

><span data-ttu-id="b609b-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b609b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
