---
title: 删除 conversationMember
description: 从频道中删除 conversationMember。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: dee9dfbe5e77dba544517bbfdd277c25f85f4846
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491271"
---
# <a name="delete-conversationmember"></a><span data-ttu-id="18d61-103">删除 conversationMember</span><span class="sxs-lookup"><span data-stu-id="18d61-103">Delete conversationMember</span></span>

<span data-ttu-id="18d61-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18d61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18d61-105">从[频道](../resources/channel.md)中删除[conversationMember](../resources/conversationmember.md) 。</span><span class="sxs-lookup"><span data-stu-id="18d61-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="18d61-106">此操作仅在具有[channelMembershipType](../resources/enums.md#channelmembershiptype-values)的通道上受支持 `private` 。</span><span class="sxs-lookup"><span data-stu-id="18d61-106">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="18d61-107">与任何其他[channelMembershipType](../resources/enums.md#channelmembershiptype-values)的调用将返回 `400 Bad Request` 响应。</span><span class="sxs-lookup"><span data-stu-id="18d61-107">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="18d61-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="18d61-108">Permissions</span></span>

<span data-ttu-id="18d61-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18d61-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18d61-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="18d61-111">Permission Type</span></span>|<span data-ttu-id="18d61-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18d61-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="18d61-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18d61-113">Delegated (work or school account)</span></span>| <span data-ttu-id="18d61-114">ChannelMember、Group 写全部、所有的 ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="18d61-114">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="18d61-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18d61-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18d61-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="18d61-116">Not supported.</span></span>|
|<span data-ttu-id="18d61-117">Application</span><span class="sxs-lookup"><span data-stu-id="18d61-117">Application</span></span>| <span data-ttu-id="18d61-118">ChannelMember、Group 写全部、所有的 ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="18d61-118">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18d61-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18d61-119">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="18d61-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="18d61-120">Request headers</span></span>

| <span data-ttu-id="18d61-121">标头</span><span class="sxs-lookup"><span data-stu-id="18d61-121">Header</span></span>       | <span data-ttu-id="18d61-122">值</span><span class="sxs-lookup"><span data-stu-id="18d61-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18d61-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18d61-123">Authorization</span></span>  | <span data-ttu-id="18d61-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="18d61-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18d61-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="18d61-126">Request body</span></span>

<span data-ttu-id="18d61-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="18d61-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18d61-128">响应</span><span class="sxs-lookup"><span data-stu-id="18d61-128">Response</span></span>

<span data-ttu-id="18d61-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="18d61-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="18d61-130">示例</span><span class="sxs-lookup"><span data-stu-id="18d61-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="18d61-131">请求</span><span class="sxs-lookup"><span data-stu-id="18d61-131">Request</span></span>

<span data-ttu-id="18d61-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18d61-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="18d61-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="18d61-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="18d61-134">C#</span><span class="sxs-lookup"><span data-stu-id="18d61-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18d61-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18d61-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18d61-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18d61-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="18d61-137">响应</span><span class="sxs-lookup"><span data-stu-id="18d61-137">Response</span></span>

<span data-ttu-id="18d61-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="18d61-138">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
