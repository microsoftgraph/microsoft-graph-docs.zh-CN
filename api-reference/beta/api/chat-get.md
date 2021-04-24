---
title: 获取聊天
description: 检索一个聊天。
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1862f080194f8a55c8ba0ec6fcc37d9f94b51b58
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961343"
---
# <a name="get-chat"></a><span data-ttu-id="7f1cd-103">获取聊天</span><span class="sxs-lookup"><span data-stu-id="7f1cd-103">Get chat</span></span>

<span data-ttu-id="7f1cd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f1cd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f1cd-105">检索一个[聊天](../resources/chat.md)（不含其消息）。</span><span class="sxs-lookup"><span data-stu-id="7f1cd-105">Retrieve a single [chat](../resources/chat.md) (without its messages).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f1cd-106">权限</span><span class="sxs-lookup"><span data-stu-id="7f1cd-106">Permissions</span></span>

<span data-ttu-id="7f1cd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f1cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7f1cd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f1cd-109">Permission type</span></span>      | <span data-ttu-id="7f1cd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f1cd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f1cd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f1cd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7f1cd-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f1cd-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="7f1cd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f1cd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f1cd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f1cd-114">Not supported.</span></span>    |
|<span data-ttu-id="7f1cd-115">Application</span><span class="sxs-lookup"><span data-stu-id="7f1cd-115">Application</span></span> | <span data-ttu-id="7f1cd-116">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f1cd-116">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f1cd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f1cd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{chat-id}
GET /users/{user-id}/chats/{chat-id}
GET /chats/{chat-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f1cd-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7f1cd-118">Optional query parameters</span></span>

<span data-ttu-id="7f1cd-119">此操作当前不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7f1cd-119">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f1cd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f1cd-120">Request headers</span></span>

| <span data-ttu-id="7f1cd-121">标头</span><span class="sxs-lookup"><span data-stu-id="7f1cd-121">Header</span></span>       | <span data-ttu-id="7f1cd-122">值</span><span class="sxs-lookup"><span data-stu-id="7f1cd-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7f1cd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f1cd-123">Authorization</span></span>  | <span data-ttu-id="7f1cd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7f1cd-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7f1cd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f1cd-126">Request body</span></span>

<span data-ttu-id="7f1cd-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7f1cd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f1cd-128">响应</span><span class="sxs-lookup"><span data-stu-id="7f1cd-128">Response</span></span>

<span data-ttu-id="7f1cd-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chat](../resources/chat.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7f1cd-129">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7f1cd-130">示例</span><span class="sxs-lookup"><span data-stu-id="7f1cd-130">Examples</span></span>

### <a name="example-1-get-a-group-chat"></a><span data-ttu-id="7f1cd-131">示例 1：获取群组聊天</span><span class="sxs-lookup"><span data-stu-id="7f1cd-131">Example 1: Get a group chat</span></span>
#### <a name="request"></a><span data-ttu-id="7f1cd-132">请求</span><span class="sxs-lookup"><span data-stu-id="7f1cd-132">Request</span></span>
<span data-ttu-id="7f1cd-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7f1cd-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_group_chat"
}-->
```http
GET https://graph.microsoft.com/beta/chats/19:b8577894a63548969c5c92bb9c80c5e1@thread.v2
```

