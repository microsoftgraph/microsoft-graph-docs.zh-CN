---
title: 列出 conversationMembers
description: 检索聊天或频道成员的列表。
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cf0b60d6ac5939a519a6da35b47a646c3d94c8af
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782983"
---
# <a name="list-conversationmembers"></a><span data-ttu-id="c4506-103">列出 conversationMembers</span><span class="sxs-lookup"><span data-stu-id="c4506-103">List conversationMembers</span></span>

<span data-ttu-id="c4506-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4506-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c4506-105">列出[聊天](../resources/chatmessage.md)或[频道](../resources/channel.md)中的所有[对话成员](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="c4506-105">List all [conversation members](../resources/conversationmember.md) in a [chat](../resources/chatmessage.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4506-106">权限</span><span class="sxs-lookup"><span data-stu-id="c4506-106">Permissions</span></span>

<span data-ttu-id="c4506-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4506-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4506-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4506-109">Permission Type</span></span>|<span data-ttu-id="c4506-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4506-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="c4506-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4506-111">Delegated (work or school account)</span></span>| <span data-ttu-id="c4506-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4506-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="c4506-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4506-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4506-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4506-114">Not supported.</span></span>|
|<span data-ttu-id="c4506-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4506-115">Application</span></span>| <span data-ttu-id="c4506-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4506-116">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="c4506-117">在调用具有应用程序权限的此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="c4506-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="c4506-118">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="c4506-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="c4506-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4506-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members
GET /users/{id}/chats/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4506-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c4506-120">Optional query parameters</span></span>

<span data-ttu-id="c4506-121">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c4506-121">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4506-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4506-122">Request headers</span></span>

| <span data-ttu-id="c4506-123">标头</span><span class="sxs-lookup"><span data-stu-id="c4506-123">Header</span></span>       | <span data-ttu-id="c4506-124">值</span><span class="sxs-lookup"><span data-stu-id="c4506-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c4506-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4506-125">Authorization</span></span>  | <span data-ttu-id="c4506-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4506-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c4506-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4506-128">Request body</span></span>

<span data-ttu-id="c4506-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c4506-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4506-130">响应</span><span class="sxs-lookup"><span data-stu-id="c4506-130">Response</span></span>

<span data-ttu-id="c4506-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="c4506-131">If successful, this method returns a `200 OK` response code and a list of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4506-132">示例</span><span class="sxs-lookup"><span data-stu-id="c4506-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4506-133">请求</span><span class="sxs-lookup"><span data-stu-id="c4506-133">Request</span></span>

<span data-ttu-id="c4506-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c4506-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c4506-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4506-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_conversation_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/chats/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="c4506-136">C#</span><span class="sxs-lookup"><span data-stu-id="c4506-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-conversation-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4506-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4506-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-conversation-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4506-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4506-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-conversation-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4506-139">Java</span><span class="sxs-lookup"><span data-stu-id="c4506-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-conversation-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c4506-140">响应</span><span class="sxs-lookup"><span data-stu-id="c4506-140">Response</span></span>

<span data-ttu-id="c4506-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c4506-141">The following is an example of the response.</span></span>

><span data-ttu-id="c4506-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c4506-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d%40unq.gbl.spaces')/members",
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
