---
title: 向聊天添加成员
description: 将 conversationMember 添加到聊天中。
author: bhartono
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f3fe6c34d81e34f614f914780886902a8bf563c2
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843769"
---
# <a name="add-member-to-a-chat"></a><span data-ttu-id="3ec49-103">向聊天添加成员</span><span class="sxs-lookup"><span data-stu-id="3ec49-103">Add member to a chat</span></span>

<span data-ttu-id="3ec49-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ec49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ec49-105">将 [conversationMember](../resources/conversationmember.md) 添加到 [聊天中](../resources/chat.md)。</span><span class="sxs-lookup"><span data-stu-id="3ec49-105">Add a [conversationMember](../resources/conversationmember.md) to a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3ec49-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="3ec49-106">Permissions</span></span>

<span data-ttu-id="3ec49-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ec49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ec49-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ec49-109">Permission Type</span></span>|<span data-ttu-id="3ec49-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ec49-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="3ec49-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ec49-111">Delegated (work or school account)</span></span>| <span data-ttu-id="3ec49-112">ChatMember.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ec49-112">ChatMember.ReadWrite</span></span> |
|<span data-ttu-id="3ec49-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ec49-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ec49-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ec49-114">Not supported.</span></span>|
|<span data-ttu-id="3ec49-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ec49-115">Application</span></span>| <span data-ttu-id="3ec49-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ec49-116">Not supported.</span></span> |

<!-- { "blockType": "ignored"} -->
```http
POST /chats/{chat-id}/members
```

## <a name="request-headers"></a><span data-ttu-id="3ec49-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ec49-117">Request headers</span></span>

| <span data-ttu-id="3ec49-118">标头</span><span class="sxs-lookup"><span data-stu-id="3ec49-118">Header</span></span>       | <span data-ttu-id="3ec49-119">值</span><span class="sxs-lookup"><span data-stu-id="3ec49-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3ec49-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ec49-120">Authorization</span></span>  | <span data-ttu-id="3ec49-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ec49-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="3ec49-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ec49-123">Content-Type</span></span>|<span data-ttu-id="3ec49-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3ec49-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ec49-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ec49-126">Request body</span></span>

<span data-ttu-id="3ec49-127">在请求正文中，提供 JSON 表示形式的 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3ec49-127">In the request body, supply a JSON representation of the [conversationMember](../resources/conversationmember.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3ec49-128">响应</span><span class="sxs-lookup"><span data-stu-id="3ec49-128">Response</span></span>

<span data-ttu-id="3ec49-129">如果成功，此方法将返回响应代码和位置标头，该标头提供新创建的成员 `201 Created` 对象的 URL 路径。</span><span class="sxs-lookup"><span data-stu-id="3ec49-129">If successful, this method returns a `201 Created` response code and a Location header that provides a URL path to the newly created member object.</span></span>

## <a name="examples"></a><span data-ttu-id="3ec49-130">示例</span><span class="sxs-lookup"><span data-stu-id="3ec49-130">Examples</span></span>

### <a name="example-1-add-a-single-member-to-a-chat-and-specify-the-timespan-for-the-conversation-history"></a><span data-ttu-id="3ec49-131">示例 1：向聊天中添加单个成员并指定对话历史记录的时间跨度</span><span class="sxs-lookup"><span data-stu-id="3ec49-131">Example 1: Add a single member to a chat and specify the timespan for the conversation history</span></span>

#### <a name="request"></a><span data-ttu-id="3ec49-132">请求</span><span class="sxs-lookup"><span data-stu-id="3ec49-132">Request</span></span>

<span data-ttu-id="3ec49-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ec49-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3ec49-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ec49-134">HTTP</span></span>](#tab/http)
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
    "visibleHistoryStartDateTime": "2019-04-18T23:51:43.255Z"
}
```
# <a name="javascript"></a>[<span data-ttu-id="3ec49-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ec49-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-specific-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ec49-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ec49-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-specific-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ec49-137">Java</span><span class="sxs-lookup"><span data-stu-id="3ec49-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-specific-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="3ec49-138">C#</span><span class="sxs-lookup"><span data-stu-id="3ec49-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-specific-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="3ec49-139">响应</span><span class="sxs-lookup"><span data-stu-id="3ec49-139">Response</span></span>

<span data-ttu-id="3ec49-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3ec49-140">Here is an example of the response.</span></span>

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_with_specific_visibleHistoryStartDateTime",
  "@odata.type": "Microsoft.Teams.GraphSvc.conversationMember"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```

### <a name="example-2-adding-a-single-member-to-a-microsoft-teams-chat-sharing-no-chat-history"></a><span data-ttu-id="3ec49-141">示例 2：向 Microsoft Teams 聊天添加单个成员，不共享聊天历史记录</span><span class="sxs-lookup"><span data-stu-id="3ec49-141">Example 2: Adding a single member to a Microsoft Teams chat, sharing no chat history</span></span>

#### <a name="request"></a><span data-ttu-id="3ec49-142">请求</span><span class="sxs-lookup"><span data-stu-id="3ec49-142">Request</span></span>

<span data-ttu-id="3ec49-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ec49-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3ec49-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ec49-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_no_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/beta/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
}
```

# <a name="javascript"></a>[<span data-ttu-id="3ec49-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ec49-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-no-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ec49-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ec49-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-no-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ec49-147">Java</span><span class="sxs-lookup"><span data-stu-id="3ec49-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-no-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="3ec49-148">C#</span><span class="sxs-lookup"><span data-stu-id="3ec49-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-no-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="3ec49-149">响应</span><span class="sxs-lookup"><span data-stu-id="3ec49-149">Response</span></span>

<span data-ttu-id="3ec49-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3ec49-150">Here is an example of the response.</span></span>

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_with_no_visibleHistoryStartDateTime",
  "@odata.type": "Microsoft.Teams.GraphSvc.conversationMember"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```

### <a name="example-3-adding-a-single-member-to-a-microsoft-teams-chat-sharing-the-whole-history-of-the-chat"></a><span data-ttu-id="3ec49-151">示例 3：向 Microsoft Teams 聊天添加单个成员，共享聊天的整个历史记录</span><span class="sxs-lookup"><span data-stu-id="3ec49-151">Example 3: Adding a single member to a Microsoft Teams chat, sharing the whole history of the chat</span></span>

#### <a name="request"></a><span data-ttu-id="3ec49-152">请求</span><span class="sxs-lookup"><span data-stu-id="3ec49-152">Request</span></span>

<span data-ttu-id="3ec49-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ec49-153">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3ec49-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ec49-154">HTTP</span></span>](#tab/http)
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
    "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z"
}
```
# <a name="javascript"></a>[<span data-ttu-id="3ec49-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ec49-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-all-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ec49-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ec49-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-all-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ec49-157">Java</span><span class="sxs-lookup"><span data-stu-id="3ec49-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-all-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="3ec49-158">C#</span><span class="sxs-lookup"><span data-stu-id="3ec49-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-all-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="3ec49-159">响应</span><span class="sxs-lookup"><span data-stu-id="3ec49-159">Response</span></span>

<span data-ttu-id="3ec49-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3ec49-160">Here is an example of the response.</span></span>

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_with_all_visibleHistoryStartDateTime",
  "@odata.type": "Microsoft.Teams.GraphSvc.conversationMember"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```


