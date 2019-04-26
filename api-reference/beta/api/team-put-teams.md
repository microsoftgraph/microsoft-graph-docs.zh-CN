---
title: 从组创建团队
description: 从组新建团队。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 9950b92acb28d8138bba363170c8e1e89b5f1d5a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335254"
---
# <a name="create-team-from-group"></a><span data-ttu-id="99544-103">从组创建团队</span><span class="sxs-lookup"><span data-stu-id="99544-103">Create team from group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99544-104">从[组](../resources/group.md)新建[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="99544-104">Create a new [team](../resources/team.md) from a [group](../resources/group.md).</span></span>

<span data-ttu-id="99544-105">若要创建团队，组必须至少拥有一个所有者。</span><span class="sxs-lookup"><span data-stu-id="99544-105">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="99544-106">如果在不到 15 分钟之前创建组，则可能会因为重复延迟导致“创建团队呼叫”失败并显示错误代码 404。</span><span class="sxs-lookup"><span data-stu-id="99544-106">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="99544-107">建议的模式是重试“创建团队呼叫”三次，每次呼叫之间延迟 10 秒。</span><span class="sxs-lookup"><span data-stu-id="99544-107">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="99544-108">权限</span><span class="sxs-lookup"><span data-stu-id="99544-108">Permissions</span></span>

<span data-ttu-id="99544-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99544-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99544-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="99544-111">Permission type</span></span>      | <span data-ttu-id="99544-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99544-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99544-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99544-113">Delegated (work or school account)</span></span> | <span data-ttu-id="99544-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99544-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="99544-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99544-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99544-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="99544-116">Not supported.</span></span>    |
|<span data-ttu-id="99544-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="99544-117">Application</span></span> | <span data-ttu-id="99544-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99544-118">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="99544-119">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="99544-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="99544-120">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的组。</span><span class="sxs-lookup"><span data-stu-id="99544-120">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="99544-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99544-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="99544-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="99544-122">Request headers</span></span>

| <span data-ttu-id="99544-123">标头</span><span class="sxs-lookup"><span data-stu-id="99544-123">Header</span></span>       | <span data-ttu-id="99544-124">值</span><span class="sxs-lookup"><span data-stu-id="99544-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="99544-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="99544-125">Authorization</span></span>  | <span data-ttu-id="99544-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="99544-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="99544-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="99544-128">Content-Type</span></span>  | <span data-ttu-id="99544-129">application/json</span><span class="sxs-lookup"><span data-stu-id="99544-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="99544-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="99544-130">Request body</span></span>

<span data-ttu-id="99544-131">在请求正文中，提供 [team](../resources/team.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99544-131">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="99544-132">响应</span><span class="sxs-lookup"><span data-stu-id="99544-132">Response</span></span>

<span data-ttu-id="99544-133">如果成功，此方法应该会在响应正文中返回 `201 Created` 响应代码和 [team](../resources/team.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="99544-133">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99544-134">示例</span><span class="sxs-lookup"><span data-stu-id="99544-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="99544-135">请求</span><span class="sxs-lookup"><span data-stu-id="99544-135">Request</span></span>

<span data-ttu-id="99544-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="99544-136">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="99544-137">响应</span><span class="sxs-lookup"><span data-stu-id="99544-137">Response</span></span>

<span data-ttu-id="99544-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="99544-138">The following is an example of the response.</span></span> 

><span data-ttu-id="99544-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="99544-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="99544-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="99544-141">See also</span></span>

- [<span data-ttu-id="99544-142">创建包含团队的组</span><span class="sxs-lookup"><span data-stu-id="99544-142">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
