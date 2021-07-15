---
title: 向聊天添加成员
description: 向聊天中添加 conversationMember。
author: bhartono
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b320a3303925b6c1527d891210a330df401f2c1f
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430072"
---
# <a name="add-member-to-a-chat"></a><span data-ttu-id="b1e23-103">向聊天添加成员</span><span class="sxs-lookup"><span data-stu-id="b1e23-103">Add member to a chat</span></span>

<span data-ttu-id="b1e23-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1e23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1e23-105">将 [conversationMember](../resources/conversationmember.md) 添加到 [聊天](../resources/chat.md)。</span><span class="sxs-lookup"><span data-stu-id="b1e23-105">Add a [conversationMember](../resources/conversationmember.md) to a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b1e23-106">权限</span><span class="sxs-lookup"><span data-stu-id="b1e23-106">Permissions</span></span>

<span data-ttu-id="b1e23-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1e23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1e23-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1e23-109">Permission Type</span></span>|<span data-ttu-id="b1e23-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b1e23-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="b1e23-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1e23-111">Delegated (work or school account)</span></span>| <span data-ttu-id="b1e23-112">ChatMember.ReadWrite、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1e23-112">ChatMember.ReadWrite, Chat.ReadWrite</span></span> |
|<span data-ttu-id="b1e23-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1e23-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1e23-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1e23-114">Not supported.</span></span>|
|<span data-ttu-id="b1e23-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1e23-115">Application</span></span>| <span data-ttu-id="b1e23-116">Chat.Manage.Chat\*、ChatMember.ReadWrite.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1e23-116">Chat.Manage.Chat\*, ChatMember.ReadWrite.All, Chat.ReadWrite.All</span></span> |

> <span data-ttu-id="b1e23-117">**注意**：标有 \* 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="b1e23-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

<!-- { "blockType": "ignored"} -->
```http
POST /chats/{chat-id}/members
```

## <a name="request-headers"></a><span data-ttu-id="b1e23-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1e23-118">Request headers</span></span>

| <span data-ttu-id="b1e23-119">标头</span><span class="sxs-lookup"><span data-stu-id="b1e23-119">Header</span></span>       | <span data-ttu-id="b1e23-120">值</span><span class="sxs-lookup"><span data-stu-id="b1e23-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b1e23-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1e23-121">Authorization</span></span>  | <span data-ttu-id="b1e23-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b1e23-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="b1e23-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b1e23-124">Content-Type</span></span>|<span data-ttu-id="b1e23-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b1e23-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1e23-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1e23-127">Request body</span></span>

<span data-ttu-id="b1e23-128">在请求正文中，提供 JSON 表示形式的 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1e23-128">In the request body, supply a JSON representation of the [conversationMember](../resources/conversationmember.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b1e23-129">响应</span><span class="sxs-lookup"><span data-stu-id="b1e23-129">Response</span></span>

<span data-ttu-id="b1e23-130">如果成功，此方法返回 响应代码和 Location 标头，这些响应代码和位置标头提供指向新创建的成员 `201 Created` 对象的 URL 路径。</span><span class="sxs-lookup"><span data-stu-id="b1e23-130">If successful, this method returns a `201 Created` response code and a Location header that provides a URL path to the newly created member object.</span></span>

## <a name="examples"></a><span data-ttu-id="b1e23-131">示例</span><span class="sxs-lookup"><span data-stu-id="b1e23-131">Examples</span></span>

### <a name="example-1-add-a-single-member-to-a-chat-and-specify-the-timespan-for-the-conversation-history"></a><span data-ttu-id="b1e23-132">示例 1：向聊天中添加单个成员并指定对话历史记录的时间跨度</span><span class="sxs-lookup"><span data-stu-id="b1e23-132">Example 1: Add a single member to a chat and specify the timespan for the conversation history</span></span>

#### <a name="request"></a><span data-ttu-id="b1e23-133">请求</span><span class="sxs-lookup"><span data-stu-id="b1e23-133">Request</span></span>

<span data-ttu-id="b1e23-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1e23-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b1e23-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1e23-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_specific_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/beta/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5",
    "visibleHistoryStartDateTime": "2019-04-18T23:51:43.255Z",
    "roles": ["owner"]
}
```
# <a name="javascript"></a>[<span data-ttu-id="b1e23-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1e23-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-specific-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1e23-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1e23-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-specific-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b1e23-138">Java</span><span class="sxs-lookup"><span data-stu-id="b1e23-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-specific-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="b1e23-139">C#</span><span class="sxs-lookup"><span data-stu-id="b1e23-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-specific-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="b1e23-140">响应</span><span class="sxs-lookup"><span data-stu-id="b1e23-140">Response</span></span>

<span data-ttu-id="b1e23-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b1e23-141">Here is an example of the response.</span></span>

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_with_specific_visibleHistoryStartDateTime"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```

### <a name="example-2-adding-a-single-member-to-a-microsoft-teams-chat-sharing-no-chat-history"></a><span data-ttu-id="b1e23-142">示例 2：将单个成员添加到聊天Microsoft Teams，不共享聊天历史记录</span><span class="sxs-lookup"><span data-stu-id="b1e23-142">Example 2: Adding a single member to a Microsoft Teams chat, sharing no chat history</span></span>

#### <a name="request"></a><span data-ttu-id="b1e23-143">请求</span><span class="sxs-lookup"><span data-stu-id="b1e23-143">Request</span></span>

<span data-ttu-id="b1e23-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1e23-144">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b1e23-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1e23-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_no_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/beta/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5",
    "roles": ["owner"]
}
```

# <a name="javascript"></a>[<span data-ttu-id="b1e23-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1e23-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-no-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1e23-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1e23-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-no-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b1e23-148">Java</span><span class="sxs-lookup"><span data-stu-id="b1e23-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-no-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="b1e23-149">C#</span><span class="sxs-lookup"><span data-stu-id="b1e23-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-no-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="b1e23-150">响应</span><span class="sxs-lookup"><span data-stu-id="b1e23-150">Response</span></span>

<span data-ttu-id="b1e23-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b1e23-151">Here is an example of the response.</span></span>

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_with_no_visibleHistoryStartDateTime"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```

### <a name="example-3-adding-a-single-member-to-a-microsoft-teams-chat-sharing-the-whole-history-of-the-chat"></a><span data-ttu-id="b1e23-152">示例 3：将单个成员添加到Microsoft Teams聊天，共享聊天的整个历史记录</span><span class="sxs-lookup"><span data-stu-id="b1e23-152">Example 3: Adding a single member to a Microsoft Teams chat, sharing the whole history of the chat</span></span>

#### <a name="request"></a><span data-ttu-id="b1e23-153">请求</span><span class="sxs-lookup"><span data-stu-id="b1e23-153">Request</span></span>

<span data-ttu-id="b1e23-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1e23-154">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b1e23-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1e23-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_all_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/beta/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5",
    "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z",
    "roles": ["owner"]
}
```
# <a name="javascript"></a>[<span data-ttu-id="b1e23-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1e23-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-all-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1e23-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1e23-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-all-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b1e23-158">Java</span><span class="sxs-lookup"><span data-stu-id="b1e23-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-all-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="b1e23-159">C#</span><span class="sxs-lookup"><span data-stu-id="b1e23-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-all-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="b1e23-160">响应</span><span class="sxs-lookup"><span data-stu-id="b1e23-160">Response</span></span>

<span data-ttu-id="b1e23-161">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b1e23-161">Here is an example of the response.</span></span>

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_with_all_visibleHistoryStartDateTime"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```


