---
title: 获取 chatMessageHostedContent
description: 检索 chatMessageHostedContent 对象的属性和关系。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 56c96c812c1c5f8e8a6d471224bf8faef2733045
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947750"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="d789e-103">获取 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="d789e-103">Get chatMessageHostedContent</span></span>

<span data-ttu-id="d789e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d789e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d789e-105">检索 [chatMessageHostedContent 对象的属性和](../resources/chatmessagehostedcontent.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="d789e-105">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d789e-106">权限</span><span class="sxs-lookup"><span data-stu-id="d789e-106">Permissions</span></span>

<span data-ttu-id="d789e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d789e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d789e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d789e-109">Permission type</span></span>                        | <span data-ttu-id="d789e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d789e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="d789e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d789e-111">Delegated (work or school account)</span></span>| <span data-ttu-id="d789e-112">对于 **用户** 或 **聊天** 资源：Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d789e-112">For **user** or **chat** resource: Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="d789e-113">对于 **频道** 资源：ChannelMessage.Read.All、Group.Read.All、Group.Read.WriteAll</span><span class="sxs-lookup"><span data-stu-id="d789e-113">For **channel** resource: ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="d789e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d789e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d789e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d789e-115">Not supported.</span></span>|
|<span data-ttu-id="d789e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d789e-116">Application</span></span>| <span data-ttu-id="d789e-117">对于 **用户** 或 **聊天** 资源：Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d789e-117">For **user** or **chat** resource: Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="d789e-118">对于 **频道** 资源：ChannelMessage.Read.Group\*、ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d789e-118">For **channel** resource: ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="d789e-119">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="d789e-119">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="d789e-120">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="d789e-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="d789e-121">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="d789e-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="d789e-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d789e-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d789e-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d789e-123">Optional query parameters</span></span>

<span data-ttu-id="d789e-124">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d789e-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d789e-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="d789e-125">Request headers</span></span>

| <span data-ttu-id="d789e-126">名称</span><span class="sxs-lookup"><span data-stu-id="d789e-126">Name</span></span>      |<span data-ttu-id="d789e-127">说明</span><span class="sxs-lookup"><span data-stu-id="d789e-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d789e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="d789e-128">Authorization</span></span> | <span data-ttu-id="d789e-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d789e-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d789e-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d789e-130">Request body</span></span>

<span data-ttu-id="d789e-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d789e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d789e-132">响应</span><span class="sxs-lookup"><span data-stu-id="d789e-132">Response</span></span>

<span data-ttu-id="d789e-133">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d789e-133">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d789e-134">示例</span><span class="sxs-lookup"><span data-stu-id="d789e-134">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="d789e-135">示例 1：获取托管内容</span><span class="sxs-lookup"><span data-stu-id="d789e-135">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="d789e-136">请求</span><span class="sxs-lookup"><span data-stu-id="d789e-136">Request</span></span>

<span data-ttu-id="d789e-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d789e-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d789e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="d789e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="c"></a>[<span data-ttu-id="d789e-139">C#</span><span class="sxs-lookup"><span data-stu-id="d789e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d789e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d789e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d789e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d789e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d789e-142">Java</span><span class="sxs-lookup"><span data-stu-id="d789e-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chatmessagehostedcontent-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="d789e-143">响应</span><span class="sxs-lookup"><span data-stu-id="d789e-143">Response</span></span>

<span data-ttu-id="d789e-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d789e-144">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="d789e-145">为了可读性，可能会缩短此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d789e-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d789e-146">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d789e-146">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="d789e-147">示例 2：获取图像的托管内容字节</span><span class="sxs-lookup"><span data-stu-id="d789e-147">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="d789e-148">请求</span><span class="sxs-lookup"><span data-stu-id="d789e-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d789e-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="d789e-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}/$value
```
# <a name="c"></a>[<span data-ttu-id="d789e-150">C#</span><span class="sxs-lookup"><span data-stu-id="d789e-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d789e-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d789e-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d789e-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d789e-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d789e-153">Java</span><span class="sxs-lookup"><span data-stu-id="d789e-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chatmessagehostedcontent-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d789e-154">响应</span><span class="sxs-lookup"><span data-stu-id="d789e-154">Response</span></span>

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


