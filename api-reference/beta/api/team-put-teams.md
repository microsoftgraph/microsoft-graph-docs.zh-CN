---
title: 创建工作组
description: 创建新组下的工作组。
ms.openlocfilehash: 2e0331724006d18a0c02227427e7251b1d7e096d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048350"
---
# <a name="create-team"></a><span data-ttu-id="8ff4f-103">创建工作组</span><span class="sxs-lookup"><span data-stu-id="8ff4f-103">Create team</span></span>

> <span data-ttu-id="8ff4f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8ff4f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ff4f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8ff4f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ff4f-106">创建新[团队](../resources/team.md)下一个[组](../resources/group.md)。</span><span class="sxs-lookup"><span data-stu-id="8ff4f-106">Create a new [team](../resources/team.md) under a [group](../resources/group.md).</span></span>

<span data-ttu-id="8ff4f-107">用于创建团队、 组必须具有至少一个所有者。</span><span class="sxs-lookup"><span data-stu-id="8ff4f-107">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="8ff4f-108">如果创建不超过 15 分钟，则可能创建团队呼叫，因为复制延迟 404 错误代码失败。</span><span class="sxs-lookup"><span data-stu-id="8ff4f-108">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="8ff4f-109">建议的模式是重试创建团队呼叫三次与调用之间 10 秒的延迟。</span><span class="sxs-lookup"><span data-stu-id="8ff4f-109">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ff4f-110">权限</span><span class="sxs-lookup"><span data-stu-id="8ff4f-110">Permissions</span></span>

<span data-ttu-id="8ff4f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ff4f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ff4f-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ff4f-113">Permission type</span></span>      | <span data-ttu-id="8ff4f-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8ff4f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ff4f-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ff4f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="8ff4f-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ff4f-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8ff4f-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ff4f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ff4f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ff4f-118">Not supported.</span></span>    |
|<span data-ttu-id="8ff4f-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ff4f-119">Application</span></span> | <span data-ttu-id="8ff4f-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ff4f-120">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ff4f-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ff4f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="8ff4f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ff4f-122">Request headers</span></span>

| <span data-ttu-id="8ff4f-123">标头</span><span class="sxs-lookup"><span data-stu-id="8ff4f-123">Header</span></span>       | <span data-ttu-id="8ff4f-124">值</span><span class="sxs-lookup"><span data-stu-id="8ff4f-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8ff4f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ff4f-125">Authorization</span></span>  | <span data-ttu-id="8ff4f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8ff4f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8ff4f-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ff4f-128">Content-Type</span></span>  | <span data-ttu-id="8ff4f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="8ff4f-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8ff4f-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ff4f-130">Request body</span></span>

<span data-ttu-id="8ff4f-131">在请求正文中，提供一个[团队](../resources/team.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ff4f-131">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8ff4f-132">响应</span><span class="sxs-lookup"><span data-stu-id="8ff4f-132">Response</span></span>

<span data-ttu-id="8ff4f-133">如果成功，则此方法应返回`201 Created`响应代码和响应正文中的[团队](../resources/team.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8ff4f-133">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ff4f-134">示例</span><span class="sxs-lookup"><span data-stu-id="8ff4f-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8ff4f-135">请求</span><span class="sxs-lookup"><span data-stu-id="8ff4f-135">Request</span></span>

<span data-ttu-id="8ff4f-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8ff4f-136">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="8ff4f-137">响应</span><span class="sxs-lookup"><span data-stu-id="8ff4f-137">Response</span></span>

<span data-ttu-id="8ff4f-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8ff4f-138">The following is an example of the response.</span></span> 

><span data-ttu-id="8ff4f-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8ff4f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="8ff4f-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="8ff4f-141">See also</span></span>

- [<span data-ttu-id="8ff4f-142">与团队创建组</span><span class="sxs-lookup"><span data-stu-id="8ff4f-142">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
