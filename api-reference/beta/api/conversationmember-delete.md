---
title: 删除 conversationMember
description: 从频道中删除 conversationMember。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bd741926b7627dcb6926501569d17eb2191029f4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956792"
---
# <a name="delete-conversationmember"></a><span data-ttu-id="a9b7a-103">删除 conversationMember</span><span class="sxs-lookup"><span data-stu-id="a9b7a-103">Delete conversationMember</span></span>

<span data-ttu-id="a9b7a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9b7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9b7a-105">从[频道](../resources/channel.md)中删除[conversationMember](../resources/conversationmember.md) 。</span><span class="sxs-lookup"><span data-stu-id="a9b7a-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="a9b7a-106">此操作仅在具有 [channelMembershipType](../resources/enums.md#channelmembershiptype-values) 的通道上受支持 `private` 。</span><span class="sxs-lookup"><span data-stu-id="a9b7a-106">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="a9b7a-107">与任何其他 [channelMembershipType](../resources/enums.md#channelmembershiptype-values) 的调用将返回 `400 Bad Request` 响应。</span><span class="sxs-lookup"><span data-stu-id="a9b7a-107">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9b7a-108">权限</span><span class="sxs-lookup"><span data-stu-id="a9b7a-108">Permissions</span></span>

<span data-ttu-id="a9b7a-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9b7a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9b7a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9b7a-111">Permission Type</span></span>|<span data-ttu-id="a9b7a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9b7a-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="a9b7a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9b7a-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a9b7a-114">ChannelMember、Group 写全部、所有的 ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="a9b7a-114">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="a9b7a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9b7a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9b7a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9b7a-116">Not supported.</span></span>|
|<span data-ttu-id="a9b7a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9b7a-117">Application</span></span>| <span data-ttu-id="a9b7a-118">ChannelMember、Group 写全部、所有的 ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="a9b7a-118">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9b7a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9b7a-119">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a9b7a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9b7a-120">Request headers</span></span>

| <span data-ttu-id="a9b7a-121">标头</span><span class="sxs-lookup"><span data-stu-id="a9b7a-121">Header</span></span>       | <span data-ttu-id="a9b7a-122">值</span><span class="sxs-lookup"><span data-stu-id="a9b7a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a9b7a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9b7a-123">Authorization</span></span>  | <span data-ttu-id="a9b7a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a9b7a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a9b7a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9b7a-126">Request body</span></span>

<span data-ttu-id="a9b7a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a9b7a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9b7a-128">响应</span><span class="sxs-lookup"><span data-stu-id="a9b7a-128">Response</span></span>

<span data-ttu-id="a9b7a-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a9b7a-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a9b7a-130">示例</span><span class="sxs-lookup"><span data-stu-id="a9b7a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9b7a-131">请求</span><span class="sxs-lookup"><span data-stu-id="a9b7a-131">Request</span></span>

<span data-ttu-id="a9b7a-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a9b7a-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9b7a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9b7a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="a9b7a-134">C#</span><span class="sxs-lookup"><span data-stu-id="a9b7a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9b7a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9b7a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9b7a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9b7a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9b7a-137">Java</span><span class="sxs-lookup"><span data-stu-id="a9b7a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-conversation-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a9b7a-138">响应</span><span class="sxs-lookup"><span data-stu-id="a9b7a-138">Response</span></span>

<span data-ttu-id="a9b7a-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a9b7a-139">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```


