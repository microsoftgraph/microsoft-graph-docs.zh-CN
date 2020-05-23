---
title: 列出 conversationMembers
description: 检索聊天或频道成员。
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f5454db8b04fee03c2c5ae27e0842df6aa0781fb
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288513"
---
# <a name="list-conversationmembers"></a><span data-ttu-id="0587b-103">列出 conversationMembers</span><span class="sxs-lookup"><span data-stu-id="0587b-103">List conversationMembers</span></span>

<span data-ttu-id="0587b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0587b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0587b-105">列出[聊天](../resources/chat.md)或[频道](../resources/channel.md)中的所有[对话成员](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="0587b-105">List all [conversation members](../resources/conversationmember.md) in a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0587b-106">权限</span><span class="sxs-lookup"><span data-stu-id="0587b-106">Permissions</span></span>

<span data-ttu-id="0587b-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0587b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0587b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0587b-109">Permission Type</span></span>|<span data-ttu-id="0587b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0587b-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="0587b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0587b-111">Delegated (work or school account)</span></span>| <span data-ttu-id="0587b-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0587b-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="0587b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0587b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0587b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0587b-114">Not supported.</span></span>|
|<span data-ttu-id="0587b-115">Application</span><span class="sxs-lookup"><span data-stu-id="0587b-115">Application</span></span>| <span data-ttu-id="0587b-116">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0587b-116">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="0587b-117">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="0587b-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="0587b-118">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="0587b-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="0587b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0587b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members
GET /users/{id}/chats/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0587b-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0587b-120">Optional query parameters</span></span>

<span data-ttu-id="0587b-121">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0587b-121">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0587b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="0587b-122">Request headers</span></span>

| <span data-ttu-id="0587b-123">标头</span><span class="sxs-lookup"><span data-stu-id="0587b-123">Header</span></span>       | <span data-ttu-id="0587b-124">值</span><span class="sxs-lookup"><span data-stu-id="0587b-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0587b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0587b-125">Authorization</span></span>  | <span data-ttu-id="0587b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0587b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0587b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0587b-128">Request body</span></span>

<span data-ttu-id="0587b-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0587b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0587b-130">响应</span><span class="sxs-lookup"><span data-stu-id="0587b-130">Response</span></span>

<span data-ttu-id="0587b-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="0587b-131">If successful, this method returns a `200 OK` response code and a list of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0587b-132">示例</span><span class="sxs-lookup"><span data-stu-id="0587b-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0587b-133">请求</span><span class="sxs-lookup"><span data-stu-id="0587b-133">Request</span></span>

<span data-ttu-id="0587b-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0587b-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0587b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0587b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_conversation_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/chats/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="0587b-136">C#</span><span class="sxs-lookup"><span data-stu-id="0587b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-conversation-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0587b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0587b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-conversation-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0587b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0587b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-conversation-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0587b-139">响应</span><span class="sxs-lookup"><span data-stu-id="0587b-139">Response</span></span>

<span data-ttu-id="0587b-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0587b-140">Here is an example of the response.</span></span>

><span data-ttu-id="0587b-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0587b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d%40unq.gbl.spaces')/members",
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "roles": [],
            "displayName": "John Doe",
            "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "email": null
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
