---
title: 获取 chatMessageHostedContent
description: 检索 chatMessageHostedContent 对象的属性和关系。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: eb5c56eb1a67e8fac936e9a80600f8291cd595d4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982579"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="44a7c-103">获取 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="44a7c-103">Get chatMessageHostedContent</span></span>

<span data-ttu-id="44a7c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44a7c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44a7c-105">检索 [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="44a7c-105">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="44a7c-106">权限</span><span class="sxs-lookup"><span data-stu-id="44a7c-106">Permissions</span></span>

<span data-ttu-id="44a7c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44a7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44a7c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="44a7c-109">Permission type</span></span>                        | <span data-ttu-id="44a7c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44a7c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="44a7c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44a7c-111">Delegated (work or school account)</span></span>| <span data-ttu-id="44a7c-112">对于 **用户** 或 **聊天** 资源：聊天、阅读、读写</span><span class="sxs-lookup"><span data-stu-id="44a7c-112">For **user** or **chat** resource: Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="44a7c-113">对于 **信道** 资源： ChannelMessage、Group. WriteAll。请参阅。</span><span class="sxs-lookup"><span data-stu-id="44a7c-113">For **channel** resource: ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="44a7c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44a7c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44a7c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="44a7c-115">Not supported.</span></span>|
|<span data-ttu-id="44a7c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="44a7c-116">Application</span></span>| <span data-ttu-id="44a7c-117">对于 **用户** 或 **聊天** 资源：聊天、全部、聊天室。所有</span><span class="sxs-lookup"><span data-stu-id="44a7c-117">For **user** or **chat** resource: Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="44a7c-118">对于 **信道** 资源： ChannelMessage \*、ChannelMessage、group. All、Group. All。 all</span><span class="sxs-lookup"><span data-stu-id="44a7c-118">For **channel** resource: ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="44a7c-119">**注意**：标有 \* 的权限用于[特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="44a7c-119">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="44a7c-120">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="44a7c-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="44a7c-121">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="44a7c-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="44a7c-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44a7c-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="44a7c-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="44a7c-123">Optional query parameters</span></span>

<span data-ttu-id="44a7c-124">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="44a7c-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44a7c-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="44a7c-125">Request headers</span></span>

| <span data-ttu-id="44a7c-126">名称</span><span class="sxs-lookup"><span data-stu-id="44a7c-126">Name</span></span>      |<span data-ttu-id="44a7c-127">说明</span><span class="sxs-lookup"><span data-stu-id="44a7c-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="44a7c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="44a7c-128">Authorization</span></span> | <span data-ttu-id="44a7c-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="44a7c-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="44a7c-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="44a7c-130">Request body</span></span>

<span data-ttu-id="44a7c-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="44a7c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44a7c-132">响应</span><span class="sxs-lookup"><span data-stu-id="44a7c-132">Response</span></span>

<span data-ttu-id="44a7c-133">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="44a7c-133">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="44a7c-134">示例</span><span class="sxs-lookup"><span data-stu-id="44a7c-134">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="44a7c-135">示例1：获取托管内容</span><span class="sxs-lookup"><span data-stu-id="44a7c-135">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="44a7c-136">请求</span><span class="sxs-lookup"><span data-stu-id="44a7c-136">Request</span></span>

<span data-ttu-id="44a7c-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="44a7c-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="44a7c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="44a7c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="c"></a>[<span data-ttu-id="44a7c-139">C#</span><span class="sxs-lookup"><span data-stu-id="44a7c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44a7c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44a7c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44a7c-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44a7c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="44a7c-142">响应</span><span class="sxs-lookup"><span data-stu-id="44a7c-142">Response</span></span>

<span data-ttu-id="44a7c-143">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="44a7c-143">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="44a7c-144">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="44a7c-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="44a7c-145">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="44a7c-145">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="44a7c-146">示例2：获取图像的托管内容字节</span><span class="sxs-lookup"><span data-stu-id="44a7c-146">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="44a7c-147">请求</span><span class="sxs-lookup"><span data-stu-id="44a7c-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="44a7c-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="44a7c-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}/$value
```
# <a name="c"></a>[<span data-ttu-id="44a7c-149">C#</span><span class="sxs-lookup"><span data-stu-id="44a7c-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44a7c-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44a7c-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44a7c-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44a7c-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="44a7c-152">响应</span><span class="sxs-lookup"><span data-stu-id="44a7c-152">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->

```http
HTTP/1.1 200 OK
Content-type: image/jpeg
Content-length: 201
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


