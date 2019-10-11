---
title: 列出 conversationMembers
description: 检索聊天或频道成员。
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 00d3a31d11f354204a64c1957d611a06f5c004be
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439804"
---
# <a name="list-conversationmembers"></a><span data-ttu-id="e5925-103">列出 conversationMembers</span><span class="sxs-lookup"><span data-stu-id="e5925-103">List conversationMembers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5925-104">列出[聊天](../resources/chat.md)或[频道](../resources/channel.md)中的所有[对话成员](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="e5925-104">List all [conversation members](../resources/conversationmember.md) in a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e5925-105">权限</span><span class="sxs-lookup"><span data-stu-id="e5925-105">Permissions</span></span>

<span data-ttu-id="e5925-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5925-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5925-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5925-108">Permission Type</span></span>|<span data-ttu-id="e5925-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5925-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="e5925-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5925-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e5925-111">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5925-111">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="e5925-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5925-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5925-113">不支持</span><span class="sxs-lookup"><span data-stu-id="e5925-113">Not supported</span></span>|
|<span data-ttu-id="e5925-114">Application</span><span class="sxs-lookup"><span data-stu-id="e5925-114">Application</span></span>| <span data-ttu-id="e5925-115">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5925-115">Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="e5925-116">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="e5925-116">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="e5925-117">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="e5925-117">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="e5925-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5925-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members
GET /users/{id}/chats/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5925-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e5925-119">Optional query parameters</span></span>

<span data-ttu-id="e5925-120">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e5925-120">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5925-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5925-121">Request headers</span></span>

| <span data-ttu-id="e5925-122">标头</span><span class="sxs-lookup"><span data-stu-id="e5925-122">Header</span></span>       | <span data-ttu-id="e5925-123">值</span><span class="sxs-lookup"><span data-stu-id="e5925-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e5925-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5925-124">Authorization</span></span>  | <span data-ttu-id="e5925-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5925-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e5925-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5925-127">Request body</span></span>

<span data-ttu-id="e5925-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e5925-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5925-129">响应</span><span class="sxs-lookup"><span data-stu-id="e5925-129">Response</span></span>

<span data-ttu-id="e5925-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="e5925-130">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5925-131">示例</span><span class="sxs-lookup"><span data-stu-id="e5925-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e5925-132">请求</span><span class="sxs-lookup"><span data-stu-id="e5925-132">Request</span></span>

<span data-ttu-id="e5925-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5925-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e5925-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5925-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_conversation_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/chats/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e5925-135">C#</span><span class="sxs-lookup"><span data-stu-id="e5925-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-conversation-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e5925-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5925-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-conversation-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e5925-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5925-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-conversation-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e5925-138">响应</span><span class="sxs-lookup"><span data-stu-id="e5925-138">Response</span></span>

<span data-ttu-id="e5925-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e5925-139">Here is an example of the response.</span></span>

><span data-ttu-id="e5925-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e5925-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
