---
title: 删除 schedulingGroup
description: 通过设置 schedulingGroup 的 isActive 属性将其标记为非活动
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7a23472db0b87204ed3dd3e7408154738a940103
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867903"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="6fbde-103">删除 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="6fbde-103">Delete schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fbde-104">通过设置[schedulingGroup](../resources/schedulinggroup.md)的**isActive**属性将其标记为非活动状态。</span><span class="sxs-lookup"><span data-stu-id="6fbde-104">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="6fbde-105">此方法不会从计划中删除[schedulingGroup](../resources/schedulinggroup.md) 。</span><span class="sxs-lookup"><span data-stu-id="6fbde-105">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="6fbde-106">分配给计划组的现有[班次](../resources/shift.md)实例仍为组的一部分。</span><span class="sxs-lookup"><span data-stu-id="6fbde-106">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="6fbde-107">权限</span><span class="sxs-lookup"><span data-stu-id="6fbde-107">Permissions</span></span>

<span data-ttu-id="6fbde-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6fbde-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fbde-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fbde-110">Permission type</span></span>      | <span data-ttu-id="6fbde-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6fbde-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fbde-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fbde-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6fbde-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fbde-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6fbde-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fbde-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fbde-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fbde-115">Not supported.</span></span>    |
|<span data-ttu-id="6fbde-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6fbde-116">Application</span></span> | <span data-ttu-id="6fbde-117">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="6fbde-117">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="6fbde-118">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="6fbde-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="6fbde-119">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="6fbde-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6fbde-120">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="6fbde-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6fbde-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fbde-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="6fbde-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="6fbde-122">Request headers</span></span>

| <span data-ttu-id="6fbde-123">标头</span><span class="sxs-lookup"><span data-stu-id="6fbde-123">Header</span></span>       | <span data-ttu-id="6fbde-124">值</span><span class="sxs-lookup"><span data-stu-id="6fbde-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6fbde-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fbde-125">Authorization</span></span>  | <span data-ttu-id="6fbde-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6fbde-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6fbde-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fbde-128">Request body</span></span>
<span data-ttu-id="6fbde-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6fbde-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fbde-130">响应</span><span class="sxs-lookup"><span data-stu-id="6fbde-130">Response</span></span>

<span data-ttu-id="6fbde-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6fbde-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fbde-133">示例</span><span class="sxs-lookup"><span data-stu-id="6fbde-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6fbde-134">请求</span><span class="sxs-lookup"><span data-stu-id="6fbde-134">Request</span></span>

<span data-ttu-id="6fbde-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6fbde-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6fbde-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fbde-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6fbde-137">C#</span><span class="sxs-lookup"><span data-stu-id="6fbde-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-delete-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6fbde-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fbde-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-delete-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6fbde-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fbde-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-delete-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6fbde-140">响应</span><span class="sxs-lookup"><span data-stu-id="6fbde-140">Response</span></span>

<span data-ttu-id="6fbde-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6fbde-141">The following is an example of the response.</span></span> 

><span data-ttu-id="6fbde-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6fbde-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Marks a schedulingGroup as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
