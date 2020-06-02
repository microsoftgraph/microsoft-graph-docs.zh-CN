---
title: 获取 conversationMember
description: 检索聊天或频道成员。
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: efe599d9a1b4f7a928f9b0ae7dabfc845683af30
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491276"
---
# <a name="get-conversationmember"></a><span data-ttu-id="51182-103">获取 conversationMember</span><span class="sxs-lookup"><span data-stu-id="51182-103">Get conversationMember</span></span>

<span data-ttu-id="51182-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51182-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51182-105">检索[聊天](../resources/chat.md)或[频道](../resources/channel.md)中的 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="51182-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="51182-106">权限</span><span class="sxs-lookup"><span data-stu-id="51182-106">Permissions</span></span>

<span data-ttu-id="51182-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51182-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51182-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="51182-109">Permission Type</span></span>|<span data-ttu-id="51182-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="51182-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="51182-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51182-111">Delegated (work or school account)</span></span>| <span data-ttu-id="51182-112">对于**用户**或**聊天**资源： User.readbasic.all、聊天、阅读和读写</span><span class="sxs-lookup"><span data-stu-id="51182-112">For **user** or **chat** resource: Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="51182-113">对于**信道**资源： ChannelMember、ChannelMember、group. All、group. all、all、all、all、all 和 all。</span><span class="sxs-lookup"><span data-stu-id="51182-113">For **channel** resource: ChannelMember.Read.All, ChannelMember.ReadWrite, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="51182-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51182-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51182-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="51182-115">Not supported.</span></span>|
|<span data-ttu-id="51182-116">Application</span><span class="sxs-lookup"><span data-stu-id="51182-116">Application</span></span>| <span data-ttu-id="51182-117">对于**用户**或**聊天**资源： user.readbasic.all、聊天室、全部聊天。所有</span><span class="sxs-lookup"><span data-stu-id="51182-117">For **user** or **chat** resource: Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="51182-118">对于**信道**Resource： ChannelMember、ChannelMember、group、group、group、group、all、group。 all，all，all，all，all，all，all</span><span class="sxs-lookup"><span data-stu-id="51182-118">For **channel** resource: Member.Read.Group\*, ChannelMember.Read.All, ChannelMember.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="51182-119">**注意**：标记为 \* 的权限使用[特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="51182-119">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="51182-120">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="51182-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="51182-121">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="51182-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="51182-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51182-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51182-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="51182-123">Optional query parameters</span></span>

<span data-ttu-id="51182-124">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="51182-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51182-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="51182-125">Request headers</span></span>

| <span data-ttu-id="51182-126">标头</span><span class="sxs-lookup"><span data-stu-id="51182-126">Header</span></span>       | <span data-ttu-id="51182-127">值</span><span class="sxs-lookup"><span data-stu-id="51182-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="51182-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="51182-128">Authorization</span></span>  | <span data-ttu-id="51182-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="51182-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51182-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="51182-131">Request body</span></span>

<span data-ttu-id="51182-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="51182-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51182-133">响应</span><span class="sxs-lookup"><span data-stu-id="51182-133">Response</span></span>

<span data-ttu-id="51182-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="51182-134">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51182-135">示例</span><span class="sxs-lookup"><span data-stu-id="51182-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="51182-136">请求</span><span class="sxs-lookup"><span data-stu-id="51182-136">Request</span></span>

<span data-ttu-id="51182-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="51182-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="51182-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="51182-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="51182-139">C#</span><span class="sxs-lookup"><span data-stu-id="51182-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51182-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51182-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51182-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51182-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="51182-142">响应</span><span class="sxs-lookup"><span data-stu-id="51182-142">Response</span></span>

<span data-ttu-id="51182-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="51182-143">Here is an example of the response.</span></span>

><span data-ttu-id="51182-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="51182-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
