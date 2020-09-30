---
title: 删除 schedulingGroup
description: 通过设置 schedulingGroup 的 isActive 属性将其标记为非活动
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f19f6f4f228b400b66345df16fcd1320f3aa31d7
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314613"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="dba97-103">删除 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="dba97-103">Delete schedulingGroup</span></span>

<span data-ttu-id="dba97-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dba97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dba97-105">通过设置 [schedulingGroup](../resources/schedulinggroup.md) 的 **isActive** 属性将其标记为非活动状态。</span><span class="sxs-lookup"><span data-stu-id="dba97-105">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="dba97-106">此方法不会从计划中删除 [schedulingGroup](../resources/schedulinggroup.md) 。</span><span class="sxs-lookup"><span data-stu-id="dba97-106">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="dba97-107">分配给计划组的现有 [班次](../resources/shift.md) 实例仍为组的一部分。</span><span class="sxs-lookup"><span data-stu-id="dba97-107">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="dba97-108">权限</span><span class="sxs-lookup"><span data-stu-id="dba97-108">Permissions</span></span>

<span data-ttu-id="dba97-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dba97-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dba97-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dba97-111">Permission type</span></span>      | <span data-ttu-id="dba97-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dba97-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dba97-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dba97-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dba97-114">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="dba97-114">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dba97-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dba97-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dba97-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dba97-116">Not supported.</span></span>    |
|<span data-ttu-id="dba97-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dba97-117">Application</span></span> | <span data-ttu-id="dba97-118">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dba97-118">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dba97-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dba97-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="dba97-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dba97-120">Request headers</span></span>

| <span data-ttu-id="dba97-121">标头</span><span class="sxs-lookup"><span data-stu-id="dba97-121">Header</span></span>       | <span data-ttu-id="dba97-122">值</span><span class="sxs-lookup"><span data-stu-id="dba97-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dba97-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dba97-123">Authorization</span></span>  | <span data-ttu-id="dba97-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dba97-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dba97-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dba97-126">Request body</span></span>
<span data-ttu-id="dba97-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dba97-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dba97-128">响应</span><span class="sxs-lookup"><span data-stu-id="dba97-128">Response</span></span>

<span data-ttu-id="dba97-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="dba97-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dba97-131">示例</span><span class="sxs-lookup"><span data-stu-id="dba97-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dba97-132">请求</span><span class="sxs-lookup"><span data-stu-id="dba97-132">Request</span></span>

<span data-ttu-id="dba97-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dba97-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dba97-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="dba97-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="c"></a>[<span data-ttu-id="dba97-135">C#</span><span class="sxs-lookup"><span data-stu-id="dba97-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-delete-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dba97-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dba97-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-delete-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dba97-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dba97-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-delete-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dba97-138">响应</span><span class="sxs-lookup"><span data-stu-id="dba97-138">Response</span></span>

<span data-ttu-id="dba97-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dba97-139">The following is an example of the response.</span></span> 

><span data-ttu-id="dba97-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dba97-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


