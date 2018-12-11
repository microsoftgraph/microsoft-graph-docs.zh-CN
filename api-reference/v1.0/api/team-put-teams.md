---
title: 创建工作组
description: 创建新组下的工作组。
ms.openlocfilehash: d7afffb331bf4a1714083ebb5f95147ec48a65d0
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222546"
---
# <a name="create-team"></a><span data-ttu-id="e2d9b-103">创建工作组</span><span class="sxs-lookup"><span data-stu-id="e2d9b-103">Create team</span></span>



<span data-ttu-id="e2d9b-104">创建新[团队](../resources/team.md)下一个[组](../resources/group.md)。</span><span class="sxs-lookup"><span data-stu-id="e2d9b-104">Create a new [team](../resources/team.md) under a [group](../resources/group.md).</span></span>

<span data-ttu-id="e2d9b-105">用于创建团队、 组必须具有至少一个所有者。</span><span class="sxs-lookup"><span data-stu-id="e2d9b-105">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="e2d9b-106">如果创建不超过 15 分钟，则可能创建团队呼叫，因为复制延迟 404 错误代码失败。</span><span class="sxs-lookup"><span data-stu-id="e2d9b-106">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="e2d9b-107">建议的模式是重试创建团队呼叫三次与调用之间 10 秒的延迟。</span><span class="sxs-lookup"><span data-stu-id="e2d9b-107">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2d9b-108">权限</span><span class="sxs-lookup"><span data-stu-id="e2d9b-108">Permissions</span></span>

<span data-ttu-id="e2d9b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2d9b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2d9b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2d9b-111">Permission type</span></span>      | <span data-ttu-id="e2d9b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2d9b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2d9b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2d9b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e2d9b-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2d9b-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e2d9b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2d9b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2d9b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2d9b-116">Not supported.</span></span>    |
|<span data-ttu-id="e2d9b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2d9b-117">Application</span></span> | <span data-ttu-id="e2d9b-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2d9b-118">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="e2d9b-119">**注意**： 此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="e2d9b-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e2d9b-120">全局管理员和 Microsoft 团队服务管理员可以访问它们不的成员的组。</span><span class="sxs-lookup"><span data-stu-id="e2d9b-120">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e2d9b-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2d9b-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="e2d9b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2d9b-122">Request headers</span></span>

| <span data-ttu-id="e2d9b-123">标头</span><span class="sxs-lookup"><span data-stu-id="e2d9b-123">Header</span></span>       | <span data-ttu-id="e2d9b-124">值</span><span class="sxs-lookup"><span data-stu-id="e2d9b-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e2d9b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2d9b-125">Authorization</span></span>  | <span data-ttu-id="e2d9b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2d9b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e2d9b-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e2d9b-128">Content-Type</span></span>  | <span data-ttu-id="e2d9b-129">application/json</span><span class="sxs-lookup"><span data-stu-id="e2d9b-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e2d9b-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2d9b-130">Request body</span></span>

<span data-ttu-id="e2d9b-131">在请求正文中，提供一个[团队](../resources/team.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2d9b-131">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e2d9b-132">响应</span><span class="sxs-lookup"><span data-stu-id="e2d9b-132">Response</span></span>

<span data-ttu-id="e2d9b-133">如果成功，则此方法应返回`201 Created`响应代码和响应正文中的[团队](../resources/team.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e2d9b-133">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2d9b-134">示例</span><span class="sxs-lookup"><span data-stu-id="e2d9b-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e2d9b-135">请求</span><span class="sxs-lookup"><span data-stu-id="e2d9b-135">Request</span></span>

<span data-ttu-id="e2d9b-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e2d9b-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
PUT https://graph.microsoft.com/v1.0/groups/{id}/team
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

#### <a name="response"></a><span data-ttu-id="e2d9b-137">响应</span><span class="sxs-lookup"><span data-stu-id="e2d9b-137">Response</span></span>

<span data-ttu-id="e2d9b-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e2d9b-138">The following is an example of the response.</span></span> 

><span data-ttu-id="e2d9b-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e2d9b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="e2d9b-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e2d9b-141">See also</span></span>

- [<span data-ttu-id="e2d9b-142">与团队创建组</span><span class="sxs-lookup"><span data-stu-id="e2d9b-142">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
