---
title: 获取 chatMessageHostedContent
description: 检索 chatMessageHostedContent 对象的属性和关系。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ca3fca6ddf7801df8ed7f23285c35029aaaab14e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437710"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="f66ae-103">获取 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="f66ae-103">Get chatMessageHostedContent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f66ae-104">检索[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f66ae-104">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f66ae-105">权限</span><span class="sxs-lookup"><span data-stu-id="f66ae-105">Permissions</span></span>

<span data-ttu-id="f66ae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f66ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f66ae-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f66ae-108">Permission type</span></span>                        | <span data-ttu-id="f66ae-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f66ae-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f66ae-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f66ae-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f66ae-111">聊天、阅读和读写</span><span class="sxs-lookup"><span data-stu-id="f66ae-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="f66ae-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f66ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f66ae-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f66ae-113">Not supported.</span></span> |
| <span data-ttu-id="f66ae-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f66ae-114">Application</span></span>                            | <span data-ttu-id="f66ae-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f66ae-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f66ae-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f66ae-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f66ae-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f66ae-117">Optional query parameters</span></span>

<span data-ttu-id="f66ae-118">此操作不支持[OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f66ae-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f66ae-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f66ae-119">Request headers</span></span>

| <span data-ttu-id="f66ae-120">名称</span><span class="sxs-lookup"><span data-stu-id="f66ae-120">Name</span></span>      |<span data-ttu-id="f66ae-121">说明</span><span class="sxs-lookup"><span data-stu-id="f66ae-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f66ae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f66ae-122">Authorization</span></span> | <span data-ttu-id="f66ae-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f66ae-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f66ae-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f66ae-124">Request body</span></span>

<span data-ttu-id="f66ae-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f66ae-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f66ae-126">响应</span><span class="sxs-lookup"><span data-stu-id="f66ae-126">Response</span></span>

<span data-ttu-id="f66ae-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和请求的[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f66ae-127">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f66ae-128">示例</span><span class="sxs-lookup"><span data-stu-id="f66ae-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f66ae-129">请求</span><span class="sxs-lookup"><span data-stu-id="f66ae-129">Request</span></span>

<span data-ttu-id="f66ae-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f66ae-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f66ae-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f66ae-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f66ae-132">C#</span><span class="sxs-lookup"><span data-stu-id="f66ae-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f66ae-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="f66ae-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f66ae-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="f66ae-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f66ae-135">响应</span><span class="sxs-lookup"><span data-stu-id="f66ae-135">Response</span></span>

<span data-ttu-id="f66ae-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f66ae-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="f66ae-137">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f66ae-137">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f66ae-138">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f66ae-138">All the properties will be returned from an actual call.</span></span>

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