#### <a name="response"></a><span data-ttu-id="7f1cd-134">响应</span><span class="sxs-lookup"><span data-stu-id="7f1cd-134">Response</span></span>
<span data-ttu-id="7f1cd-135">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="7f1cd-135">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:b8577894a63548969c5c92bb9c80c5e1@thread.v2",
    "topic": "test group 1",
    "createdDateTime": "2021-04-06T19:49:52.431Z",
    "lastUpdatedDateTime": "2021-04-06T19:54:04.306Z",
    "chatType": "group"
}
```

### <a name="example-2-get-a-users-one-on-one-chat"></a><span data-ttu-id="7f1cd-136">示例 2：通过一次聊天获取用户</span><span class="sxs-lookup"><span data-stu-id="7f1cd-136">Example 2: Get a user's one on one chat</span></span>
#### <a name="request"></a><span data-ttu-id="7f1cd-137">请求</span><span class="sxs-lookup"><span data-stu-id="7f1cd-137">Request</span></span>
<span data-ttu-id="7f1cd-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7f1cd-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7f1cd-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f1cd-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces
```
# <a name="c"></a>[<span data-ttu-id="7f1cd-140">C#</span><span class="sxs-lookup"><span data-stu-id="7f1cd-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f1cd-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f1cd-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f1cd-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f1cd-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f1cd-143">Java</span><span class="sxs-lookup"><span data-stu-id="7f1cd-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7f1cd-144">响应</span><span class="sxs-lookup"><span data-stu-id="7f1cd-144">Response</span></span>
<span data-ttu-id="7f1cd-145">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="7f1cd-145">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces",
    "topic": null,
    "createdDateTime": "2019-04-18T23:51:42.099Z",
    "lastUpdatedDateTime": "2019-04-18T23:51:43.255Z",
    "chatType": "oneOnOne"
}
```

### <a name="example-3-get-a-chat-and-all-its-members"></a><span data-ttu-id="7f1cd-146">示例 3：获取聊天及其所有成员</span><span class="sxs-lookup"><span data-stu-id="7f1cd-146">Example 3: Get a chat and all its members</span></span>
#### <a name="request"></a><span data-ttu-id="7f1cd-147">请求</span><span class="sxs-lookup"><span data-stu-id="7f1cd-147">Request</span></span>
<span data-ttu-id="7f1cd-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7f1cd-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chat_withmembers"
}-->
```http
GET https://graph.microsoft.com/beta/chats/19:b8577894a63548969c5c92bb9c80c5e1@thread.v2?$expand=members
```

#### <a name="response"></a><span data-ttu-id="7f1cd-149">响应</span><span class="sxs-lookup"><span data-stu-id="7f1cd-149">Response</span></span>
<span data-ttu-id="7f1cd-150">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="7f1cd-150">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats(members())/$entity",
    "id": "19:b8577894a63548969c5c92bb9c80c5e1@thread.v2",
    "topic": "test group 1",
    "createdDateTime": "2021-04-06T19:49:52.431Z",
    "lastUpdatedDateTime": "2021-04-21T17:13:44.033Z",
    "chatType": "group",
    "members@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ab8577894a63548969c5c92bb9c80c5e1%40thread.v2')/members",
    "members": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzhjMGExYTY3LTUwY2UtNDExNC1iYjZjLWRhOWM1ZGJjZjZjYQ==",
            "roles": [
                "owner"
            ],
            "displayName": "John Doe",
            "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z",
            "userId": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
            "email": "john@contoso.onmicrosoft.com",
            "tenantId": "b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzQ1OTVkMmYyLTdiMzEtNDQ2Yy04NGZkLTliNzk1ZTYzMTE0Yg==",
            "roles": [
                "owner"
            ],
            "displayName": "Test User 1",
            "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z",
            "userId": "4595d2f2-7b31-446c-84fd-9b795e63114b",
            "email": "testuser1@contoso.onmicrosoft.com",
            "tenantId": "b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzgyZmU3NzU4LTViYjMtNGYwZC1hNDNmLWU1NTVmZDM5OWM2Zg==",
            "roles": [
                "owner"
            ],
            "displayName": "Test User 2",
            "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z",
            "userId": "82fe7758-5bb3-4f0d-a43f-e555fd399c6f",
            "email": "testuser2@contoso.onmicrosoft.com",
            "tenantId": "b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzJjOGQyYjVjLTE4NDktNDA2Ni1iNTdkLWU3YTBlOWU0NGVjOA==",
            "roles": [
                "owner"
            ],
            "displayName": "Test User 3",
            "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z",
            "userId": "2c8d2b5c-1849-4066-b57d-e7a0e9e44ec8",
            "email": "testuser3@contoso.onmicrosoft.com",
            "tenantId": "b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzhlYTBlMzhiLWVmYjMtNDc1Ny05MjRhLTVmOTQwNjFjZjhjMg==",
            "roles": [
                "owner"
            ],
            "displayName": "Test User 4",
            "visibleHistoryStartDateTime": "2021-04-20T17:13:43.715Z",
            "userId": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
            "email": "testuser4@contoso.onmicrosoft.com",
            "tenantId": "b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


