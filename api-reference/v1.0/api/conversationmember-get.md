---
title: 获取 conversationMember
description: 检索聊天或频道成员。
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 054bbb8d69d843fd26644ac658bd2b7553600a7a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963867"
---
# <a name="get-conversationmember"></a><span data-ttu-id="505c8-103">获取 conversationMember</span><span class="sxs-lookup"><span data-stu-id="505c8-103">Get conversationMember</span></span>

<span data-ttu-id="505c8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="505c8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="505c8-105">检索[聊天](../resources/chatmessage.md)或[频道](../resources/channel.md)中的 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="505c8-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chatmessage.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="505c8-106">权限</span><span class="sxs-lookup"><span data-stu-id="505c8-106">Permissions</span></span>

<span data-ttu-id="505c8-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="505c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="505c8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="505c8-109">Permission Type</span></span>|<span data-ttu-id="505c8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="505c8-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="505c8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="505c8-111">Delegated (work or school account)</span></span>| <span data-ttu-id="505c8-112">对于 **用户** 或 **聊天** 资源：Chat.ReadBasic、Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="505c8-112">For **user** or **chat** resource: Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="505c8-113">对于 **频道** 资源：ChannelMember.Read.All、ChannelMember.ReadWrite、Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="505c8-113">For **channel** resource: ChannelMember.Read.All, ChannelMember.ReadWrite</span></span> |
|<span data-ttu-id="505c8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="505c8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="505c8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="505c8-115">Not supported.</span></span>|
|<span data-ttu-id="505c8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="505c8-116">Application</span></span>| <span data-ttu-id="505c8-117">对于 **用户** 或 **聊天** 资源：不支持。</span><span class="sxs-lookup"><span data-stu-id="505c8-117">For **user** or **chat** resource: Not supported.</span></span><br/><br/><span data-ttu-id="505c8-118">对于 **频道** 资源：TeamMember.Read.Group\*、ChannelMember.Read.All、ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="505c8-118">For **channel** resource: TeamMember.Read.Group\*, ChannelMember.Read.All, ChannelMember.ReadWrite.All</span></span> |

> <span data-ttu-id="505c8-119">**注意**：标有 \* 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="505c8-119">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="505c8-120">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="505c8-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="505c8-121">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="505c8-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="505c8-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="505c8-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="505c8-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="505c8-123">Optional query parameters</span></span>

<span data-ttu-id="505c8-124">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="505c8-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="505c8-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="505c8-125">Request headers</span></span>

| <span data-ttu-id="505c8-126">标头</span><span class="sxs-lookup"><span data-stu-id="505c8-126">Header</span></span>       | <span data-ttu-id="505c8-127">值</span><span class="sxs-lookup"><span data-stu-id="505c8-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="505c8-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="505c8-128">Authorization</span></span>  | <span data-ttu-id="505c8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="505c8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="505c8-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="505c8-131">Request body</span></span>

<span data-ttu-id="505c8-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="505c8-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="505c8-133">响应</span><span class="sxs-lookup"><span data-stu-id="505c8-133">Response</span></span>

<span data-ttu-id="505c8-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="505c8-134">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="505c8-135">示例</span><span class="sxs-lookup"><span data-stu-id="505c8-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="505c8-136">请求</span><span class="sxs-lookup"><span data-stu-id="505c8-136">Request</span></span>

<span data-ttu-id="505c8-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="505c8-137">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="505c8-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="505c8-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/V1.0/chats/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="505c8-139">C#</span><span class="sxs-lookup"><span data-stu-id="505c8-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="505c8-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="505c8-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="505c8-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="505c8-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="505c8-142">Java</span><span class="sxs-lookup"><span data-stu-id="505c8-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="505c8-143">响应</span><span class="sxs-lookup"><span data-stu-id="505c8-143">Response</span></span>

<span data-ttu-id="505c8-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="505c8-144">Here is an example of the response.</span></span>

><span data-ttu-id="505c8-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="505c8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
