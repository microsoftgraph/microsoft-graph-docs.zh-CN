---
title: 创建团队
description: 在某个组下创建新的团队。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5a2f197492ae831dc3e435e3f7a63a4f02714b1a
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290340"
---
# <a name="create-team"></a><span data-ttu-id="a3802-103">创建团队</span><span class="sxs-lookup"><span data-stu-id="a3802-103">Create team</span></span>

<span data-ttu-id="a3802-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3802-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="a3802-105">在某个[组](../resources/group.md)下创建新的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="a3802-105">Create a new [team](../resources/team.md) under a [group](../resources/group.md).</span></span>

<span data-ttu-id="a3802-106">若要创建团队，组必须至少拥有一个所有者。</span><span class="sxs-lookup"><span data-stu-id="a3802-106">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="a3802-107">如果在不到 15 分钟之前创建组，则可能会因为重复延迟导致“创建团队呼叫”失败并显示错误代码 404。</span><span class="sxs-lookup"><span data-stu-id="a3802-107">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="a3802-108">建议的模式是重试“创建团队呼叫”三次，每次呼叫之间延迟 10 秒。</span><span class="sxs-lookup"><span data-stu-id="a3802-108">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3802-109">权限</span><span class="sxs-lookup"><span data-stu-id="a3802-109">Permissions</span></span>

<span data-ttu-id="a3802-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3802-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3802-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3802-112">Permission type</span></span>      | <span data-ttu-id="a3802-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3802-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3802-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3802-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a3802-115">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3802-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="a3802-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3802-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3802-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3802-117">Not supported.</span></span>    |
|<span data-ttu-id="a3802-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3802-118">Application</span></span> | <span data-ttu-id="a3802-119">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3802-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="a3802-120">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="a3802-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a3802-121">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的组。</span><span class="sxs-lookup"><span data-stu-id="a3802-121">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a3802-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3802-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="a3802-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3802-123">Request headers</span></span>

| <span data-ttu-id="a3802-124">标头</span><span class="sxs-lookup"><span data-stu-id="a3802-124">Header</span></span>       | <span data-ttu-id="a3802-125">值</span><span class="sxs-lookup"><span data-stu-id="a3802-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a3802-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3802-126">Authorization</span></span>  | <span data-ttu-id="a3802-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a3802-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a3802-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a3802-129">Content-Type</span></span>  | <span data-ttu-id="a3802-130">application/json</span><span class="sxs-lookup"><span data-stu-id="a3802-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a3802-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3802-131">Request body</span></span>

<span data-ttu-id="a3802-132">在请求正文中，提供 [team](../resources/team.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3802-132">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a3802-133">响应</span><span class="sxs-lookup"><span data-stu-id="a3802-133">Response</span></span>

<span data-ttu-id="a3802-134">如果成功，此方法应该会在响应正文中返回 `201 Created` 响应代码和 [team](../resources/team.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a3802-134">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3802-135">示例</span><span class="sxs-lookup"><span data-stu-id="a3802-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a3802-136">请求</span><span class="sxs-lookup"><span data-stu-id="a3802-136">Request</span></span>

<span data-ttu-id="a3802-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a3802-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a3802-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3802-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
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
# <a name="c"></a>[<span data-ttu-id="a3802-139">C#</span><span class="sxs-lookup"><span data-stu-id="a3802-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3802-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3802-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3802-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3802-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3802-142">Java</span><span class="sxs-lookup"><span data-stu-id="a3802-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a3802-143">响应</span><span class="sxs-lookup"><span data-stu-id="a3802-143">Response</span></span>

<span data-ttu-id="a3802-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a3802-144">The following is an example of the response.</span></span> 

><span data-ttu-id="a3802-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a3802-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
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

## <a name="see-also"></a><span data-ttu-id="a3802-147">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a3802-147">See also</span></span>

- [<span data-ttu-id="a3802-148">创建包含团队的组</span><span class="sxs-lookup"><span data-stu-id="a3802-148">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
