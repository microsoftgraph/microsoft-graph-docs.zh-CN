---
title: 列出 chatMessageHostedContents
description: 从邮件中检索 chatMessageHostedContent 对象的列表。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a39071d71728b6e510734ab05109f7c94a8a0e7f
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333389"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="be57c-103">列出 hostedContents</span><span class="sxs-lookup"><span data-stu-id="be57c-103">List hostedContents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be57c-104">从邮件中检索[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="be57c-104">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span>

## <a name="permissions"></a><span data-ttu-id="be57c-105">权限</span><span class="sxs-lookup"><span data-stu-id="be57c-105">Permissions</span></span>

<span data-ttu-id="be57c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be57c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be57c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="be57c-108">Permission type</span></span>                        | <span data-ttu-id="be57c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="be57c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="be57c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be57c-110">Delegated (work or school account)</span></span>|<span data-ttu-id="be57c-111">对于**用户**或**聊天**资源：</span><span class="sxs-lookup"><span data-stu-id="be57c-111">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="be57c-112">聊天、阅读和读写</span><span class="sxs-lookup"><span data-stu-id="be57c-112">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="be57c-113">对于**频道**资源：</span><span class="sxs-lookup"><span data-stu-id="be57c-113">For **channel** resource:</span></span><br/><span data-ttu-id="be57c-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be57c-114">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="be57c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be57c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be57c-116">不支持</span><span class="sxs-lookup"><span data-stu-id="be57c-116">Not supported</span></span>|
|<span data-ttu-id="be57c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="be57c-117">Application</span></span>| <span data-ttu-id="be57c-118">对于**用户**或**聊天**资源：</span><span class="sxs-lookup"><span data-stu-id="be57c-118">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="be57c-119">"聊天室"、"所有"、"全部聊天"</span><span class="sxs-lookup"><span data-stu-id="be57c-119">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="be57c-120">对于**频道**资源：</span><span class="sxs-lookup"><span data-stu-id="be57c-120">For **channel** resource:</span></span><br/><span data-ttu-id="be57c-121">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be57c-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="be57c-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be57c-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents
GET /users/{id}/chats/{id}/messages/{id}/hostedContents
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be57c-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="be57c-123">Optional query parameters</span></span>

<span data-ttu-id="be57c-124">此操作不支持[OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="be57c-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be57c-125">请求头</span><span class="sxs-lookup"><span data-stu-id="be57c-125">Request headers</span></span>

| <span data-ttu-id="be57c-126">名称</span><span class="sxs-lookup"><span data-stu-id="be57c-126">Name</span></span>      |<span data-ttu-id="be57c-127">说明</span><span class="sxs-lookup"><span data-stu-id="be57c-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="be57c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="be57c-128">Authorization</span></span> | <span data-ttu-id="be57c-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="be57c-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="be57c-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="be57c-130">Request body</span></span>

<span data-ttu-id="be57c-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="be57c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be57c-132">响应</span><span class="sxs-lookup"><span data-stu-id="be57c-132">Response</span></span>

<span data-ttu-id="be57c-133">如果成功，此方法在响应`200 OK`正文中返回响应代码和[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="be57c-133">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be57c-134">示例</span><span class="sxs-lookup"><span data-stu-id="be57c-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be57c-135">请求</span><span class="sxs-lookup"><span data-stu-id="be57c-135">Request</span></span>

<span data-ttu-id="be57c-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="be57c-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="be57c-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="be57c-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontents"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="be57c-138">C#</span><span class="sxs-lookup"><span data-stu-id="be57c-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="be57c-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be57c-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="be57c-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be57c-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="be57c-141">响应</span><span class="sxs-lookup"><span data-stu-id="be57c-141">Response</span></span>

<span data-ttu-id="be57c-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="be57c-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="be57c-143">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="be57c-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="be57c-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="be57c-144">All the properties will be returned from an actual call.</span></span>

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
  "value": [
    {
      "id": "id-value"
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
