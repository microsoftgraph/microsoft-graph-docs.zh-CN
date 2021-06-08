---
title: 向聊天添加成员
description: 向聊天中添加 conversationMember。
author: bhartono
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d5355d04f573d368052be374cc0ddc57b16b1247
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786543"
---
# <a name="add-member-to-a-chat"></a><span data-ttu-id="f2b5d-103">向聊天添加成员</span><span class="sxs-lookup"><span data-stu-id="f2b5d-103">Add member to a chat</span></span>

<span data-ttu-id="f2b5d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2b5d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2b5d-105">将 [conversationMember](../resources/conversationmember.md) 添加到 [聊天](../resources/chat.md)。</span><span class="sxs-lookup"><span data-stu-id="f2b5d-105">Add a [conversationMember](../resources/conversationmember.md) to a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f2b5d-106">权限</span><span class="sxs-lookup"><span data-stu-id="f2b5d-106">Permissions</span></span>

<span data-ttu-id="f2b5d-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2b5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2b5d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2b5d-109">Permission Type</span></span>|<span data-ttu-id="f2b5d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2b5d-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="f2b5d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2b5d-111">Delegated (work or school account)</span></span>| <span data-ttu-id="f2b5d-112">ChatMember.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2b5d-112">ChatMember.ReadWrite</span></span> |
|<span data-ttu-id="f2b5d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2b5d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2b5d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2b5d-114">Not supported.</span></span>|
|<span data-ttu-id="f2b5d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2b5d-115">Application</span></span>| <span data-ttu-id="f2b5d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2b5d-116">Not supported.</span></span> |

<!-- { "blockType": "ignored"} -->
```http
POST /chats/{chat-id}/members
```

## <a name="request-headers"></a><span data-ttu-id="f2b5d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2b5d-117">Request headers</span></span>

| <span data-ttu-id="f2b5d-118">标头</span><span class="sxs-lookup"><span data-stu-id="f2b5d-118">Header</span></span>       | <span data-ttu-id="f2b5d-119">值</span><span class="sxs-lookup"><span data-stu-id="f2b5d-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f2b5d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2b5d-120">Authorization</span></span>  | <span data-ttu-id="f2b5d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2b5d-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="f2b5d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f2b5d-123">Content-Type</span></span>|<span data-ttu-id="f2b5d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f2b5d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2b5d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2b5d-126">Request body</span></span>

<span data-ttu-id="f2b5d-127">在请求正文中，提供 JSON 表示形式的 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2b5d-127">In the request body, supply a JSON representation of the [conversationMember](../resources/conversationmember.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f2b5d-128">响应</span><span class="sxs-lookup"><span data-stu-id="f2b5d-128">Response</span></span>

<span data-ttu-id="f2b5d-129">如果成功，此方法返回 响应代码和 Location 标头，这些响应代码和位置标头提供指向新创建的成员 `201 Created` 对象的 URL 路径。</span><span class="sxs-lookup"><span data-stu-id="f2b5d-129">If successful, this method returns a `201 Created` response code and a Location header that provides a URL path to the newly created member object.</span></span>

## <a name="examples"></a><span data-ttu-id="f2b5d-130">示例</span><span class="sxs-lookup"><span data-stu-id="f2b5d-130">Examples</span></span>

### <a name="example-1-add-a-single-member-to-a-chat-and-specify-the-timespan-for-the-conversation-history"></a><span data-ttu-id="f2b5d-131">示例 1：向聊天中添加单个成员并指定对话历史记录的时间跨度</span><span class="sxs-lookup"><span data-stu-id="f2b5d-131">Example 1: Add a single member to a chat and specify the timespan for the conversation history</span></span>

#### <a name="request"></a><span data-ttu-id="f2b5d-132">请求</span><span class="sxs-lookup"><span data-stu-id="f2b5d-132">Request</span></span>

<span data-ttu-id="f2b5d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2b5d-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f2b5d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2b5d-134">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="f2b5d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2b5d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-specific-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2b5d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2b5d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-specific-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2b5d-137">Java</span><span class="sxs-lookup"><span data-stu-id="f2b5d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-specific-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="f2b5d-138">C#</span><span class="sxs-lookup"><span data-stu-id="f2b5d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-specific-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="f2b5d-139">响应</span><span class="sxs-lookup"><span data-stu-id="f2b5d-139">Response</span></span>

<span data-ttu-id="f2b5d-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f2b5d-140">Here is an example of the response.</span></span>

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

### <a name="example-2-adding-a-single-member-to-a-microsoft-teams-chat-sharing-no-chat-history"></a><span data-ttu-id="f2b5d-141">示例 2：将单个成员添加到聊天Microsoft Teams，不共享聊天历史记录</span><span class="sxs-lookup"><span data-stu-id="f2b5d-141">Example 2: Adding a single member to a Microsoft Teams chat, sharing no chat history</span></span>

#### <a name="request"></a><span data-ttu-id="f2b5d-142">请求</span><span class="sxs-lookup"><span data-stu-id="f2b5d-142">Request</span></span>

<span data-ttu-id="f2b5d-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2b5d-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f2b5d-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2b5d-144">HTTP</span></span>](#tab/http)
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

# <a name="javascript"></a>[<span data-ttu-id="f2b5d-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2b5d-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-no-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2b5d-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2b5d-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-no-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2b5d-147">Java</span><span class="sxs-lookup"><span data-stu-id="f2b5d-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-no-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="f2b5d-148">C#</span><span class="sxs-lookup"><span data-stu-id="f2b5d-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-no-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="f2b5d-149">响应</span><span class="sxs-lookup"><span data-stu-id="f2b5d-149">Response</span></span>

<span data-ttu-id="f2b5d-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f2b5d-150">Here is an example of the response.</span></span>

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

### <a name="example-3-adding-a-single-member-to-a-microsoft-teams-chat-sharing-the-whole-history-of-the-chat"></a><span data-ttu-id="f2b5d-151">示例 3：将单个成员添加到Microsoft Teams聊天，共享聊天的整个历史记录</span><span class="sxs-lookup"><span data-stu-id="f2b5d-151">Example 3: Adding a single member to a Microsoft Teams chat, sharing the whole history of the chat</span></span>

#### <a name="request"></a><span data-ttu-id="f2b5d-152">请求</span><span class="sxs-lookup"><span data-stu-id="f2b5d-152">Request</span></span>

<span data-ttu-id="f2b5d-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2b5d-153">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f2b5d-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2b5d-154">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="f2b5d-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2b5d-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-all-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2b5d-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2b5d-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-all-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2b5d-157">Java</span><span class="sxs-lookup"><span data-stu-id="f2b5d-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-all-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="f2b5d-158">C#</span><span class="sxs-lookup"><span data-stu-id="f2b5d-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-all-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="f2b5d-159">响应</span><span class="sxs-lookup"><span data-stu-id="f2b5d-159">Response</span></span>

<span data-ttu-id="f2b5d-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f2b5d-160">Here is an example of the response.</span></span>

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


