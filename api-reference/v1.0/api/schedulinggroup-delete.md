---
title: 删除 schedulingGroup
description: 通过设置 schedulingGroup 的 isActive 属性将其标记为非活动
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7c7aae33e48ca3170cdc2ce06e96d704139ec13f
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155136"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="a79d3-103">删除 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="a79d3-103">Delete schedulingGroup</span></span>

<span data-ttu-id="a79d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a79d3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a79d3-105">通过设置[schedulingGroup](../resources/schedulinggroup.md)的**isActive**属性将其标记为非活动状态。</span><span class="sxs-lookup"><span data-stu-id="a79d3-105">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="a79d3-106">此方法不会从计划中删除[schedulingGroup](../resources/schedulinggroup.md) 。</span><span class="sxs-lookup"><span data-stu-id="a79d3-106">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="a79d3-107">分配给计划组的现有[班次](../resources/shift.md)实例仍为组的一部分。</span><span class="sxs-lookup"><span data-stu-id="a79d3-107">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="a79d3-108">权限</span><span class="sxs-lookup"><span data-stu-id="a79d3-108">Permissions</span></span>

<span data-ttu-id="a79d3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a79d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a79d3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a79d3-111">Permission type</span></span>      | <span data-ttu-id="a79d3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a79d3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a79d3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a79d3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a79d3-114">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="a79d3-114">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a79d3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a79d3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a79d3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a79d3-116">Not supported.</span></span>    |
|<span data-ttu-id="a79d3-117">Application</span><span class="sxs-lookup"><span data-stu-id="a79d3-117">Application</span></span> | <span data-ttu-id="a79d3-118">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a79d3-118">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="a79d3-119">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="a79d3-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a79d3-120">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="a79d3-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a79d3-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a79d3-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="a79d3-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a79d3-122">Request headers</span></span>

| <span data-ttu-id="a79d3-123">标头</span><span class="sxs-lookup"><span data-stu-id="a79d3-123">Header</span></span>       | <span data-ttu-id="a79d3-124">值</span><span class="sxs-lookup"><span data-stu-id="a79d3-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a79d3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a79d3-125">Authorization</span></span>  | <span data-ttu-id="a79d3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a79d3-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a79d3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a79d3-128">Request body</span></span>
<span data-ttu-id="a79d3-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a79d3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a79d3-130">响应</span><span class="sxs-lookup"><span data-stu-id="a79d3-130">Response</span></span>

<span data-ttu-id="a79d3-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a79d3-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a79d3-133">示例</span><span class="sxs-lookup"><span data-stu-id="a79d3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a79d3-134">请求</span><span class="sxs-lookup"><span data-stu-id="a79d3-134">Request</span></span>

<span data-ttu-id="a79d3-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a79d3-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
---


### <a name="response"></a><span data-ttu-id="a79d3-136">响应</span><span class="sxs-lookup"><span data-stu-id="a79d3-136">Response</span></span>

<span data-ttu-id="a79d3-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a79d3-137">The following is an example of the response.</span></span> 

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
