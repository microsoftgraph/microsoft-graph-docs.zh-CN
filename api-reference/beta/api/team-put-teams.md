---
title: 从组创建团队
description: 从组新建团队。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: c47b3e7568c09c3b7f5e3debaec2eb74e074d6e7
ms.sourcegitcommit: 9ffac53b262203917dfb20ac981e97f50d398199
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2019
ms.locfileid: "34669657"
---
# <a name="create-team-from-group"></a><span data-ttu-id="80037-103">从组创建团队</span><span class="sxs-lookup"><span data-stu-id="80037-103">Create team from group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> [!IMPORTANT]
> <span data-ttu-id="80037-104">我们正在弃用此 API 来支持[创建团队](../api/team-post.md)，并将于 2019 年末之前将其删除。</span><span class="sxs-lookup"><span data-stu-id="80037-104">This API is in the process of being depracated in favor of [Create team](../api/team-post.md), and will be removed by the end of 2019.</span></span> <span data-ttu-id="80037-105">要详细了解如何通过组来创建团队，请查看[创建团队](../api/team-post.md)中的示例 4 和示例 5。</span><span class="sxs-lookup"><span data-stu-id="80037-105">For details about how to create a team from a group, see examples 4 and 5 in [Create team](../api/team-post.md).</span></span>

<span data-ttu-id="80037-106">从[组](../resources/group.md)新建[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="80037-106">Create a new [team](../resources/team.md) from a [group](../resources/group.md).</span></span>

<span data-ttu-id="80037-107">若要创建团队，组必须至少拥有一个所有者。</span><span class="sxs-lookup"><span data-stu-id="80037-107">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="80037-108">如果在不到 15 分钟之前创建组，则可能会因为重复延迟导致“创建团队呼叫”失败并显示错误代码 404。</span><span class="sxs-lookup"><span data-stu-id="80037-108">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="80037-109">建议的模式是重试“创建团队呼叫”三次，每次呼叫之间延迟 10 秒。</span><span class="sxs-lookup"><span data-stu-id="80037-109">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="80037-110">权限</span><span class="sxs-lookup"><span data-stu-id="80037-110">Permissions</span></span>

<span data-ttu-id="80037-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80037-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80037-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="80037-113">Permission type</span></span>      | <span data-ttu-id="80037-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80037-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80037-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80037-115">Delegated (work or school account)</span></span> | <span data-ttu-id="80037-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80037-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="80037-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80037-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80037-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="80037-118">Not supported.</span></span>    |
|<span data-ttu-id="80037-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="80037-119">Application</span></span> | <span data-ttu-id="80037-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80037-120">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="80037-121">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="80037-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="80037-122">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的组。</span><span class="sxs-lookup"><span data-stu-id="80037-122">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="80037-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80037-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="80037-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="80037-124">Request headers</span></span>

| <span data-ttu-id="80037-125">标头</span><span class="sxs-lookup"><span data-stu-id="80037-125">Header</span></span>       | <span data-ttu-id="80037-126">值</span><span class="sxs-lookup"><span data-stu-id="80037-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="80037-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="80037-127">Authorization</span></span>  | <span data-ttu-id="80037-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80037-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="80037-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="80037-130">Content-Type</span></span>  | <span data-ttu-id="80037-131">application/json</span><span class="sxs-lookup"><span data-stu-id="80037-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="80037-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="80037-132">Request body</span></span>

<span data-ttu-id="80037-133">在请求正文中，提供 [team](../resources/team.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80037-133">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="80037-134">响应</span><span class="sxs-lookup"><span data-stu-id="80037-134">Response</span></span>

<span data-ttu-id="80037-135">如果成功，此方法应该会在响应正文中返回 `201 Created` 响应代码和 [team](../resources/team.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80037-135">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80037-136">示例</span><span class="sxs-lookup"><span data-stu-id="80037-136">Example</span></span>

#### <a name="request"></a><span data-ttu-id="80037-137">请求</span><span class="sxs-lookup"><span data-stu-id="80037-137">Request</span></span>

<span data-ttu-id="80037-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="80037-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
PUT https://graph.microsoft.com/beta/groups/{id}/team
Content-type: application/json

{  
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  }
}
```

#### <a name="response"></a><span data-ttu-id="80037-139">响应</span><span class="sxs-lookup"><span data-stu-id="80037-139">Response</span></span>

<span data-ttu-id="80037-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="80037-140">The following is an example of the response.</span></span> 

><span data-ttu-id="80037-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="80037-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true    
  },
  "guestSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true 
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true    
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a><span data-ttu-id="80037-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="80037-143">See also</span></span>

- [<span data-ttu-id="80037-144">创建包含团队的组</span><span class="sxs-lookup"><span data-stu-id="80037-144">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
