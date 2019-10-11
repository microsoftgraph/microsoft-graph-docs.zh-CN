---
title: 获取 chatMessageHostedContent
description: 检索 chatMessageHostedContent 对象的属性和关系。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e911091bb4e1b5cd3179f781dd0d2f326f121a3d
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439861"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="e15b2-103">获取 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="e15b2-103">Get chatMessageHostedContent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e15b2-104">检索[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e15b2-104">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e15b2-105">权限</span><span class="sxs-lookup"><span data-stu-id="e15b2-105">Permissions</span></span>

<span data-ttu-id="e15b2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e15b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e15b2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e15b2-108">Permission type</span></span>                        | <span data-ttu-id="e15b2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e15b2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="e15b2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e15b2-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e15b2-111">对于**用户**或**聊天**资源：</span><span class="sxs-lookup"><span data-stu-id="e15b2-111">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="e15b2-112">聊天、阅读和读写</span><span class="sxs-lookup"><span data-stu-id="e15b2-112">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="e15b2-113">对于**频道**资源：</span><span class="sxs-lookup"><span data-stu-id="e15b2-113">For **channel** resource:</span></span><br/><span data-ttu-id="e15b2-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e15b2-114">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="e15b2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e15b2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e15b2-116">不支持</span><span class="sxs-lookup"><span data-stu-id="e15b2-116">Not supported</span></span>|
|<span data-ttu-id="e15b2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e15b2-117">Application</span></span>| <span data-ttu-id="e15b2-118">对于**用户**或**聊天**资源：</span><span class="sxs-lookup"><span data-stu-id="e15b2-118">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="e15b2-119">"聊天室"、"所有"、"全部聊天"</span><span class="sxs-lookup"><span data-stu-id="e15b2-119">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="e15b2-120">对于**频道**资源：</span><span class="sxs-lookup"><span data-stu-id="e15b2-120">For **channel** resource:</span></span><br/><span data-ttu-id="e15b2-121">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e15b2-121">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="e15b2-122">在使用应用程序权限调用此 API 之前，您必须请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="e15b2-122">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="e15b2-123">有关详细信息，请参阅[Microsoft 团队中的受保护 api](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="e15b2-123">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="e15b2-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e15b2-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e15b2-125">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="e15b2-125">Optional query parameters</span></span>

<span data-ttu-id="e15b2-126">此操作不支持[OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e15b2-126">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e15b2-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="e15b2-127">Request headers</span></span>

| <span data-ttu-id="e15b2-128">名称</span><span class="sxs-lookup"><span data-stu-id="e15b2-128">Name</span></span>      |<span data-ttu-id="e15b2-129">说明</span><span class="sxs-lookup"><span data-stu-id="e15b2-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e15b2-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="e15b2-130">Authorization</span></span> | <span data-ttu-id="e15b2-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e15b2-131">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e15b2-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="e15b2-132">Request body</span></span>

<span data-ttu-id="e15b2-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e15b2-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e15b2-134">响应</span><span class="sxs-lookup"><span data-stu-id="e15b2-134">Response</span></span>

<span data-ttu-id="e15b2-135">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e15b2-135">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e15b2-136">示例</span><span class="sxs-lookup"><span data-stu-id="e15b2-136">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="e15b2-137">示例1：获取托管内容</span><span class="sxs-lookup"><span data-stu-id="e15b2-137">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="e15b2-138">请求</span><span class="sxs-lookup"><span data-stu-id="e15b2-138">Request</span></span>

<span data-ttu-id="e15b2-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e15b2-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e15b2-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="e15b2-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e15b2-141">C#</span><span class="sxs-lookup"><span data-stu-id="e15b2-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e15b2-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e15b2-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e15b2-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e15b2-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e15b2-144">响应</span><span class="sxs-lookup"><span data-stu-id="e15b2-144">Response</span></span>

<span data-ttu-id="e15b2-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e15b2-145">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="e15b2-146">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e15b2-146">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e15b2-147">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e15b2-147">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="e15b2-148">示例2：获取图像的托管内容字节</span><span class="sxs-lookup"><span data-stu-id="e15b2-148">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="e15b2-149">请求</span><span class="sxs-lookup"><span data-stu-id="e15b2-149">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e15b2-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="e15b2-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}/$value
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e15b2-151">C#</span><span class="sxs-lookup"><span data-stu-id="e15b2-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e15b2-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e15b2-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e15b2-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e15b2-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e15b2-154">响应</span><span class="sxs-lookup"><span data-stu-id="e15b2-154">Response</span></span>

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
