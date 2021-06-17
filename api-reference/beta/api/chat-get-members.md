---
title: 获取聊天中的 conversationMember
description: 检索聊天成员。
author: bhartono
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7b747374afd1138c4270784dbdca58d644802c8f
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971333"
---
# <a name="get-conversationmember-in-a-chat"></a><span data-ttu-id="a405f-103">获取聊天中的 conversationMember</span><span class="sxs-lookup"><span data-stu-id="a405f-103">Get conversationMember in a chat</span></span>

<span data-ttu-id="a405f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a405f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a405f-105">从[聊天](../resources/chat.md)中检索 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="a405f-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

> [!NOTE]
> <span data-ttu-id="a405f-106">服务器返回的成员 ID 必须作为不透明的字符串处理。</span><span class="sxs-lookup"><span data-stu-id="a405f-106">The membership IDs returned by the server must be treated as opaque strings.</span></span> <span data-ttu-id="a405f-107">客户端不应尝试对这些资源 ID 进行分析或做出任何假设。</span><span class="sxs-lookup"><span data-stu-id="a405f-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="a405f-p102">未来，成员资格结果可以映射到来自不同租户的用户，如响应中所示。客户端不应假定所有成员仅来自当前租户。</span><span class="sxs-lookup"><span data-stu-id="a405f-p102">The membership results could map to users from different tenants, as indicated in the response, in the future. The client should not assume that all members are from the current tenant only.</span></span>

## <a name="permissions"></a><span data-ttu-id="a405f-110">权限</span><span class="sxs-lookup"><span data-stu-id="a405f-110">Permissions</span></span>

<span data-ttu-id="a405f-p103">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a405f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a405f-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="a405f-113">Permission Type</span></span>|<span data-ttu-id="a405f-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a405f-114">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="a405f-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a405f-115">Delegated (work or school account)</span></span>| <span data-ttu-id="a405f-116">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a405f-116">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="a405f-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a405f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a405f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a405f-118">Not supported.</span></span>|
|<span data-ttu-id="a405f-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="a405f-119">Application</span></span>| <span data-ttu-id="a405f-120">ChatMember.Read.Chat *、Chat.Manage.Chat*、ChatMember.Read.All、ChatMember.ReadWrite.All、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a405f-120">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |

> <span data-ttu-id="a405f-121">**注意**：标有 \* 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="a405f-121">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="a405f-122">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="a405f-122">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="a405f-123">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="a405f-123">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="a405f-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a405f-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/members/{membership-id}
GET /users/{user-id | user-principal-name}/chats/{chat-id}/members/{membership-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a405f-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a405f-125">Optional query parameters</span></span>

<span data-ttu-id="a405f-126">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a405f-126">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a405f-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="a405f-127">Request headers</span></span>

| <span data-ttu-id="a405f-128">标头</span><span class="sxs-lookup"><span data-stu-id="a405f-128">Header</span></span>       | <span data-ttu-id="a405f-129">值</span><span class="sxs-lookup"><span data-stu-id="a405f-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a405f-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="a405f-130">Authorization</span></span>  | <span data-ttu-id="a405f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a405f-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a405f-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="a405f-133">Request body</span></span>

<span data-ttu-id="a405f-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a405f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a405f-135">响应</span><span class="sxs-lookup"><span data-stu-id="a405f-135">Response</span></span>

<span data-ttu-id="a405f-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a405f-136">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a405f-137">示例</span><span class="sxs-lookup"><span data-stu-id="a405f-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="a405f-138">请求</span><span class="sxs-lookup"><span data-stu-id="a405f-138">Request</span></span>

<span data-ttu-id="a405f-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a405f-139">Here is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="a405f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="a405f-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:b8577894a63548969c5c92bb9c80c5e1@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzJjOGQyYjVjLTE4NDktNDA2Ni1iNTdkLWU3YTBlOWU0NGVjOA==
```
# <a name="c"></a>[<span data-ttu-id="a405f-141">C#</span><span class="sxs-lookup"><span data-stu-id="a405f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a405f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a405f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a405f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a405f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a405f-144">Java</span><span class="sxs-lookup"><span data-stu-id="a405f-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a405f-145">响应</span><span class="sxs-lookup"><span data-stu-id="a405f-145">Response</span></span>

<span data-ttu-id="a405f-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a405f-146">Here is an example of the response.</span></span>

<!-- 
{
  "blockType": "response",
  "truncated": true,
  "name": "get_conversation_member",
  "@odata.type": "microsoft.graph.conversationMember"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ab8577894a63548969c5c92bb9c80c5e1%40thread.v2')/members/$entity",
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzJjOGQyYjVjLTE4NDktNDA2Ni1iNTdkLWU3YTBlOWU0NGVjOA==",
    "roles": [
        "owner"
    ],
    "displayName": "John Doe",
    "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z",
    "userId": "2c8d2b5c-1849-4066-b57d-e7a0e9e44ec8",
    "email": "johndoe@contoso.onmicrosoft.com",
    "tenantId": "b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation: member get",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


