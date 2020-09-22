---
title: 删除 schedulingGroup
description: 通过设置 schedulingGroup 的 isActive 属性将其标记为非活动
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9c5eabe4503bf8ac3f6d98d16a0a85a6f01d5af4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071925"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="28e44-103">删除 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="28e44-103">Delete schedulingGroup</span></span>

<span data-ttu-id="28e44-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28e44-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28e44-105">通过设置 [schedulingGroup](../resources/schedulinggroup.md) 的 **isActive** 属性将其标记为非活动状态。</span><span class="sxs-lookup"><span data-stu-id="28e44-105">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="28e44-106">此方法不会从计划中删除 [schedulingGroup](../resources/schedulinggroup.md) 。</span><span class="sxs-lookup"><span data-stu-id="28e44-106">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="28e44-107">分配给计划组的现有 [班次](../resources/shift.md) 实例仍为组的一部分。</span><span class="sxs-lookup"><span data-stu-id="28e44-107">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="28e44-108">权限</span><span class="sxs-lookup"><span data-stu-id="28e44-108">Permissions</span></span>

<span data-ttu-id="28e44-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="28e44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28e44-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="28e44-111">Permission type</span></span>      | <span data-ttu-id="28e44-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="28e44-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28e44-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28e44-113">Delegated (work or school account)</span></span> | <span data-ttu-id="28e44-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28e44-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="28e44-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28e44-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28e44-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="28e44-116">Not supported.</span></span>    |
|<span data-ttu-id="28e44-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="28e44-117">Application</span></span> | <span data-ttu-id="28e44-118">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="28e44-118">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="28e44-119">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="28e44-119">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="28e44-120">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="28e44-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="28e44-121">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="28e44-121">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="28e44-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28e44-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="28e44-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="28e44-123">Request headers</span></span>

| <span data-ttu-id="28e44-124">标头</span><span class="sxs-lookup"><span data-stu-id="28e44-124">Header</span></span>       | <span data-ttu-id="28e44-125">值</span><span class="sxs-lookup"><span data-stu-id="28e44-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="28e44-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="28e44-126">Authorization</span></span>  | <span data-ttu-id="28e44-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="28e44-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="28e44-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="28e44-129">Request body</span></span>
<span data-ttu-id="28e44-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="28e44-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28e44-131">响应</span><span class="sxs-lookup"><span data-stu-id="28e44-131">Response</span></span>

<span data-ttu-id="28e44-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="28e44-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28e44-134">示例</span><span class="sxs-lookup"><span data-stu-id="28e44-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="28e44-135">请求</span><span class="sxs-lookup"><span data-stu-id="28e44-135">Request</span></span>

<span data-ttu-id="28e44-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="28e44-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28e44-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="28e44-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="c"></a>[<span data-ttu-id="28e44-138">C#</span><span class="sxs-lookup"><span data-stu-id="28e44-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-delete-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28e44-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28e44-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-delete-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28e44-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28e44-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-delete-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="28e44-141">响应</span><span class="sxs-lookup"><span data-stu-id="28e44-141">Response</span></span>

<span data-ttu-id="28e44-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="28e44-142">The following is an example of the response.</span></span> 

><span data-ttu-id="28e44-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="28e44-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


