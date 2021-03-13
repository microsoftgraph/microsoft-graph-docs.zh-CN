---
title: 列出聊天
description: 检索用户的聊天列表。
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0416a123b0694b3b2ffcd6756334fcf891da0b82
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775764"
---
# <a name="list-chats"></a><span data-ttu-id="656a2-103">列出聊天</span><span class="sxs-lookup"><span data-stu-id="656a2-103">List chats</span></span>

<span data-ttu-id="656a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="656a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="656a2-105">检索用户 [属于](../resources/chat.md) 的聊天列表。</span><span class="sxs-lookup"><span data-stu-id="656a2-105">Retrieve the list of [chats](../resources/chat.md) that the user is part of.</span></span>

## <a name="permissions"></a><span data-ttu-id="656a2-106">权限</span><span class="sxs-lookup"><span data-stu-id="656a2-106">Permissions</span></span>

<span data-ttu-id="656a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="656a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="656a2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="656a2-109">Permission type</span></span>      | <span data-ttu-id="656a2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="656a2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="656a2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="656a2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="656a2-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="656a2-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="656a2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="656a2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="656a2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="656a2-114">Not supported.</span></span>    |
|<span data-ttu-id="656a2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="656a2-115">Application</span></span> | <span data-ttu-id="656a2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="656a2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="656a2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="656a2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats
GET /users/{user-id}/chats
GET /chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="656a2-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="656a2-118">Optional query parameters</span></span>

<span data-ttu-id="656a2-119">此方法仅 (`$expand` **members** 属性和 `$filter` [OData](/graph/query-parameters)) 参数的自定义响应。</span><span class="sxs-lookup"><span data-stu-id="656a2-119">This method supports the `$expand` (only for the **members** property) and `$filter` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="656a2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="656a2-120">Request headers</span></span>

| <span data-ttu-id="656a2-121">标头</span><span class="sxs-lookup"><span data-stu-id="656a2-121">Header</span></span>       | <span data-ttu-id="656a2-122">值</span><span class="sxs-lookup"><span data-stu-id="656a2-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="656a2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="656a2-123">Authorization</span></span>  | <span data-ttu-id="656a2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="656a2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="656a2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="656a2-126">Request body</span></span>

<span data-ttu-id="656a2-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="656a2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="656a2-128">响应</span><span class="sxs-lookup"><span data-stu-id="656a2-128">Response</span></span>

<span data-ttu-id="656a2-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chat](../resources/chat.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="656a2-129">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="656a2-130">示例</span><span class="sxs-lookup"><span data-stu-id="656a2-130">Example</span></span>

### <a name="example-1-list-all-the-chats"></a><span data-ttu-id="656a2-131">示例 1：列出所有聊天</span><span class="sxs-lookup"><span data-stu-id="656a2-131">Example 1: List all the chats</span></span>

#### <a name="request"></a><span data-ttu-id="656a2-132">请求</span><span class="sxs-lookup"><span data-stu-id="656a2-132">Request</span></span>

<span data-ttu-id="656a2-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="656a2-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="656a2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="656a2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_chats"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats
```
# <a name="c"></a>[<span data-ttu-id="656a2-135">C#</span><span class="sxs-lookup"><span data-stu-id="656a2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-chats-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="656a2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="656a2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-chats-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="656a2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="656a2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-chats-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="656a2-138">Java</span><span class="sxs-lookup"><span data-stu-id="656a2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-chats-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="656a2-139">响应</span><span class="sxs-lookup"><span data-stu-id="656a2-139">Response</span></span>

<span data-ttu-id="656a2-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="656a2-140">Here is an example of the response.</span></span> 

><span data-ttu-id="656a2-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="656a2-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats",
    "@odata.count": 3,
    "value": [
        {
            "id": "19:meeting_MjdhNjM4YzUtYzExZi00OTFkLTkzZTAtNTVlNmZmMDhkNGU2@thread.v2",
            "topic": "Meeting chat sample",
            "createdDateTime": "2020-12-08T23:53:05.801Z",
            "lastUpdatedDateTime": "2020-12-08T23:58:32.511Z",
            "chatType": "meeting"
        },
        {
            "id": "19:561082c0f3f847a58069deb8eb300807@thread.v2",
            "topic": "Group chat sample",
            "createdDateTime": "2020-12-03T19:41:07.054Z",
            "lastUpdatedDateTime": "2020-12-08T23:53:11.012Z",
            "chatType": "group"
        },
        {
            "id": "19:d74fc2ed-cb0e-4288-a219-b5c71abaf2aa_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2020-12-04T23:10:28.51Z",
            "lastUpdatedDateTime": "2020-12-04T23:10:36.925Z",
            "chatType": "oneOnOne"
        }
    ]
}
```

