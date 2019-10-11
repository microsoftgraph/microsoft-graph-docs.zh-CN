---
title: 获取 conversationMember
description: 检索聊天或频道成员。
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bd1d7cc150ade0a9c50083d9b9833ae682599b95
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439811"
---
# <a name="get-conversationmember"></a><span data-ttu-id="0a2c5-103">获取 conversationMember</span><span class="sxs-lookup"><span data-stu-id="0a2c5-103">Get conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a2c5-104">检索[聊天](../resources/chat.md)或[频道](../resources/channel.md)中的 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="0a2c5-104">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0a2c5-105">权限</span><span class="sxs-lookup"><span data-stu-id="0a2c5-105">Permissions</span></span>

<span data-ttu-id="0a2c5-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a2c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a2c5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a2c5-108">Permission Type</span></span>|<span data-ttu-id="0a2c5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a2c5-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="0a2c5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a2c5-110">Delegated (work or school account)</span></span>|<span data-ttu-id="0a2c5-111">对于**用户**或**聊天**资源：</span><span class="sxs-lookup"><span data-stu-id="0a2c5-111">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="0a2c5-112">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a2c5-112">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="0a2c5-113">对于**频道**资源：</span><span class="sxs-lookup"><span data-stu-id="0a2c5-113">For **channel** resource:</span></span><br/><span data-ttu-id="0a2c5-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a2c5-114">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="0a2c5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a2c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a2c5-116">不支持</span><span class="sxs-lookup"><span data-stu-id="0a2c5-116">Not supported</span></span>|
|<span data-ttu-id="0a2c5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a2c5-117">Application</span></span>| <span data-ttu-id="0a2c5-118">对于**用户**或**聊天**资源：</span><span class="sxs-lookup"><span data-stu-id="0a2c5-118">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="0a2c5-119">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a2c5-119">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="0a2c5-120">对于**频道**资源：</span><span class="sxs-lookup"><span data-stu-id="0a2c5-120">For **channel** resource:</span></span><br/><span data-ttu-id="0a2c5-121">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a2c5-121">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="0a2c5-122">在调用具有应用程序权限的此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="0a2c5-122">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="0a2c5-123">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="0a2c5-123">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="0a2c5-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a2c5-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0a2c5-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0a2c5-125">Optional query parameters</span></span>

<span data-ttu-id="0a2c5-126">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0a2c5-126">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a2c5-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a2c5-127">Request headers</span></span>

| <span data-ttu-id="0a2c5-128">标头</span><span class="sxs-lookup"><span data-stu-id="0a2c5-128">Header</span></span>       | <span data-ttu-id="0a2c5-129">值</span><span class="sxs-lookup"><span data-stu-id="0a2c5-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0a2c5-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a2c5-130">Authorization</span></span>  | <span data-ttu-id="0a2c5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0a2c5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0a2c5-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a2c5-133">Request body</span></span>

<span data-ttu-id="0a2c5-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0a2c5-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a2c5-135">响应</span><span class="sxs-lookup"><span data-stu-id="0a2c5-135">Response</span></span>

<span data-ttu-id="0a2c5-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0a2c5-136">If successful, this method returns a `200 OK` response code and a [channel](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a2c5-137">示例</span><span class="sxs-lookup"><span data-stu-id="0a2c5-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a2c5-138">请求</span><span class="sxs-lookup"><span data-stu-id="0a2c5-138">Request</span></span>

<span data-ttu-id="0a2c5-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0a2c5-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0a2c5-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a2c5-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0a2c5-141">C#</span><span class="sxs-lookup"><span data-stu-id="0a2c5-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a2c5-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a2c5-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0a2c5-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a2c5-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0a2c5-144">响应</span><span class="sxs-lookup"><span data-stu-id="0a2c5-144">Response</span></span>

<span data-ttu-id="0a2c5-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0a2c5-145">Here is an example of the response.</span></span>

><span data-ttu-id="0a2c5-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0a2c5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
