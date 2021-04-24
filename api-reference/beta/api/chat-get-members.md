---
title: 获取聊天中的 conversationMember
description: 检索聊天成员。
author: bhartono
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 067575ac3fa19ed1763c88923f97b20a0126a25e
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961336"
---
# <a name="get-conversationmember-in-a-chat"></a><span data-ttu-id="cfca9-103">获取聊天中的 conversationMember</span><span class="sxs-lookup"><span data-stu-id="cfca9-103">Get conversationMember in a chat</span></span>

<span data-ttu-id="cfca9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfca9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfca9-105">从[聊天](../resources/chat.md)中检索 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="cfca9-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

> [!NOTE]
> <span data-ttu-id="cfca9-106">服务器返回的成员 ID 必须作为不透明的字符串处理。</span><span class="sxs-lookup"><span data-stu-id="cfca9-106">The membership IDs returned by the server must be treated as opaque strings.</span></span> <span data-ttu-id="cfca9-107">客户端不应尝试对这些资源 ID 进行分析或做出任何假设。</span><span class="sxs-lookup"><span data-stu-id="cfca9-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="cfca9-108">成员资格结果将来可能会映射到来自不同租户的用户，如响应中所示。</span><span class="sxs-lookup"><span data-stu-id="cfca9-108">The membership results could map to users from different tenants, as indicated in the response, in the future.</span></span> <span data-ttu-id="cfca9-109">客户端不应假定所有成员都仅来自当前租户。</span><span class="sxs-lookup"><span data-stu-id="cfca9-109">The client should not assume that all members are from the current tenant only.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfca9-110">权限</span><span class="sxs-lookup"><span data-stu-id="cfca9-110">Permissions</span></span>

<span data-ttu-id="cfca9-p103">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cfca9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfca9-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="cfca9-113">Permission Type</span></span>|<span data-ttu-id="cfca9-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cfca9-114">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="cfca9-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cfca9-115">Delegated (work or school account)</span></span>| <span data-ttu-id="cfca9-116">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfca9-116">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="cfca9-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cfca9-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfca9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfca9-118">Not supported.</span></span>|
|<span data-ttu-id="cfca9-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="cfca9-119">Application</span></span>| <span data-ttu-id="cfca9-120">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="cfca9-120">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All.</span></span> |

> <span data-ttu-id="cfca9-121">**注意**：标有 \* 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="cfca9-121">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="cfca9-122">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="cfca9-122">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="cfca9-123">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="cfca9-123">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="cfca9-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cfca9-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/members/{membership-id}
GET /users/{user-id}/chats/{chat-id}/members/{membership-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cfca9-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cfca9-125">Optional query parameters</span></span>

<span data-ttu-id="cfca9-126">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cfca9-126">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cfca9-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="cfca9-127">Request headers</span></span>

| <span data-ttu-id="cfca9-128">标头</span><span class="sxs-lookup"><span data-stu-id="cfca9-128">Header</span></span>       | <span data-ttu-id="cfca9-129">值</span><span class="sxs-lookup"><span data-stu-id="cfca9-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cfca9-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfca9-130">Authorization</span></span>  | <span data-ttu-id="cfca9-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cfca9-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cfca9-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="cfca9-133">Request body</span></span>

<span data-ttu-id="cfca9-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cfca9-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfca9-135">响应</span><span class="sxs-lookup"><span data-stu-id="cfca9-135">Response</span></span>

<span data-ttu-id="cfca9-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cfca9-136">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfca9-137">示例</span><span class="sxs-lookup"><span data-stu-id="cfca9-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfca9-138">请求</span><span class="sxs-lookup"><span data-stu-id="cfca9-138">Request</span></span>

<span data-ttu-id="cfca9-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cfca9-139">Here is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/chats/19:b8577894a63548969c5c92bb9c80c5e1@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzJjOGQyYjVjLTE4NDktNDA2Ni1iNTdkLWU3YTBlOWU0NGVjOA==
```

### <a name="response"></a><span data-ttu-id="cfca9-140">响应</span><span class="sxs-lookup"><span data-stu-id="cfca9-140">Response</span></span>

<span data-ttu-id="cfca9-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cfca9-141">Here is an example of the response.</span></span>

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


