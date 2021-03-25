---
title: 获取聊天中的 conversationMember
description: 检索聊天成员。
author: bhartono
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9ef01b0308df8ffd05a6337b18c4f8c16a359114
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202382"
---
# <a name="get-conversationmember-in-a-chat"></a><span data-ttu-id="40919-103">获取聊天中的 conversationMember</span><span class="sxs-lookup"><span data-stu-id="40919-103">Get conversationMember in a chat</span></span>

<span data-ttu-id="40919-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40919-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="40919-105">从[聊天](../resources/chat.md)中检索 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="40919-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="40919-106">权限</span><span class="sxs-lookup"><span data-stu-id="40919-106">Permissions</span></span>

<span data-ttu-id="40919-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40919-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40919-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="40919-109">Permission Type</span></span>|<span data-ttu-id="40919-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="40919-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="40919-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40919-111">Delegated (work or school account)</span></span>| <span data-ttu-id="40919-112">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40919-112">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="40919-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40919-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40919-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="40919-114">Not supported.</span></span>|
|<span data-ttu-id="40919-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="40919-115">Application</span></span>| <span data-ttu-id="40919-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="40919-116">Not supported.</span></span> |

> <span data-ttu-id="40919-117">**注意**：标有 \* 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="40919-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="40919-118">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="40919-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="40919-119">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="40919-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="40919-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40919-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/members/{membership-id}
GET /users/{user-id}/chats/{chat-id}/members/{membership-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40919-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="40919-121">Optional query parameters</span></span>

<span data-ttu-id="40919-122">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="40919-122">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40919-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="40919-123">Request headers</span></span>

| <span data-ttu-id="40919-124">标头</span><span class="sxs-lookup"><span data-stu-id="40919-124">Header</span></span>       | <span data-ttu-id="40919-125">值</span><span class="sxs-lookup"><span data-stu-id="40919-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="40919-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="40919-126">Authorization</span></span>  | <span data-ttu-id="40919-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="40919-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="40919-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="40919-129">Request body</span></span>

<span data-ttu-id="40919-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="40919-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40919-131">响应</span><span class="sxs-lookup"><span data-stu-id="40919-131">Response</span></span>

<span data-ttu-id="40919-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="40919-132">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

> [!NOTE]
> <span data-ttu-id="40919-133">此功能存在一些已知问题。</span><span class="sxs-lookup"><span data-stu-id="40919-133">There are some known issues with this functionality.</span></span> <span data-ttu-id="40919-134">有关详细信息，请参阅[已知问题](/graph/known-issues#missing-properties-for-chat-members)。</span><span class="sxs-lookup"><span data-stu-id="40919-134">For details, see [known issues](/graph/known-issues#missing-properties-for-chat-members).</span></span>

## <a name="example"></a><span data-ttu-id="40919-135">示例</span><span class="sxs-lookup"><span data-stu-id="40919-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="40919-136">请求</span><span class="sxs-lookup"><span data-stu-id="40919-136">Request</span></span>

<span data-ttu-id="40919-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="40919-137">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="40919-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="40919-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/141c574c-dd90-4131-b173-baf4bb0e894e
```
# <a name="c"></a>[<span data-ttu-id="40919-139">C#</span><span class="sxs-lookup"><span data-stu-id="40919-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40919-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40919-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40919-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40919-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40919-142">Java</span><span class="sxs-lookup"><span data-stu-id="40919-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-member-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="40919-143">响应</span><span class="sxs-lookup"><span data-stu-id="40919-143">Response</span></span>

<span data-ttu-id="40919-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="40919-144">Here is an example of the response.</span></span>

><span data-ttu-id="40919-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="40919-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "get_conversation_member_1",
  "@odata.type": "microsoft.graph.conversationMember"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "id": "07ad17ad-ada5-4f1f-a650-7a963886a8a7",
    "roles": [ "owner" ],
    "displayName": "Minna Pham",
    "userId": "07ad17ad-ada5-4f1f-a650-7a963886a8a7",
    "email": null,
    "tenantId": "6e5147da-6a35-4275-b3f3-fc069456b6eb",
    "visibleHistoryStartDateTime": "2019-04-18T23:51:43.255Z"
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


