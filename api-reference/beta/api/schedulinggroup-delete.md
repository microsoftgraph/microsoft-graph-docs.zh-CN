---
title: 删除 schedulingGroup
description: 通过设置 schedulingGroup 的 isActive 属性将其标记为非活动
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6a41108349d7e398d10afd183273f731cf947fe8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331370"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="b71ba-103">删除 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="b71ba-103">Delete schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b71ba-104">通过设置[schedulingGroup](../resources/schedulinggroup.md)的**isActive**属性将其标记为非活动状态。</span><span class="sxs-lookup"><span data-stu-id="b71ba-104">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="b71ba-105">此方法不会从计划中删除[schedulingGroup](../resources/schedulinggroup.md) 。</span><span class="sxs-lookup"><span data-stu-id="b71ba-105">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="b71ba-106">分配给计划组的现有[班次](../resources/shift.md)实例仍为组的一部分。</span><span class="sxs-lookup"><span data-stu-id="b71ba-106">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="b71ba-107">权限</span><span class="sxs-lookup"><span data-stu-id="b71ba-107">Permissions</span></span>

<span data-ttu-id="b71ba-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b71ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b71ba-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b71ba-110">Permission type</span></span>      | <span data-ttu-id="b71ba-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b71ba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b71ba-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b71ba-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b71ba-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b71ba-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b71ba-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b71ba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b71ba-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b71ba-115">Not supported.</span></span>    |
|<span data-ttu-id="b71ba-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b71ba-116">Application</span></span> | <span data-ttu-id="b71ba-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b71ba-117">Not supported.</span></span> |

> <span data-ttu-id="b71ba-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="b71ba-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b71ba-119">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="b71ba-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b71ba-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b71ba-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="b71ba-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b71ba-121">Request headers</span></span>

| <span data-ttu-id="b71ba-122">标头</span><span class="sxs-lookup"><span data-stu-id="b71ba-122">Header</span></span>       | <span data-ttu-id="b71ba-123">值</span><span class="sxs-lookup"><span data-stu-id="b71ba-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b71ba-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b71ba-124">Authorization</span></span>  | <span data-ttu-id="b71ba-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b71ba-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b71ba-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b71ba-127">Content-Type</span></span>  | <span data-ttu-id="b71ba-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b71ba-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b71ba-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b71ba-129">Request body</span></span>
<span data-ttu-id="b71ba-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b71ba-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b71ba-131">响应</span><span class="sxs-lookup"><span data-stu-id="b71ba-131">Response</span></span>

<span data-ttu-id="b71ba-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b71ba-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b71ba-134">示例</span><span class="sxs-lookup"><span data-stu-id="b71ba-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b71ba-135">请求</span><span class="sxs-lookup"><span data-stu-id="b71ba-135">Request</span></span>

<span data-ttu-id="b71ba-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b71ba-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

#### <a name="response"></a><span data-ttu-id="b71ba-137">响应</span><span class="sxs-lookup"><span data-stu-id="b71ba-137">Response</span></span>

<span data-ttu-id="b71ba-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b71ba-138">The following is an example of the response.</span></span> 

><span data-ttu-id="b71ba-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b71ba-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
