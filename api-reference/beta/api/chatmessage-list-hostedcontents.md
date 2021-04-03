---
title: 列出 hostedContents
description: 从消息中检索 chatMessageHostedContent 对象的列表。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bd7e01dd6cc10efb57ff43d6b61c07def3895403
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51583031"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="e0dfe-103">列出 hostedContents</span><span class="sxs-lookup"><span data-stu-id="e0dfe-103">List hostedContents</span></span>

<span data-ttu-id="e0dfe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0dfe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0dfe-105">从消息中检索 [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-105">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span> <span data-ttu-id="e0dfe-106">此 API 仅列出托管的内容对象。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-106">This API only lists the hosted content objects.</span></span> <span data-ttu-id="e0dfe-107">若要获取内容字节，请参阅 [获取 chatmessage 托管内容](chatmessagehostedcontent-get.md)</span><span class="sxs-lookup"><span data-stu-id="e0dfe-107">To get the content bytes, see [get chatmessage hosted content](chatmessagehostedcontent-get.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="e0dfe-108">权限</span><span class="sxs-lookup"><span data-stu-id="e0dfe-108">Permissions</span></span>

### <a name="permissions-for-channel"></a><span data-ttu-id="e0dfe-109">频道权限</span><span class="sxs-lookup"><span data-stu-id="e0dfe-109">Permissions for channel</span></span>

| <span data-ttu-id="e0dfe-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0dfe-110">Permission type</span></span>                        | <span data-ttu-id="e0dfe-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0dfe-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="e0dfe-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0dfe-112">Delegated (work or school account)</span></span>| <span data-ttu-id="e0dfe-113">ChannelMessage.Read.All、Group.Read.All、Group.Read.WriteAll</span><span class="sxs-lookup"><span data-stu-id="e0dfe-113">ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="e0dfe-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0dfe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0dfe-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-115">Not supported.</span></span>|
|<span data-ttu-id="e0dfe-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0dfe-116">Application</span></span>| <span data-ttu-id="e0dfe-117">ChannelMessage.Read.Group、ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0dfe-117">ChannelMessage.Read.Group, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

### <a name="permissions-for-chat"></a><span data-ttu-id="e0dfe-118">聊天权限</span><span class="sxs-lookup"><span data-stu-id="e0dfe-118">Permissions for chat</span></span>

| <span data-ttu-id="e0dfe-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0dfe-119">Permission type</span></span>                        | <span data-ttu-id="e0dfe-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0dfe-120">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="e0dfe-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0dfe-121">Delegated (work or school account)</span></span>| <span data-ttu-id="e0dfe-122">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0dfe-122">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="e0dfe-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0dfe-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0dfe-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-124">Not supported.</span></span>|
|<span data-ttu-id="e0dfe-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0dfe-125">Application</span></span>| <span data-ttu-id="e0dfe-126">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0dfe-126">Chat.Read.All, Chat.ReadWrite.All</span></span>|

> <span data-ttu-id="e0dfe-127">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-127">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="e0dfe-128">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-128">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="e0dfe-129">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-129">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="e0dfe-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0dfe-130">HTTP request</span></span>

<span data-ttu-id="e0dfe-131">**获取频道消息中的 hostedContents**</span><span class="sxs-lookup"><span data-stu-id="e0dfe-131">**Get hostedContents in a channel message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/hostedContents
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies/{reply-id}/hostedContents
```

<span data-ttu-id="e0dfe-132">**获取聊天消息中的 hostedContents**</span><span class="sxs-lookup"><span data-stu-id="e0dfe-132">**Get hostedContents in a chat message**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/messages/{message-id}/hostedContents
GET /users/{user-id}/chats/{chat-id}/messages/{message-id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0dfe-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e0dfe-133">Optional query parameters</span></span>

<span data-ttu-id="e0dfe-134">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-134">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0dfe-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0dfe-135">Request headers</span></span>

| <span data-ttu-id="e0dfe-136">名称</span><span class="sxs-lookup"><span data-stu-id="e0dfe-136">Name</span></span>      |<span data-ttu-id="e0dfe-137">说明</span><span class="sxs-lookup"><span data-stu-id="e0dfe-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0dfe-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0dfe-138">Authorization</span></span> | <span data-ttu-id="e0dfe-139">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e0dfe-139">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0dfe-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0dfe-140">Request body</span></span>

<span data-ttu-id="e0dfe-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0dfe-142">响应</span><span class="sxs-lookup"><span data-stu-id="e0dfe-142">Response</span></span>

<span data-ttu-id="e0dfe-143">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-143">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e0dfe-144">示例</span><span class="sxs-lookup"><span data-stu-id="e0dfe-144">Examples</span></span>

### <a name="example-1-list-hosted-content-for-a-channel-message"></a><span data-ttu-id="e0dfe-145">示例 1：列出频道消息的托管内容</span><span class="sxs-lookup"><span data-stu-id="e0dfe-145">Example 1: List hosted content for a channel message</span></span>

#### <a name="request"></a><span data-ttu-id="e0dfe-146">请求</span><span class="sxs-lookup"><span data-stu-id="e0dfe-146">Request</span></span>

<span data-ttu-id="e0dfe-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_hostedcontentschannelmessage_1"
}-->
```http
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/hostedContents
```

#### <a name="response"></a><span data-ttu-id="e0dfe-148">响应</span><span class="sxs-lookup"><span data-stu-id="e0dfe-148">Response</span></span>

<span data-ttu-id="e0dfe-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-149">The following is an example of the response.</span></span>

> <span data-ttu-id="e0dfe-150">**注意：** `contentBytes` 和 `contentType` 始终设置为 null。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-150">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1616963377068')/hostedContents",
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

### <a name="example-2-list-hosted-content-for-reply-to-a-channel-message"></a><span data-ttu-id="e0dfe-151">示例 2：列出用于回复频道消息的托管内容</span><span class="sxs-lookup"><span data-stu-id="e0dfe-151">Example 2: List hosted content for reply to a channel message</span></span>

#### <a name="request"></a><span data-ttu-id="e0dfe-152">请求</span><span class="sxs-lookup"><span data-stu-id="e0dfe-152">Request</span></span>

<span data-ttu-id="e0dfe-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-153">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_hostedcontentschannelmessage_2"
}-->
```http
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/replies/1616963389737/hostedContents
```

#### <a name="response"></a><span data-ttu-id="e0dfe-154">响应</span><span class="sxs-lookup"><span data-stu-id="e0dfe-154">Response</span></span>

<span data-ttu-id="e0dfe-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-155">The following is an example of the response.</span></span>

> <span data-ttu-id="e0dfe-156">**注意：** `contentBytes` 和 `contentType` 始终设置为 null。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-156">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1616963377068')/replies('1616963389737')/hostedContents",
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

### <a name="example-2--list-hosted-content-for-message-in-a-chat"></a><span data-ttu-id="e0dfe-157">示例 2：列出聊天中消息的托管内容</span><span class="sxs-lookup"><span data-stu-id="e0dfe-157">Example 2 : List hosted content for message in a chat</span></span>

#### <a name="request"></a><span data-ttu-id="e0dfe-158">请求</span><span class="sxs-lookup"><span data-stu-id="e0dfe-158">Request</span></span>

<span data-ttu-id="e0dfe-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_hostedcontentschatmessage_1"
}-->
```http
GET https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents
```

#### <a name="response"></a><span data-ttu-id="e0dfe-160">响应</span><span class="sxs-lookup"><span data-stu-id="e0dfe-160">Response</span></span>

<span data-ttu-id="e0dfe-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-161">The following is an example of the response.</span></span>

> <span data-ttu-id="e0dfe-162">**注意：** `contentBytes` 和 `contentType` 始终设置为 null。</span><span class="sxs-lookup"><span data-stu-id="e0dfe-162">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3A2da4c29f6d7041eca70b638b43d45437%40thread.v2')/messages('1615971548136')/hostedContents",
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


