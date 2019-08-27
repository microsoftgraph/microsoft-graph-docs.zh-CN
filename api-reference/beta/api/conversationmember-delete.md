---
title: 删除 conversationMember
description: 从频道中删除 conversationMember。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 739705d2c57210d15813ad8cbed4627afef29d07
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633912"
---
# <a name="delete-conversationmember"></a><span data-ttu-id="a764d-103">删除 conversationMember</span><span class="sxs-lookup"><span data-stu-id="a764d-103">Delete conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a764d-104">从[频道](../resources/channel.md)中删除[conversationMember](../resources/conversationmember.md) 。</span><span class="sxs-lookup"><span data-stu-id="a764d-104">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="a764d-105">此操作仅在具有[channelMembershipType](../resources/enums.md#channelmembershiptype-values)的`private`通道上受支持。</span><span class="sxs-lookup"><span data-stu-id="a764d-105">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="a764d-106">与任何其他[channelMembershipType](../resources/enums.md#channelmembershiptype-values)的调用将返回`400 Bad Request`响应。</span><span class="sxs-lookup"><span data-stu-id="a764d-106">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="a764d-107">权限</span><span class="sxs-lookup"><span data-stu-id="a764d-107">Permissions</span></span>

<span data-ttu-id="a764d-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a764d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a764d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a764d-110">Permission Type</span></span>|<span data-ttu-id="a764d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a764d-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="a764d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a764d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a764d-113">对于**用户**或**聊天**资源:</span><span class="sxs-lookup"><span data-stu-id="a764d-113">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="a764d-114">聊天、阅读和读写</span><span class="sxs-lookup"><span data-stu-id="a764d-114">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="a764d-115">对于**频道**资源:</span><span class="sxs-lookup"><span data-stu-id="a764d-115">For **channel** resource:</span></span><br/><span data-ttu-id="a764d-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a764d-116">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="a764d-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a764d-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a764d-118">不支持</span><span class="sxs-lookup"><span data-stu-id="a764d-118">Not supported</span></span>|
|<span data-ttu-id="a764d-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="a764d-119">Application</span></span>| <span data-ttu-id="a764d-120">对于**用户**或**聊天**资源:</span><span class="sxs-lookup"><span data-stu-id="a764d-120">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="a764d-121">"聊天室"、"所有"、"全部聊天"</span><span class="sxs-lookup"><span data-stu-id="a764d-121">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="a764d-122">对于**频道**资源:</span><span class="sxs-lookup"><span data-stu-id="a764d-122">For **channel** resource:</span></span><br/><span data-ttu-id="a764d-123">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a764d-123">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a764d-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a764d-124">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a764d-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="a764d-125">Request headers</span></span>

| <span data-ttu-id="a764d-126">标头</span><span class="sxs-lookup"><span data-stu-id="a764d-126">Header</span></span>       | <span data-ttu-id="a764d-127">值</span><span class="sxs-lookup"><span data-stu-id="a764d-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a764d-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="a764d-128">Authorization</span></span>  | <span data-ttu-id="a764d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a764d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a764d-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="a764d-131">Request body</span></span>

<span data-ttu-id="a764d-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a764d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a764d-133">响应</span><span class="sxs-lookup"><span data-stu-id="a764d-133">Response</span></span>

<span data-ttu-id="a764d-134">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a764d-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a764d-135">示例</span><span class="sxs-lookup"><span data-stu-id="a764d-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="a764d-136">请求</span><span class="sxs-lookup"><span data-stu-id="a764d-136">Request</span></span>

<span data-ttu-id="a764d-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a764d-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a764d-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a764d-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a764d-139">C#</span><span class="sxs-lookup"><span data-stu-id="a764d-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a764d-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a764d-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a764d-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="a764d-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a764d-142">响应</span><span class="sxs-lookup"><span data-stu-id="a764d-142">Response</span></span>

<span data-ttu-id="a764d-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a764d-143">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
