---
title: 列出 hostedContents
description: 从消息中检索 chatMessageHostedContent 对象的列表。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cc6f5bcd883cc6f289444f253be29c12efcce2c0
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971389"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="bb183-103">列出 hostedContents</span><span class="sxs-lookup"><span data-stu-id="bb183-103">List hostedContents</span></span>

<span data-ttu-id="bb183-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb183-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bb183-105">从消息中检索 [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="bb183-105">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span> <span data-ttu-id="bb183-106">此 API 仅列出托管的内容对象。</span><span class="sxs-lookup"><span data-stu-id="bb183-106">This API only lists the hosted content objects.</span></span> <span data-ttu-id="bb183-107">若要获取内容字节，请参阅 [获取 chatmessage 托管内容](chatmessagehostedcontent-get.md)</span><span class="sxs-lookup"><span data-stu-id="bb183-107">To get the content bytes, see [get chatmessage hosted content](chatmessagehostedcontent-get.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="bb183-108">权限</span><span class="sxs-lookup"><span data-stu-id="bb183-108">Permissions</span></span>

### <a name="permissions-for-channel"></a><span data-ttu-id="bb183-109">频道权限</span><span class="sxs-lookup"><span data-stu-id="bb183-109">Permissions for channel</span></span>

| <span data-ttu-id="bb183-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb183-110">Permission type</span></span>                        | <span data-ttu-id="bb183-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb183-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="bb183-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb183-112">Delegated (work or school account)</span></span>| <span data-ttu-id="bb183-113">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb183-113">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="bb183-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb183-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb183-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb183-115">Not supported.</span></span>|
|<span data-ttu-id="bb183-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb183-116">Application</span></span>| <span data-ttu-id="bb183-117">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb183-117">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span> |

### <a name="permissions-for-chat"></a><span data-ttu-id="bb183-118">聊天权限</span><span class="sxs-lookup"><span data-stu-id="bb183-118">Permissions for chat</span></span>

| <span data-ttu-id="bb183-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb183-119">Permission type</span></span>                        | <span data-ttu-id="bb183-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb183-120">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="bb183-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb183-121">Delegated (work or school account)</span></span>| <span data-ttu-id="bb183-122">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb183-122">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="bb183-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb183-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb183-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb183-124">Not supported.</span></span>|
|<span data-ttu-id="bb183-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb183-125">Application</span></span>| <span data-ttu-id="bb183-126">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb183-126">Chat.Read.All, Chat.ReadWrite.All</span></span>|

> <span data-ttu-id="bb183-127">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="bb183-127">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="bb183-128">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="bb183-128">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="bb183-129">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="bb183-129">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="bb183-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb183-130">HTTP request</span></span>

<span data-ttu-id="bb183-131">**获取频道消息中的 hostedContents**</span><span class="sxs-lookup"><span data-stu-id="bb183-131">**Get hostedContents in a channel message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/hostedContents
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies/{reply-id}/hostedContents
```

<span data-ttu-id="bb183-132">**获取聊天消息中的 hostedContents**</span><span class="sxs-lookup"><span data-stu-id="bb183-132">**Get hostedContents in a chat message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/messages/{message-id}/hostedContents
GET /users/{user-id | user-principal-name}/chats/{chat-id}/messages/{message-id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bb183-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bb183-133">Optional query parameters</span></span>

<span data-ttu-id="bb183-134">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bb183-134">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb183-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb183-135">Request headers</span></span>

| <span data-ttu-id="bb183-136">名称</span><span class="sxs-lookup"><span data-stu-id="bb183-136">Name</span></span>      |<span data-ttu-id="bb183-137">说明</span><span class="sxs-lookup"><span data-stu-id="bb183-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bb183-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb183-138">Authorization</span></span> | <span data-ttu-id="bb183-139">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bb183-139">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb183-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb183-140">Request body</span></span>

<span data-ttu-id="bb183-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb183-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb183-142">响应</span><span class="sxs-lookup"><span data-stu-id="bb183-142">Response</span></span>

<span data-ttu-id="bb183-143">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bb183-143">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bb183-144">示例</span><span class="sxs-lookup"><span data-stu-id="bb183-144">Examples</span></span>

### <a name="example-1-list-hosted-content-for-a-channel-message"></a><span data-ttu-id="bb183-145">示例 1：列出频道消息的托管内容</span><span class="sxs-lookup"><span data-stu-id="bb183-145">Example 1: List hosted content for a channel message</span></span>

#### <a name="request"></a><span data-ttu-id="bb183-146">请求</span><span class="sxs-lookup"><span data-stu-id="bb183-146">Request</span></span>

<span data-ttu-id="bb183-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bb183-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bb183-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb183-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontentschannelmessage_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/hostedContents
```
# <a name="c"></a>[<span data-ttu-id="bb183-149">C#</span><span class="sxs-lookup"><span data-stu-id="bb183-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontentschannelmessage-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb183-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb183-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontentschannelmessage-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb183-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb183-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontentschannelmessage-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bb183-152">Java</span><span class="sxs-lookup"><span data-stu-id="bb183-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hostedcontentschannelmessage-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bb183-153">响应</span><span class="sxs-lookup"><span data-stu-id="bb183-153">Response</span></span>

<span data-ttu-id="bb183-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bb183-154">The following is an example of the response.</span></span>

> <span data-ttu-id="bb183-155">**注意：** `contentBytes` 和 `contentType` 始终设置为 null。</span><span class="sxs-lookup"><span data-stu-id="bb183-155">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1616963377068')/hostedContents",
    "@odata.count": 2,
    "value": [
        {
            "id": "aWQ9eF8wLXd1cy1kMS02YmI3Nzk3ZGU2MmRjODdjODA4YmQ1ZmI0OWM4NjI2ZCx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kMS02YmI3Nzk3ZGU2MmRjODdjODA4YmQ1ZmI0OWM4NjI2ZC92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        },
        {
            "id": "aWQ9eF8wLXd1cy1kNi0xMzY3OTE4MzVlODIxOGZlMmUwZWEwYTA1ODAxNjRiNCx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kNi0xMzY3OTE4MzVlODIxOGZlMmUwZWEwYTA1ODAxNjRiNC92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        }
    ]
}
```

### <a name="example-2-list-hosted-content-for-reply-to-a-channel-message"></a><span data-ttu-id="bb183-156">示例 2：列出用于回复频道消息的托管内容</span><span class="sxs-lookup"><span data-stu-id="bb183-156">Example 2: List hosted content for reply to a channel message</span></span>

#### <a name="request"></a><span data-ttu-id="bb183-157">请求</span><span class="sxs-lookup"><span data-stu-id="bb183-157">Request</span></span>

<span data-ttu-id="bb183-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bb183-158">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bb183-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb183-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontentschannelmessage_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/replies/1616963389737/hostedContents
```
# <a name="c"></a>[<span data-ttu-id="bb183-160">C#</span><span class="sxs-lookup"><span data-stu-id="bb183-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontentschannelmessage-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb183-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb183-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontentschannelmessage-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb183-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb183-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontentschannelmessage-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bb183-163">Java</span><span class="sxs-lookup"><span data-stu-id="bb183-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hostedcontentschannelmessage-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bb183-164">响应</span><span class="sxs-lookup"><span data-stu-id="bb183-164">Response</span></span>

<span data-ttu-id="bb183-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bb183-165">The following is an example of the response.</span></span>

> <span data-ttu-id="bb183-166">**注意：** `contentBytes` 和 `contentType` 始终设置为 null。</span><span class="sxs-lookup"><span data-stu-id="bb183-166">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1616963377068')/replies('1616963389737')/hostedContents",
    "@odata.count": 2,
    "value": [
        {
            "id": "aWQ9eF8wLXd1cy1kMy1hMDE3MmZiYjVkYzcxNGM4NWU5NDQwNWE5ZjNkNThmYyx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kMy1hMDE3MmZiYjVkYzcxNGM4NWU5NDQwNWE5ZjNkNThmYy92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        },
        {
            "id": "aWQ9eF8wLXd1cy1kOS03ZDlmOGVlMzk4ZGQ3YTZkMDdhMDg4OGI5ODZlNDdkYyx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS03ZDlmOGVlMzk4ZGQ3YTZkMDdhMDg4OGI5ODZlNDdkYy92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        }
    ]
}
```

### <a name="example-2--list-hosted-content-for-message-in-a-chat"></a><span data-ttu-id="bb183-167">示例 2：列出聊天中消息的托管内容</span><span class="sxs-lookup"><span data-stu-id="bb183-167">Example 2 : List hosted content for message in a chat</span></span>

#### <a name="request"></a><span data-ttu-id="bb183-168">请求</span><span class="sxs-lookup"><span data-stu-id="bb183-168">Request</span></span>

<span data-ttu-id="bb183-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bb183-169">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bb183-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb183-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontentschatmessage_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents
```
# <a name="c"></a>[<span data-ttu-id="bb183-171">C#</span><span class="sxs-lookup"><span data-stu-id="bb183-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontentschatmessage-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb183-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb183-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontentschatmessage-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb183-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb183-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontentschatmessage-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bb183-174">Java</span><span class="sxs-lookup"><span data-stu-id="bb183-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hostedcontentschatmessage-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bb183-175">响应</span><span class="sxs-lookup"><span data-stu-id="bb183-175">Response</span></span>

<span data-ttu-id="bb183-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bb183-176">The following is an example of the response.</span></span>

> <span data-ttu-id="bb183-177">**注意：** `contentBytes` 和 `contentType` 始终设置为 null。</span><span class="sxs-lookup"><span data-stu-id="bb183-177">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats('19%3A2da4c29f6d7041eca70b638b43d45437%40thread.v2')/messages('1615971548136')/hostedContents",
    "@odata.count": 1,
    "value": [
        {
            "id": "aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List hostedContents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


