---
title: 删除 conversationMember
description: 从频道中删除 conversationMember。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0a6ac8b72f5dea24c0f60062b91dac7648b91e85
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436564"
---
# <a name="delete-conversationmember"></a><span data-ttu-id="4aaa2-103">删除 conversationMember</span><span class="sxs-lookup"><span data-stu-id="4aaa2-103">Delete conversationMember</span></span>

<span data-ttu-id="4aaa2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4aaa2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4aaa2-105">从[频道](../resources/channel.md)中删除[conversationMember](../resources/conversationmember.md) 。</span><span class="sxs-lookup"><span data-stu-id="4aaa2-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="4aaa2-106">此操作仅在具有[channelMembershipType](../resources/enums.md#channelmembershiptype-values)的`private`通道上受支持。</span><span class="sxs-lookup"><span data-stu-id="4aaa2-106">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="4aaa2-107">与任何其他[channelMembershipType](../resources/enums.md#channelmembershiptype-values)的调用将返回`400 Bad Request`响应。</span><span class="sxs-lookup"><span data-stu-id="4aaa2-107">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="4aaa2-108">权限</span><span class="sxs-lookup"><span data-stu-id="4aaa2-108">Permissions</span></span>

<span data-ttu-id="4aaa2-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4aaa2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4aaa2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4aaa2-111">Permission Type</span></span>|<span data-ttu-id="4aaa2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4aaa2-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="4aaa2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4aaa2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4aaa2-114">对于**用户**或**聊天**资源：</span><span class="sxs-lookup"><span data-stu-id="4aaa2-114">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="4aaa2-115">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4aaa2-115">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="4aaa2-116">对于**频道**资源：</span><span class="sxs-lookup"><span data-stu-id="4aaa2-116">For **channel** resource:</span></span><br/><span data-ttu-id="4aaa2-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4aaa2-117">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="4aaa2-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4aaa2-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4aaa2-119">不支持</span><span class="sxs-lookup"><span data-stu-id="4aaa2-119">Not supported</span></span>|
|<span data-ttu-id="4aaa2-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="4aaa2-120">Application</span></span>| <span data-ttu-id="4aaa2-121">对于**用户**或**聊天**资源：</span><span class="sxs-lookup"><span data-stu-id="4aaa2-121">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="4aaa2-122">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4aaa2-122">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="4aaa2-123">对于**频道**资源：</span><span class="sxs-lookup"><span data-stu-id="4aaa2-123">For **channel** resource:</span></span><br/><span data-ttu-id="4aaa2-124">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4aaa2-124">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4aaa2-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4aaa2-125">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4aaa2-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="4aaa2-126">Request headers</span></span>

| <span data-ttu-id="4aaa2-127">标头</span><span class="sxs-lookup"><span data-stu-id="4aaa2-127">Header</span></span>       | <span data-ttu-id="4aaa2-128">值</span><span class="sxs-lookup"><span data-stu-id="4aaa2-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4aaa2-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="4aaa2-129">Authorization</span></span>  | <span data-ttu-id="4aaa2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4aaa2-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4aaa2-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="4aaa2-132">Request body</span></span>

<span data-ttu-id="4aaa2-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4aaa2-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4aaa2-134">响应</span><span class="sxs-lookup"><span data-stu-id="4aaa2-134">Response</span></span>

<span data-ttu-id="4aaa2-135">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4aaa2-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4aaa2-136">示例</span><span class="sxs-lookup"><span data-stu-id="4aaa2-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="4aaa2-137">请求</span><span class="sxs-lookup"><span data-stu-id="4aaa2-137">Request</span></span>

<span data-ttu-id="4aaa2-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4aaa2-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4aaa2-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="4aaa2-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="4aaa2-140">C#</span><span class="sxs-lookup"><span data-stu-id="4aaa2-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4aaa2-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4aaa2-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4aaa2-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4aaa2-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4aaa2-143">响应</span><span class="sxs-lookup"><span data-stu-id="4aaa2-143">Response</span></span>

<span data-ttu-id="4aaa2-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4aaa2-144">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
