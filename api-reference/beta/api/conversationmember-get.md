---
title: 获取 conversationMember
description: 检索聊天或频道成员。
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cfb6649709cce80b7936ddab80f18bf6f3493924
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288527"
---
# <a name="get-conversationmember"></a><span data-ttu-id="35434-103">获取 conversationMember</span><span class="sxs-lookup"><span data-stu-id="35434-103">Get conversationMember</span></span>

<span data-ttu-id="35434-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35434-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35434-105">检索[聊天](../resources/chat.md)或[频道](../resources/channel.md)中的 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="35434-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="35434-106">权限</span><span class="sxs-lookup"><span data-stu-id="35434-106">Permissions</span></span>

<span data-ttu-id="35434-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35434-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35434-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="35434-109">Permission Type</span></span>|<span data-ttu-id="35434-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="35434-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="35434-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35434-111">Delegated (work or school account)</span></span>| <span data-ttu-id="35434-112">对于**用户**或**聊天**资源： User.readbasic.all、聊天、阅读和读写</span><span class="sxs-lookup"><span data-stu-id="35434-112">For **user** or **chat** resource: Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="35434-113">对于**信道**资源： ChannelMember、ChannelMember、group. All、group. all、all、all、all、all 和 all。</span><span class="sxs-lookup"><span data-stu-id="35434-113">For **channel** resource: ChannelMember.Read.All, ChannelMember.ReadWrite, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="35434-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35434-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35434-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="35434-115">Not supported.</span></span>|
|<span data-ttu-id="35434-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="35434-116">Application</span></span>| <span data-ttu-id="35434-117">对于**用户**或**聊天**资源： user.readbasic.all、聊天室、全部聊天。所有</span><span class="sxs-lookup"><span data-stu-id="35434-117">For **user** or **chat** resource: Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="35434-118">对于**信道**Resource： Member. ChannelMember （[RSC](https://aka.ms/teams-rsc)）、ChannelMember、、group、Group。 all、group。 all、all、member。 all，all，all，all</span><span class="sxs-lookup"><span data-stu-id="35434-118">For **channel** resource: Member.Read.Group ([RSC](https://aka.ms/teams-rsc)), ChannelMember.Read.All, ChannelMember.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="35434-119">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="35434-119">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="35434-120">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="35434-120">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="35434-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35434-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="35434-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="35434-122">Optional query parameters</span></span>

<span data-ttu-id="35434-123">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="35434-123">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35434-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="35434-124">Request headers</span></span>

| <span data-ttu-id="35434-125">标头</span><span class="sxs-lookup"><span data-stu-id="35434-125">Header</span></span>       | <span data-ttu-id="35434-126">值</span><span class="sxs-lookup"><span data-stu-id="35434-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="35434-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="35434-127">Authorization</span></span>  | <span data-ttu-id="35434-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="35434-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="35434-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="35434-130">Request body</span></span>

<span data-ttu-id="35434-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="35434-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35434-132">响应</span><span class="sxs-lookup"><span data-stu-id="35434-132">Response</span></span>

<span data-ttu-id="35434-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="35434-133">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35434-134">示例</span><span class="sxs-lookup"><span data-stu-id="35434-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="35434-135">请求</span><span class="sxs-lookup"><span data-stu-id="35434-135">Request</span></span>

<span data-ttu-id="35434-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="35434-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="35434-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="35434-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="35434-138">C#</span><span class="sxs-lookup"><span data-stu-id="35434-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35434-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35434-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35434-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35434-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="35434-141">响应</span><span class="sxs-lookup"><span data-stu-id="35434-141">Response</span></span>

<span data-ttu-id="35434-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="35434-142">Here is an example of the response.</span></span>

><span data-ttu-id="35434-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="35434-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "id": "id-value",
  "displayName": "display-name-value"
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