### <a name="example-2-list-all-the-chats-along-with-the-members-of-each-chat"></a><span data-ttu-id="656a2-142">示例 2：列出所有聊天以及每个聊天的成员</span><span class="sxs-lookup"><span data-stu-id="656a2-142">Example 2: List all the chats along with the members of each chat</span></span>
#### <a name="request"></a><span data-ttu-id="656a2-143">请求</span><span class="sxs-lookup"><span data-stu-id="656a2-143">Request</span></span>

<span data-ttu-id="656a2-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="656a2-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="656a2-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="656a2-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_chats_expand_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats?$expand=members
```
# <a name="c"></a>[<span data-ttu-id="656a2-146">C#</span><span class="sxs-lookup"><span data-stu-id="656a2-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-chats-expand-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="656a2-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="656a2-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-chats-expand-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="656a2-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="656a2-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-chats-expand-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="656a2-149">Java</span><span class="sxs-lookup"><span data-stu-id="656a2-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-chats-expand-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="656a2-150">响应</span><span class="sxs-lookup"><span data-stu-id="656a2-150">Response</span></span>

<span data-ttu-id="656a2-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="656a2-151">Here is an example of the response.</span></span> 

> [!NOTE]
> <span data-ttu-id="656a2-152">服务器返回的成员 ID 必须作为不透明的字符串处理。</span><span class="sxs-lookup"><span data-stu-id="656a2-152">The membership IDs returned by the server must be treated as opaque strings.</span></span> <span data-ttu-id="656a2-153">客户端不应尝试对这些资源 ID 进行分析或做出任何假设。</span><span class="sxs-lookup"><span data-stu-id="656a2-153">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="656a2-154">成员身份结果可以映射到不同租户中的用户，如响应中将来所指示。</span><span class="sxs-lookup"><span data-stu-id="656a2-154">The membership results can map to users from different tenants, as indicated in the response, in the future.</span></span> <span data-ttu-id="656a2-155">客户端不应假定所有成员都仅来自当前租户。</span><span class="sxs-lookup"><span data-stu-id="656a2-155">The client should not assume that all members are from the current tenant only.</span></span>

><span data-ttu-id="656a2-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="656a2-156">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats(members())",
    "@odata.count": 3,
    "value": [
        {
            "id": "19:meeting_MjdhNjM4YzUtYzExZi00OTFkLTkzZTAtNTVlNmZmMDhkNGU2@thread.v2",
            "topic": "Meeting chat sample",
            "createdDateTime": "2020-12-08T23:53:05.801Z",
            "lastUpdatedDateTime": "2020-12-08T23:58:32.511Z",
            "chatType": "meeting",
            "members@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ameeting_MjdhNjM4YzUtYzExZi00OTFkLTkzZTAtNTVlNmZmMDhkNGU2%40thread.v2')/members",
            "members": [
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Tony Stark",
                    "userId": "4595d2f2-7b31-446c-84fd-9b795e63114b",
                    "email": "starkt@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMz6Jk45=",
                    "roles": [],
                    "displayName": "Peter Parker",
                    "userId": "d74fc2ed-cb0e-4288-a219-b5c71abaf2aa",
                    "email": "parkerp@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJ989kMTQ=",
                    "roles": [],
                    "displayName": "Nick Fury",
                    "userId": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
                    "email": "furyn@teamsgraph.onmicrosoft.com"
                }
            ]
        },
        {
            "id": "19:561082c0f3f847a58069deb8eb300807@thread.v2",
            "topic": "Group chat sample",
            "createdDateTime": "2020-12-03T19:41:07.054Z",
            "lastUpdatedDateTime": "2020-12-08T23:53:11.012Z",
            "chatType": "group",
            "members@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3A561082c0f3f847a58069deb8eb300807%40thread.v2')/members",
            "members": [
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Tony Stark",
                    "userId": "4595d2f2-7b31-446c-84fd-9b795e63114b",
                    "email": "starkt@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM312ftMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Bruce Banner",
                    "userId": "48bf9d52-dca7-4a5f-8398-37b95cc7bd83",
                    "email": "bannerb@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWai3MTetN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "TChalla",
                    "userId": "9efb1aea-4f83-4673-bdcd-d3f3c7be28c2",
                    "email": "tchalla@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwamii00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Thor Odinson",
                    "userId": "976f4b31-fd01-4e0b-9178-29cc40c14438",
                    "email": "odinsont@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWopiLWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Steve Rogers",
                    "userId": "976f4b31-fd01-4e0b-9178-29cc40c14438",
                    "email": "rogerss@teamsgraph.onmicrosoft.com"
                }
            ]
        },
        {
            "id": "19:d74fc2ed-cb0e-4288-a219-b5c71abaf2aa_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2020-12-04T23:10:28.51Z",
            "lastUpdatedDateTime": "2020-12-04T23:10:36.925Z",
            "chatType": "oneOnOne",
            "members@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ad74fc2ed-cb0e-4288-a219-b5c71abaf2aa_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca%40unq.gbl.spaces')/members",
            "members": [
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJ989kMTQ=",
                    "roles": [],
                    "displayName": "Nick Fury",
                    "userId": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
                    "email": "furyn@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMz6Jk45=",
                    "roles": [],
                    "displayName": "Peter Parker",
                    "userId": "d74fc2ed-cb0e-4288-a219-b5c71abaf2aa",
                    "email": "parkerp@teamsgraph.onmicrosoft.com"
                }
            ]
        }
    ]
}
```

