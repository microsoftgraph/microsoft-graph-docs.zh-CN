---
title: 获取 conversationMember
description: 检索聊天或频道成员。
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 05708a121b5cdedecc62c0b23678bf126cfd0662
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436501"
---
# <a name="get-conversationmember"></a><span data-ttu-id="45c3c-103">获取 conversationMember</span><span class="sxs-lookup"><span data-stu-id="45c3c-103">Get conversationMember</span></span>

<span data-ttu-id="45c3c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45c3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45c3c-105">检索[聊天](../resources/chat.md)或[频道](../resources/channel.md)中的 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="45c3c-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="45c3c-106">权限</span><span class="sxs-lookup"><span data-stu-id="45c3c-106">Permissions</span></span>

<span data-ttu-id="45c3c-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45c3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45c3c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="45c3c-109">Permission Type</span></span>|<span data-ttu-id="45c3c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45c3c-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="45c3c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45c3c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="45c3c-112">对于**用户**或**聊天**资源：</span><span class="sxs-lookup"><span data-stu-id="45c3c-112">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="45c3c-113">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45c3c-113">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="45c3c-114">对于**频道**资源：</span><span class="sxs-lookup"><span data-stu-id="45c3c-114">For **channel** resource:</span></span><br/><span data-ttu-id="45c3c-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45c3c-115">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="45c3c-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45c3c-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45c3c-117">不支持</span><span class="sxs-lookup"><span data-stu-id="45c3c-117">Not supported</span></span>|
|<span data-ttu-id="45c3c-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="45c3c-118">Application</span></span>| <span data-ttu-id="45c3c-119">对于**用户**或**聊天**资源：</span><span class="sxs-lookup"><span data-stu-id="45c3c-119">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="45c3c-120">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45c3c-120">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="45c3c-121">对于**频道**资源：</span><span class="sxs-lookup"><span data-stu-id="45c3c-121">For **channel** resource:</span></span><br/><span data-ttu-id="45c3c-122">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45c3c-122">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="45c3c-123">在调用具有应用程序权限的此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="45c3c-123">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="45c3c-124">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="45c3c-124">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="45c3c-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45c3c-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45c3c-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="45c3c-126">Optional query parameters</span></span>

<span data-ttu-id="45c3c-127">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="45c3c-127">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45c3c-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="45c3c-128">Request headers</span></span>

| <span data-ttu-id="45c3c-129">标头</span><span class="sxs-lookup"><span data-stu-id="45c3c-129">Header</span></span>       | <span data-ttu-id="45c3c-130">值</span><span class="sxs-lookup"><span data-stu-id="45c3c-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="45c3c-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="45c3c-131">Authorization</span></span>  | <span data-ttu-id="45c3c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="45c3c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="45c3c-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="45c3c-134">Request body</span></span>

<span data-ttu-id="45c3c-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="45c3c-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45c3c-136">响应</span><span class="sxs-lookup"><span data-stu-id="45c3c-136">Response</span></span>

<span data-ttu-id="45c3c-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="45c3c-137">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45c3c-138">示例</span><span class="sxs-lookup"><span data-stu-id="45c3c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="45c3c-139">请求</span><span class="sxs-lookup"><span data-stu-id="45c3c-139">Request</span></span>

<span data-ttu-id="45c3c-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45c3c-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="45c3c-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="45c3c-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="45c3c-142">C#</span><span class="sxs-lookup"><span data-stu-id="45c3c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45c3c-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45c3c-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45c3c-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45c3c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="45c3c-145">响应</span><span class="sxs-lookup"><span data-stu-id="45c3c-145">Response</span></span>

<span data-ttu-id="45c3c-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="45c3c-146">Here is an example of the response.</span></span>

><span data-ttu-id="45c3c-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="45c3c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
