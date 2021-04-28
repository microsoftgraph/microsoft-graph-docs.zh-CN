---
title: 列出聊天成员。
description: 检索聊天成员。
author: bhartono
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e96fdce4e22aa1f83337ca9be938b648394808ac
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047292"
---
# <a name="list-members-of-a-chat"></a><span data-ttu-id="34a1c-103">列出聊天成员。</span><span class="sxs-lookup"><span data-stu-id="34a1c-103">List members of a chat</span></span>

<span data-ttu-id="34a1c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34a1c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34a1c-105">列出[聊天](../resources/chat.md)中的所有[对话成员](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="34a1c-105">List all [conversation members](../resources/conversationmember.md) in a [chat](../resources/chat.md).</span></span>

> [!NOTE]
> <span data-ttu-id="34a1c-106">服务器返回的成员 ID 必须作为不透明的字符串处理。</span><span class="sxs-lookup"><span data-stu-id="34a1c-106">The membership IDs returned by the server must be treated as opaque strings.</span></span> <span data-ttu-id="34a1c-107">客户端不应尝试对这些资源 ID 进行分析或做出任何假设。</span><span class="sxs-lookup"><span data-stu-id="34a1c-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="34a1c-p102">成员资格结果将来可能会映射到来自不同租户的用户，如响应中所示。客户端不应假定所有成员仅来自当前租户。</span><span class="sxs-lookup"><span data-stu-id="34a1c-p102">The membership results could map to users from different tenants, as indicated in the response, in the future. The client should not assume that all members are from the current tenant only.</span></span>

## <a name="permissions"></a><span data-ttu-id="34a1c-110">权限</span><span class="sxs-lookup"><span data-stu-id="34a1c-110">Permissions</span></span>

<span data-ttu-id="34a1c-p103">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34a1c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34a1c-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="34a1c-113">Permission Type</span></span>|<span data-ttu-id="34a1c-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="34a1c-114">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="34a1c-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34a1c-115">Delegated (work or school account)</span></span>| <span data-ttu-id="34a1c-116">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34a1c-116">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="34a1c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34a1c-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34a1c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="34a1c-118">Not supported.</span></span>|
|<span data-ttu-id="34a1c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="34a1c-119">Application</span></span>| <span data-ttu-id="34a1c-120">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="34a1c-120">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All.</span></span> |

> [!NOTE]
> <span data-ttu-id="34a1c-121">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="34a1c-121">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="34a1c-122">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="34a1c-122">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="34a1c-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34a1c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/members
GET /users/{user-id}/chats/{chat-id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="34a1c-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="34a1c-124">Optional query parameters</span></span>

<span data-ttu-id="34a1c-125">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="34a1c-125">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34a1c-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="34a1c-126">Request headers</span></span>

| <span data-ttu-id="34a1c-127">标头</span><span class="sxs-lookup"><span data-stu-id="34a1c-127">Header</span></span>       | <span data-ttu-id="34a1c-128">值</span><span class="sxs-lookup"><span data-stu-id="34a1c-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="34a1c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="34a1c-129">Authorization</span></span>  | <span data-ttu-id="34a1c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="34a1c-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="34a1c-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="34a1c-132">Request body</span></span>

<span data-ttu-id="34a1c-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="34a1c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34a1c-134">响应</span><span class="sxs-lookup"><span data-stu-id="34a1c-134">Response</span></span>

<span data-ttu-id="34a1c-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="34a1c-135">If successful, this method returns a `200 OK` response code and a list of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34a1c-136">示例</span><span class="sxs-lookup"><span data-stu-id="34a1c-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="34a1c-137">请求</span><span class="sxs-lookup"><span data-stu-id="34a1c-137">Request</span></span>

<span data-ttu-id="34a1c-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="34a1c-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="34a1c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="34a1c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_conversation_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/chats/19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d@unq.gbl.spaces/members
```
# <a name="c"></a>[<span data-ttu-id="34a1c-140">C#</span><span class="sxs-lookup"><span data-stu-id="34a1c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-conversation-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="34a1c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34a1c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-conversation-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="34a1c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34a1c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-conversation-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="34a1c-143">Java</span><span class="sxs-lookup"><span data-stu-id="34a1c-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-conversation-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="34a1c-144">响应</span><span class="sxs-lookup"><span data-stu-id="34a1c-144">Response</span></span>

<span data-ttu-id="34a1c-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="34a1c-145">Here is an example of the response.</span></span>

><span data-ttu-id="34a1c-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="34a1c-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d%40unq.gbl.spaces')/members",
    "@odata.count": 3,
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "roles": [
                "owner"
            ],
            "displayName": "John Doe",
            "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "email": null,
            "tenantId": "6e5147da-6a35-4275-b3f3-fc069456b6eb",
            "visibleHistoryStartDateTime": "2019-04-18T23:51:43.255Z"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "2de87aaf-844d-4def-9dee-2c317f0be1b3",
            "roles": [
                "owner"
            ],
            "displayName": "Bart Hogan",
            "userId": "2de87aaf-844d-4def-9dee-2c317f0be1b3",
            "email": null,
            "tenantId": "6e5147da-6a35-4275-b3f3-fc069456b6eb",
            "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z"
    },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "07ad17ad-ada5-4f1f-a650-7a963886a8a7",
            "roles": [
                "owner"
            ],
            "displayName": "Minna Pham",
            "userId": "07ad17ad-ada5-4f1f-a650-7a963886a8a7",
            "email": null,
            "tenantId": "6e5147da-6a35-4275-b3f3-fc069456b6eb",
            "visibleHistoryStartDateTime": "2019-04-18T23:51:43.255Z"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation: member list",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