### <a name="example-3-list-all-the-chats-that-have-a-member-with-a-specific-display-name"></a><span data-ttu-id="656a2-157">示例 3：列出成员具有特定名称的所有显示名称</span><span class="sxs-lookup"><span data-stu-id="656a2-157">Example 3: List all the chats that have a member with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="656a2-158">请求</span><span class="sxs-lookup"><span data-stu-id="656a2-158">Request</span></span>

<span data-ttu-id="656a2-159">下面是一个请求示例，该请求将基于特定成员的信息筛选所有显示名称。</span><span class="sxs-lookup"><span data-stu-id="656a2-159">Here is an example of a request that will filter all the chats based on a specific member's display name.</span></span>

# <a name="http"></a>[<span data-ttu-id="656a2-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="656a2-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_chats_expand_members_and_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats?$expand=members&$filter=members/any(o: o/displayname eq 'Peter Parker')
```
# <a name="c"></a>[<span data-ttu-id="656a2-161">C#</span><span class="sxs-lookup"><span data-stu-id="656a2-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-chats-expand-members-and-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="656a2-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="656a2-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-chats-expand-members-and-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="656a2-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="656a2-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-chats-expand-members-and-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="656a2-164">Java</span><span class="sxs-lookup"><span data-stu-id="656a2-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-chats-expand-members-and-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="656a2-165">响应</span><span class="sxs-lookup"><span data-stu-id="656a2-165">Response</span></span>

<span data-ttu-id="656a2-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="656a2-166">Here is an example of the response.</span></span> 

> [!NOTE]
> <span data-ttu-id="656a2-167">必须将由服务器返回的会员资格 ID 视为不透明字符串。</span><span class="sxs-lookup"><span data-stu-id="656a2-167">The membership ID returned by server must be treated as opaque strings.</span></span> <span data-ttu-id="656a2-168">客户端不应尝试对这些资源 ID 进行分析或做出任何假设。</span><span class="sxs-lookup"><span data-stu-id="656a2-168">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="656a2-169">成员资格结果将来可能会映射到来自不同租户的用户，如响应中所示。</span><span class="sxs-lookup"><span data-stu-id="656a2-169">The membership results could map to users from different tenants, as indicated in the response, in the future.</span></span> <span data-ttu-id="656a2-170">客户端不应假定所有成员都仅来自当前租户。</span><span class="sxs-lookup"><span data-stu-id="656a2-170">The client should not assume that all members are from the current tenant only.</span></span>

><span data-ttu-id="656a2-171">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="656a2-171">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats(members())",
    "@odata.count": 2,
    "value": [
        {
            "id": "19:meeting_MjdhNjM4YzUtYzExZi00OTFkLTkzZTAtNTVlNmZmMDhkNGU2@thread.v2",
            "topic": "Meeting chat sample",
            "createdDateTime": "2020-12-08T23:53:05.801Z",
            "lastUpdatedDateTime": "2020-12-08T23:58:32.511Z",
            "chatType": "meeting",
            "members@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ameeting_MjdhNjM4YzUtYzExZi00OTFkLTkzZTAtNTVlNmZmMDhkNGU2%40thread.v2')/members",
            "members": [
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Tony Stark",
                    "userId": "4595d2f2-7b31-446c-84fd-9b795e63114b",
                    "email": "starkt@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMz6Jk45=",
                    "roles": [],
                    "displayName": "Peter Parker",
                    "userId": "d74fc2ed-cb0e-4288-a219-b5c71abaf2aa",
                    "email": "parkerp@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJ989kMTQ=",
                    "roles": [],
                    "displayName": "Nick Fury",
                    "userId": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
                    "email": "furyn@teamsgraph.onmicrosoft.com"
                }
            ]
        },
        {
            "id": "19:d74fc2ed-cb0e-4288-a219-b5c71abaf2aa_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2020-12-04T23:10:28.51Z",
            "lastUpdatedDateTime": "2020-12-04T23:10:36.925Z",
            "chatType": "oneOnOne",
            "members@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ad74fc2ed-cb0e-4288-a219-b5c71abaf2aa_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca%40unq.gbl.spaces')/members",
            "members": [
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJ989kMTQ=",
                    "roles": [],
                    "displayName": "Nick Fury",
                    "userId": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
                    "email": "furyn@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMz6Jk45=",
                    "roles": [],
                    "displayName": "Peter Parker",
                    "userId": "d74fc2ed-cb0e-4288-a219-b5c71abaf2aa",
                    "email": "parkerp@teamsgraph.onmicrosoft.com"
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List chats",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
