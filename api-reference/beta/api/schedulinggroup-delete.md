---
title: 删除 schedulingGroup
description: 通过设置 schedulingGroup 的 isActive 属性将其标记为非活动
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 751d40329b06fe694c7bf0c53e9dc9499b5fee57
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788008"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="601fd-103">删除 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="601fd-103">Delete schedulingGroup</span></span>

<span data-ttu-id="601fd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="601fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="601fd-105">通过设置 [schedulingGroup](../resources/schedulinggroup.md) 的 isActive 属性，将其 **标记为非** 活动状态。</span><span class="sxs-lookup"><span data-stu-id="601fd-105">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="601fd-106">此方法不会从计划中删除[schedulingGroup。](../resources/schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="601fd-106">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="601fd-107">分配给 [计划](../resources/shift.md) 组的现有班次实例仍属于该组。</span><span class="sxs-lookup"><span data-stu-id="601fd-107">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="601fd-108">权限</span><span class="sxs-lookup"><span data-stu-id="601fd-108">Permissions</span></span>

<span data-ttu-id="601fd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="601fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="601fd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="601fd-111">Permission type</span></span>      | <span data-ttu-id="601fd-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="601fd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="601fd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="601fd-113">Delegated (work or school account)</span></span> | <span data-ttu-id="601fd-114">Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="601fd-114">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="601fd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="601fd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="601fd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="601fd-116">Not supported.</span></span>    |
|<span data-ttu-id="601fd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="601fd-117">Application</span></span> | <span data-ttu-id="601fd-118">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="601fd-118">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="601fd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="601fd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="601fd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="601fd-120">Request headers</span></span>

| <span data-ttu-id="601fd-121">标头</span><span class="sxs-lookup"><span data-stu-id="601fd-121">Header</span></span>       | <span data-ttu-id="601fd-122">值</span><span class="sxs-lookup"><span data-stu-id="601fd-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="601fd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="601fd-123">Authorization</span></span>  | <span data-ttu-id="601fd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="601fd-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="601fd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="601fd-126">Request body</span></span>
<span data-ttu-id="601fd-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="601fd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="601fd-128">响应</span><span class="sxs-lookup"><span data-stu-id="601fd-128">Response</span></span>

<span data-ttu-id="601fd-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="601fd-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="601fd-131">示例</span><span class="sxs-lookup"><span data-stu-id="601fd-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="601fd-132">请求</span><span class="sxs-lookup"><span data-stu-id="601fd-132">Request</span></span>

<span data-ttu-id="601fd-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="601fd-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="601fd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="601fd-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="c"></a>[<span data-ttu-id="601fd-135">C#</span><span class="sxs-lookup"><span data-stu-id="601fd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-delete-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="601fd-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="601fd-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-delete-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="601fd-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="601fd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-delete-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="601fd-138">Java</span><span class="sxs-lookup"><span data-stu-id="601fd-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-delete-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="601fd-139">响应</span><span class="sxs-lookup"><span data-stu-id="601fd-139">Response</span></span>

<span data-ttu-id="601fd-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="601fd-140">The following is an example of the response.</span></span> 

><span data-ttu-id="601fd-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="601fd-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
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


