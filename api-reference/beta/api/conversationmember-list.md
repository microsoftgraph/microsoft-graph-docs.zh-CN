---
title: 列出 conversationMembers
description: 检索聊天成员。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 93b12576a43e2f50af88d4cba9c688d56d5ee056
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437422"
---
# <a name="list-conversationmembers"></a><span data-ttu-id="c8c96-103">列出 conversationMembers</span><span class="sxs-lookup"><span data-stu-id="c8c96-103">List conversationMembers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8c96-104">列出[聊天](../resources/chat.md)中的所有[对话成员](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="c8c96-104">List all [conversation members](../resources/conversationmember.md) in a [chat](../resources/chat.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="c8c96-105">权限</span><span class="sxs-lookup"><span data-stu-id="c8c96-105">Permissions</span></span>

<span data-ttu-id="c8c96-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8c96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8c96-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8c96-108">Permission Type</span></span>|<span data-ttu-id="c8c96-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c8c96-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="c8c96-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8c96-110">Delegated (work or school account)</span></span>|<span data-ttu-id="c8c96-111">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8c96-111">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="c8c96-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8c96-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8c96-113">不支持</span><span class="sxs-lookup"><span data-stu-id="c8c96-113">Not supported</span></span>|
|<span data-ttu-id="c8c96-114">Application</span><span class="sxs-lookup"><span data-stu-id="c8c96-114">Application</span></span>| <span data-ttu-id="c8c96-115">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8c96-115">Chat.Read.All, Chat.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8c96-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8c96-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members
GET /users/{id}/chats/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8c96-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c8c96-117">Optional query parameters</span></span>

<span data-ttu-id="c8c96-118">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c8c96-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8c96-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8c96-119">Request headers</span></span>

| <span data-ttu-id="c8c96-120">标头</span><span class="sxs-lookup"><span data-stu-id="c8c96-120">Header</span></span>       | <span data-ttu-id="c8c96-121">值</span><span class="sxs-lookup"><span data-stu-id="c8c96-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c8c96-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8c96-122">Authorization</span></span>  | <span data-ttu-id="c8c96-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c8c96-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c8c96-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8c96-125">Request body</span></span>

<span data-ttu-id="c8c96-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c8c96-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8c96-127">响应</span><span class="sxs-lookup"><span data-stu-id="c8c96-127">Response</span></span>

<span data-ttu-id="c8c96-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="c8c96-128">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8c96-129">示例</span><span class="sxs-lookup"><span data-stu-id="c8c96-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c8c96-130">请求</span><span class="sxs-lookup"><span data-stu-id="c8c96-130">Request</span></span>

<span data-ttu-id="c8c96-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c8c96-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c8c96-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8c96-132">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/me/chats/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c8c96-133">C#</span><span class="sxs-lookup"><span data-stu-id="c8c96-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c8c96-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="c8c96-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c8c96-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8c96-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c8c96-136">响应</span><span class="sxs-lookup"><span data-stu-id="c8c96-136">Response</span></span>

<span data-ttu-id="c8c96-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c8c96-137">Here is an example of the response.</span></span>

><span data-ttu-id="c8c96-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c8c96-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
