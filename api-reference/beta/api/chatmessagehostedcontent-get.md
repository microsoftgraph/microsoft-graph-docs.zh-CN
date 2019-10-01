---
title: 获取 chatMessageHostedContent
description: 检索 chatMessageHostedContent 对象的属性和关系。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e15f8aa932e2534b80fbee0c7d00d759191bc42d
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333218"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="7b822-103">获取 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="7b822-103">Get chatMessageHostedContent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b822-104">检索[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7b822-104">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b822-105">权限</span><span class="sxs-lookup"><span data-stu-id="7b822-105">Permissions</span></span>

<span data-ttu-id="7b822-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b822-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b822-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b822-108">Permission type</span></span>                        | <span data-ttu-id="7b822-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b822-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="7b822-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b822-110">Delegated (work or school account)</span></span>|<span data-ttu-id="7b822-111">对于**用户**或**聊天**资源：</span><span class="sxs-lookup"><span data-stu-id="7b822-111">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="7b822-112">聊天、阅读和读写</span><span class="sxs-lookup"><span data-stu-id="7b822-112">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="7b822-113">对于**频道**资源：</span><span class="sxs-lookup"><span data-stu-id="7b822-113">For **channel** resource:</span></span><br/><span data-ttu-id="7b822-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b822-114">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="7b822-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b822-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b822-116">不支持</span><span class="sxs-lookup"><span data-stu-id="7b822-116">Not supported</span></span>|
|<span data-ttu-id="7b822-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b822-117">Application</span></span>| <span data-ttu-id="7b822-118">对于**用户**或**聊天**资源：</span><span class="sxs-lookup"><span data-stu-id="7b822-118">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="7b822-119">"聊天室"、"所有"、"全部聊天"</span><span class="sxs-lookup"><span data-stu-id="7b822-119">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="7b822-120">对于**频道**资源：</span><span class="sxs-lookup"><span data-stu-id="7b822-120">For **channel** resource:</span></span><br/><span data-ttu-id="7b822-121">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b822-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b822-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b822-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b822-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7b822-123">Optional query parameters</span></span>

<span data-ttu-id="7b822-124">此操作不支持[OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7b822-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b822-125">请求头</span><span class="sxs-lookup"><span data-stu-id="7b822-125">Request headers</span></span>

| <span data-ttu-id="7b822-126">名称</span><span class="sxs-lookup"><span data-stu-id="7b822-126">Name</span></span>      |<span data-ttu-id="7b822-127">说明</span><span class="sxs-lookup"><span data-stu-id="7b822-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7b822-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b822-128">Authorization</span></span> | <span data-ttu-id="7b822-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7b822-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b822-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b822-130">Request body</span></span>

<span data-ttu-id="7b822-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7b822-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b822-132">响应</span><span class="sxs-lookup"><span data-stu-id="7b822-132">Response</span></span>

<span data-ttu-id="7b822-133">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7b822-133">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7b822-134">示例</span><span class="sxs-lookup"><span data-stu-id="7b822-134">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="7b822-135">示例1：获取托管内容</span><span class="sxs-lookup"><span data-stu-id="7b822-135">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="7b822-136">请求</span><span class="sxs-lookup"><span data-stu-id="7b822-136">Request</span></span>

<span data-ttu-id="7b822-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7b822-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7b822-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b822-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7b822-139">C#</span><span class="sxs-lookup"><span data-stu-id="7b822-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7b822-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b822-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7b822-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b822-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7b822-142">响应</span><span class="sxs-lookup"><span data-stu-id="7b822-142">Response</span></span>

<span data-ttu-id="7b822-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7b822-143">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="7b822-144">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7b822-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7b822-145">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7b822-145">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="7b822-146">示例2：获取图像的托管内容字节</span><span class="sxs-lookup"><span data-stu-id="7b822-146">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="7b822-147">请求</span><span class="sxs-lookup"><span data-stu-id="7b822-147">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}/$value
```

#### <a name="response"></a><span data-ttu-id="7b822-148">响应</span><span class="sxs-lookup"><span data-stu-id="7b822-148">Response</span></span>

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
