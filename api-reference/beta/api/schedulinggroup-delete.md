---
title: 删除 schedulingGroup
description: 通过设置 schedulingGroup 的 isActive 属性将其标记为非活动
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bb29270cdf246924f0c6a9293611bec82dac5cc3
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657712"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="979a1-103">删除 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="979a1-103">Delete schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="979a1-104">通过设置[schedulingGroup](../resources/schedulinggroup.md)的**isActive**属性将其标记为非活动状态。</span><span class="sxs-lookup"><span data-stu-id="979a1-104">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="979a1-105">此方法不会从计划中删除[schedulingGroup](../resources/schedulinggroup.md) 。</span><span class="sxs-lookup"><span data-stu-id="979a1-105">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="979a1-106">分配给计划组的现有[班次](../resources/shift.md)实例仍为组的一部分。</span><span class="sxs-lookup"><span data-stu-id="979a1-106">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="979a1-107">权限</span><span class="sxs-lookup"><span data-stu-id="979a1-107">Permissions</span></span>

<span data-ttu-id="979a1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="979a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="979a1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="979a1-110">Permission type</span></span>      | <span data-ttu-id="979a1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="979a1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="979a1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="979a1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="979a1-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="979a1-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="979a1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="979a1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="979a1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="979a1-115">Not supported.</span></span>    |
|<span data-ttu-id="979a1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="979a1-116">Application</span></span> | <span data-ttu-id="979a1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="979a1-117">Not supported.</span></span> |

> <span data-ttu-id="979a1-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="979a1-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="979a1-119">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="979a1-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="979a1-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="979a1-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="979a1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="979a1-121">Request headers</span></span>

| <span data-ttu-id="979a1-122">标头</span><span class="sxs-lookup"><span data-stu-id="979a1-122">Header</span></span>       | <span data-ttu-id="979a1-123">值</span><span class="sxs-lookup"><span data-stu-id="979a1-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="979a1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="979a1-124">Authorization</span></span>  | <span data-ttu-id="979a1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="979a1-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="979a1-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="979a1-127">Content-Type</span></span>  | <span data-ttu-id="979a1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="979a1-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="979a1-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="979a1-129">Request body</span></span>
<span data-ttu-id="979a1-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="979a1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="979a1-131">响应</span><span class="sxs-lookup"><span data-stu-id="979a1-131">Response</span></span>

<span data-ttu-id="979a1-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="979a1-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="979a1-134">示例</span><span class="sxs-lookup"><span data-stu-id="979a1-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="979a1-135">请求</span><span class="sxs-lookup"><span data-stu-id="979a1-135">Request</span></span>

<span data-ttu-id="979a1-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="979a1-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

#### <a name="response"></a><span data-ttu-id="979a1-137">响应</span><span class="sxs-lookup"><span data-stu-id="979a1-137">Response</span></span>

<span data-ttu-id="979a1-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="979a1-138">The following is an example of the response.</span></span> 

><span data-ttu-id="979a1-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="979a1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/schedule-delete-schedulinggroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
