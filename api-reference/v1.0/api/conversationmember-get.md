---
title: 获取 conversationMember
description: 检索聊天或频道成员。
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5b2f03bfc9375b38a4901d7f9a24e315420066ec
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941247"
---
# <a name="get-conversationmember"></a><span data-ttu-id="cd887-103">获取 conversationMember</span><span class="sxs-lookup"><span data-stu-id="cd887-103">Get conversationMember</span></span>

<span data-ttu-id="cd887-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd887-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd887-105">检索[聊天](../resources/chatmessage.md)或[频道](../resources/channel.md)中的 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="cd887-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chatmessage.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cd887-106">权限</span><span class="sxs-lookup"><span data-stu-id="cd887-106">Permissions</span></span>

<span data-ttu-id="cd887-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd887-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd887-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd887-109">Permission Type</span></span>|<span data-ttu-id="cd887-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cd887-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="cd887-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd887-111">Delegated (work or school account)</span></span>| <span data-ttu-id="cd887-112">对于 **用户** 或 **聊天** 资源：Chat.ReadBasic、Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd887-112">For **user** or **chat** resource: Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="cd887-113">对于 **频道** 资源：ChannelMember.Read.All、ChannelMember.ReadWrite、Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd887-113">For **channel** resource: ChannelMember.Read.All, ChannelMember.ReadWrite</span></span> |
|<span data-ttu-id="cd887-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd887-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd887-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd887-115">Not supported.</span></span>|
|<span data-ttu-id="cd887-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd887-116">Application</span></span>| <span data-ttu-id="cd887-117">对于 **用户** 或 **聊天** 资源：不支持。</span><span class="sxs-lookup"><span data-stu-id="cd887-117">For **user** or **chat** resource: Not supported.</span></span><br/><br/><span data-ttu-id="cd887-118">对于 **频道** 资源：TeamMember.Read.Group\*、ChannelMember.Read.All、ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd887-118">For **channel** resource: TeamMember.Read.Group\*, ChannelMember.Read.All, ChannelMember.ReadWrite.All</span></span> |

> <span data-ttu-id="cd887-119">**注意**：标有 \* 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="cd887-119">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>


## <a name="http-request"></a><span data-ttu-id="cd887-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd887-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cd887-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cd887-121">Optional query parameters</span></span>

<span data-ttu-id="cd887-122">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cd887-122">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd887-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd887-123">Request headers</span></span>

| <span data-ttu-id="cd887-124">标头</span><span class="sxs-lookup"><span data-stu-id="cd887-124">Header</span></span>       | <span data-ttu-id="cd887-125">值</span><span class="sxs-lookup"><span data-stu-id="cd887-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cd887-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd887-126">Authorization</span></span>  | <span data-ttu-id="cd887-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cd887-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cd887-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd887-129">Request body</span></span>

<span data-ttu-id="cd887-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cd887-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd887-131">响应</span><span class="sxs-lookup"><span data-stu-id="cd887-131">Response</span></span>

<span data-ttu-id="cd887-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cd887-132">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd887-133">示例</span><span class="sxs-lookup"><span data-stu-id="cd887-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd887-134">请求</span><span class="sxs-lookup"><span data-stu-id="cd887-134">Request</span></span>

<span data-ttu-id="cd887-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cd887-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cd887-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd887-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/V1.0/chats/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="cd887-137">C#</span><span class="sxs-lookup"><span data-stu-id="cd887-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd887-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd887-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd887-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd887-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd887-140">Java</span><span class="sxs-lookup"><span data-stu-id="cd887-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cd887-141">响应</span><span class="sxs-lookup"><span data-stu-id="cd887-141">Response</span></span>

<span data-ttu-id="cd887-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cd887-142">Here is an example of the response.</span></span>

><span data-ttu-id="cd887-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cd887-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!--
{
  "blockType": "response",
  "truncated": true,
  "name": "get_conversation_member_2",
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
