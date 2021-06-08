---
title: 获取 chatMessageHostedContent
description: 检索 chatMessageHostedContent 对象的属性和关系。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5a2729a3c78c1931afc57b308418a86ea06c446c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786181"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="ed66a-103">获取 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="ed66a-103">Get chatMessageHostedContent</span></span>

<span data-ttu-id="ed66a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed66a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed66a-105">检索 [chatMessageHostedContent 对象的属性和](../resources/chatmessagehostedcontent.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="ed66a-105">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed66a-106">权限</span><span class="sxs-lookup"><span data-stu-id="ed66a-106">Permissions</span></span>

<span data-ttu-id="ed66a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed66a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-for-channel"></a><span data-ttu-id="ed66a-109">频道权限</span><span class="sxs-lookup"><span data-stu-id="ed66a-109">Permissions for channel</span></span>

| <span data-ttu-id="ed66a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed66a-110">Permission type</span></span>                        | <span data-ttu-id="ed66a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed66a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="ed66a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed66a-112">Delegated (work or school account)</span></span>| <span data-ttu-id="ed66a-113">ChannelMessage.Read.All、Group.Read.All、Group.Read.WriteAll</span><span class="sxs-lookup"><span data-stu-id="ed66a-113">ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="ed66a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed66a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed66a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed66a-115">Not supported.</span></span>|
|<span data-ttu-id="ed66a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed66a-116">Application</span></span>| <span data-ttu-id="ed66a-117">ChannelMessage.Read.Group、ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed66a-117">ChannelMessage.Read.Group, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

### <a name="permissions-for-chat"></a><span data-ttu-id="ed66a-118">聊天权限</span><span class="sxs-lookup"><span data-stu-id="ed66a-118">Permissions for chat</span></span>

| <span data-ttu-id="ed66a-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed66a-119">Permission type</span></span>                        | <span data-ttu-id="ed66a-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed66a-120">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="ed66a-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed66a-121">Delegated (work or school account)</span></span>| <span data-ttu-id="ed66a-122">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed66a-122">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="ed66a-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed66a-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed66a-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed66a-124">Not supported.</span></span>|
|<span data-ttu-id="ed66a-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed66a-125">Application</span></span>| <span data-ttu-id="ed66a-126">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed66a-126">Chat.Read.All, Chat.ReadWrite.All</span></span>|

> <span data-ttu-id="ed66a-127">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="ed66a-127">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="ed66a-128">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="ed66a-128">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="ed66a-129">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="ed66a-129">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="ed66a-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed66a-130">HTTP request</span></span>

<span data-ttu-id="ed66a-131">**获取频道消息中的托管内容**</span><span class="sxs-lookup"><span data-stu-id="ed66a-131">**Get hosted content in a channel message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/hostedContents/{hosted-content-id}
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies/{reply-id}/hostedContents/{hosted-content-id}
```

<span data-ttu-id="ed66a-132">**获取聊天消息中的托管内容**</span><span class="sxs-lookup"><span data-stu-id="ed66a-132">**Get hosted content in a chat message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/messages/{message-id}/hostedContents/{hosted-content-id}
GET /users/{user-id | user-principal-name}/chats/{chat-id}/messages/{message-id}/hostedContents/{hosted-content-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed66a-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ed66a-133">Optional query parameters</span></span>

<span data-ttu-id="ed66a-134">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ed66a-134">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed66a-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed66a-135">Request headers</span></span>

| <span data-ttu-id="ed66a-136">名称</span><span class="sxs-lookup"><span data-stu-id="ed66a-136">Name</span></span>      |<span data-ttu-id="ed66a-137">说明</span><span class="sxs-lookup"><span data-stu-id="ed66a-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ed66a-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed66a-138">Authorization</span></span> | <span data-ttu-id="ed66a-139">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ed66a-139">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed66a-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed66a-140">Request body</span></span>

<span data-ttu-id="ed66a-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ed66a-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed66a-142">响应</span><span class="sxs-lookup"><span data-stu-id="ed66a-142">Response</span></span>

<span data-ttu-id="ed66a-143">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ed66a-143">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ed66a-144">示例</span><span class="sxs-lookup"><span data-stu-id="ed66a-144">Examples</span></span>

### <a name="example-1-get-hosted-content-for-message-in-a-chat"></a><span data-ttu-id="ed66a-145">示例 1：获取聊天中消息的托管内容</span><span class="sxs-lookup"><span data-stu-id="ed66a-145">Example 1: Get hosted content for message in a chat</span></span>

#### <a name="request"></a><span data-ttu-id="ed66a-146">请求</span><span class="sxs-lookup"><span data-stu-id="ed66a-146">Request</span></span>

<span data-ttu-id="ed66a-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ed66a-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ed66a-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed66a-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontentchatmessage_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents/aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv
```
# <a name="c"></a>[<span data-ttu-id="ed66a-149">C#</span><span class="sxs-lookup"><span data-stu-id="ed66a-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontentchatmessage-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed66a-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed66a-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontentchatmessage-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed66a-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed66a-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontentchatmessage-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed66a-152">Java</span><span class="sxs-lookup"><span data-stu-id="ed66a-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hostedcontentchatmessage-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ed66a-153">响应</span><span class="sxs-lookup"><span data-stu-id="ed66a-153">Response</span></span>

<span data-ttu-id="ed66a-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ed66a-154">The following is an example of the response.</span></span>

> <span data-ttu-id="ed66a-155">**注意：** `contentBytes` 和 `contentType` 始终设置为 null。</span><span class="sxs-lookup"><span data-stu-id="ed66a-155">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3A2da4c29f6d7041eca70b638b43d45437%40thread.v2')/messages('1615971548136')/hostedContents/$entity",
    "id": "aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv",
    "contentBytes": null,
    "contentType": null
}
```

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="ed66a-156">示例 2：获取图像的托管内容字节</span><span class="sxs-lookup"><span data-stu-id="ed66a-156">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="ed66a-157">请求</span><span class="sxs-lookup"><span data-stu-id="ed66a-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ed66a-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed66a-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontentchatmessage_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents/aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv/$value
```
# <a name="c"></a>[<span data-ttu-id="ed66a-159">C#</span><span class="sxs-lookup"><span data-stu-id="ed66a-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontentchatmessage-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed66a-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed66a-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontentchatmessage-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed66a-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed66a-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontentchatmessage-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed66a-162">Java</span><span class="sxs-lookup"><span data-stu-id="ed66a-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hostedcontentchatmessage-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ed66a-163">响应</span><span class="sxs-lookup"><span data-stu-id="ed66a-163">Response</span></span>

<span data-ttu-id="ed66a-164">响应包含正文中托管内容的字节。</span><span class="sxs-lookup"><span data-stu-id="ed66a-164">Response contains bytes for the hosted content in the body.</span></span> <span data-ttu-id="ed66a-165">`content-type` header 指定托管内容类型。</span><span class="sxs-lookup"><span data-stu-id="ed66a-165">`content-type` header specifies the kind of hosted content.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->

```http
HTTP/1.1 200 OK
Content-type: image/jpeg
Content-length: 201

{
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get chatMessageHostedContent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


