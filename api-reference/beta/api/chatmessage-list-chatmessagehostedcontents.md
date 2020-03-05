---
title: 列出 chatMessageHostedContents
description: 从邮件中检索 chatMessageHostedContent 对象的列表。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0be0b5668b4e583b855ae4e4e85fdb7bc4169705
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438370"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="66a34-103">列出 hostedContents</span><span class="sxs-lookup"><span data-stu-id="66a34-103">List hostedContents</span></span>

<span data-ttu-id="66a34-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="66a34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66a34-105">从邮件中检索[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="66a34-105">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span>

## <a name="permissions"></a><span data-ttu-id="66a34-106">权限</span><span class="sxs-lookup"><span data-stu-id="66a34-106">Permissions</span></span>

<span data-ttu-id="66a34-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66a34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66a34-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="66a34-109">Permission type</span></span>                        | <span data-ttu-id="66a34-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="66a34-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="66a34-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66a34-111">Delegated (work or school account)</span></span>|<span data-ttu-id="66a34-112">对于**用户**或**聊天**资源：</span><span class="sxs-lookup"><span data-stu-id="66a34-112">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="66a34-113">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66a34-113">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="66a34-114">对于**频道**资源：</span><span class="sxs-lookup"><span data-stu-id="66a34-114">For **channel** resource:</span></span><br/><span data-ttu-id="66a34-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66a34-115">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="66a34-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66a34-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66a34-117">不支持</span><span class="sxs-lookup"><span data-stu-id="66a34-117">Not supported</span></span>|
|<span data-ttu-id="66a34-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="66a34-118">Application</span></span>| <span data-ttu-id="66a34-119">对于**用户**或**聊天**资源：</span><span class="sxs-lookup"><span data-stu-id="66a34-119">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="66a34-120">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66a34-120">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="66a34-121">对于**频道**资源：</span><span class="sxs-lookup"><span data-stu-id="66a34-121">For **channel** resource:</span></span><br/><span data-ttu-id="66a34-122">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66a34-122">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="66a34-123">在调用具有应用程序权限的此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="66a34-123">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="66a34-124">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="66a34-124">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="66a34-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66a34-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents
GET /users/{id}/chats/{id}/messages/{id}/hostedContents
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="66a34-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="66a34-126">Optional query parameters</span></span>

<span data-ttu-id="66a34-127">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="66a34-127">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66a34-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="66a34-128">Request headers</span></span>

| <span data-ttu-id="66a34-129">名称</span><span class="sxs-lookup"><span data-stu-id="66a34-129">Name</span></span>      |<span data-ttu-id="66a34-130">说明</span><span class="sxs-lookup"><span data-stu-id="66a34-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="66a34-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="66a34-131">Authorization</span></span> | <span data-ttu-id="66a34-132">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="66a34-132">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="66a34-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="66a34-133">Request body</span></span>

<span data-ttu-id="66a34-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="66a34-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66a34-135">响应</span><span class="sxs-lookup"><span data-stu-id="66a34-135">Response</span></span>

<span data-ttu-id="66a34-136">如果成功，此方法在响应`200 OK`正文中返回响应代码和[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="66a34-136">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66a34-137">示例</span><span class="sxs-lookup"><span data-stu-id="66a34-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="66a34-138">请求</span><span class="sxs-lookup"><span data-stu-id="66a34-138">Request</span></span>

<span data-ttu-id="66a34-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="66a34-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="66a34-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="66a34-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontents"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents
```
# <a name="c"></a>[<span data-ttu-id="66a34-141">C#</span><span class="sxs-lookup"><span data-stu-id="66a34-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66a34-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66a34-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66a34-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66a34-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="66a34-144">响应</span><span class="sxs-lookup"><span data-stu-id="66a34-144">Response</span></span>

<span data-ttu-id="66a34-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="66a34-145">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="66a34-146">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="66a34-146">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="66a34-147">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="66a34-147">All the properties will be returned from an actual call.</span></span>

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
