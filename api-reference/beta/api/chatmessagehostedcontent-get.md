---
title: 获取 chatMessageHostedContent
description: 检索 chatMessageHostedContent 对象的属性和关系。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d62ffb6fdf88649971992fc42e25ce16be6ae7ab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438293"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="87efe-103">获取 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="87efe-103">Get chatMessageHostedContent</span></span>

<span data-ttu-id="87efe-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="87efe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87efe-105">检索[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="87efe-105">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="87efe-106">权限</span><span class="sxs-lookup"><span data-stu-id="87efe-106">Permissions</span></span>

<span data-ttu-id="87efe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="87efe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="87efe-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="87efe-109">Permission type</span></span>                        | <span data-ttu-id="87efe-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="87efe-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="87efe-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87efe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="87efe-112">对于**用户**或**聊天**资源：</span><span class="sxs-lookup"><span data-stu-id="87efe-112">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="87efe-113">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87efe-113">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="87efe-114">对于**频道**资源：</span><span class="sxs-lookup"><span data-stu-id="87efe-114">For **channel** resource:</span></span><br/><span data-ttu-id="87efe-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87efe-115">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="87efe-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87efe-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87efe-117">不支持</span><span class="sxs-lookup"><span data-stu-id="87efe-117">Not supported</span></span>|
|<span data-ttu-id="87efe-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="87efe-118">Application</span></span>| <span data-ttu-id="87efe-119">对于**用户**或**聊天**资源：</span><span class="sxs-lookup"><span data-stu-id="87efe-119">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="87efe-120">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87efe-120">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="87efe-121">对于**频道**资源：</span><span class="sxs-lookup"><span data-stu-id="87efe-121">For **channel** resource:</span></span><br/><span data-ttu-id="87efe-122">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87efe-122">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="87efe-123">在调用具有应用程序权限的此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="87efe-123">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="87efe-124">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="87efe-124">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="87efe-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87efe-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87efe-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="87efe-126">Optional query parameters</span></span>

<span data-ttu-id="87efe-127">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="87efe-127">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87efe-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="87efe-128">Request headers</span></span>

| <span data-ttu-id="87efe-129">名称</span><span class="sxs-lookup"><span data-stu-id="87efe-129">Name</span></span>      |<span data-ttu-id="87efe-130">说明</span><span class="sxs-lookup"><span data-stu-id="87efe-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="87efe-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="87efe-131">Authorization</span></span> | <span data-ttu-id="87efe-132">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="87efe-132">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="87efe-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="87efe-133">Request body</span></span>

<span data-ttu-id="87efe-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="87efe-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87efe-135">响应</span><span class="sxs-lookup"><span data-stu-id="87efe-135">Response</span></span>

<span data-ttu-id="87efe-136">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="87efe-136">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="87efe-137">示例</span><span class="sxs-lookup"><span data-stu-id="87efe-137">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="87efe-138">示例1：获取托管内容</span><span class="sxs-lookup"><span data-stu-id="87efe-138">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="87efe-139">请求</span><span class="sxs-lookup"><span data-stu-id="87efe-139">Request</span></span>

<span data-ttu-id="87efe-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="87efe-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="87efe-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="87efe-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="c"></a>[<span data-ttu-id="87efe-142">C#</span><span class="sxs-lookup"><span data-stu-id="87efe-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87efe-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87efe-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87efe-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87efe-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="87efe-145">响应</span><span class="sxs-lookup"><span data-stu-id="87efe-145">Response</span></span>

<span data-ttu-id="87efe-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="87efe-146">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="87efe-147">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="87efe-147">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="87efe-148">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="87efe-148">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="87efe-149">示例2：获取图像的托管内容字节</span><span class="sxs-lookup"><span data-stu-id="87efe-149">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="87efe-150">请求</span><span class="sxs-lookup"><span data-stu-id="87efe-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="87efe-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="87efe-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}/$value
```
# <a name="c"></a>[<span data-ttu-id="87efe-152">C#</span><span class="sxs-lookup"><span data-stu-id="87efe-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87efe-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87efe-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87efe-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87efe-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="87efe-155">响应</span><span class="sxs-lookup"><span data-stu-id="87efe-155">Response</span></span>

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
