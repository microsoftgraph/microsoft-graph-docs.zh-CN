---
title: 列出 chatMessageHostedContents
description: 从邮件中检索 chatMessageHostedContent 对象的列表。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 077b3305ce2b342a32f52371d8382b49bd25a55d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958183"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="1b440-103">列出 hostedContents</span><span class="sxs-lookup"><span data-stu-id="1b440-103">List hostedContents</span></span>

<span data-ttu-id="1b440-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b440-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b440-105">从邮件中检索 [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="1b440-105">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b440-106">权限</span><span class="sxs-lookup"><span data-stu-id="1b440-106">Permissions</span></span>

<span data-ttu-id="1b440-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b440-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1b440-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b440-109">Permission type</span></span>                        | <span data-ttu-id="1b440-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b440-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="1b440-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b440-111">Delegated (work or school account)</span></span>| <span data-ttu-id="1b440-112">对于 **用户** 或 **聊天** 资源：聊天、阅读、读写</span><span class="sxs-lookup"><span data-stu-id="1b440-112">For **user** or **chat** resource: Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="1b440-113">对于 **信道** 资源： ChannelMessage、Group. WriteAll。请参阅。</span><span class="sxs-lookup"><span data-stu-id="1b440-113">For **channel** resource: ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="1b440-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b440-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b440-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b440-115">Not supported.</span></span>|
|<span data-ttu-id="1b440-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b440-116">Application</span></span>| <span data-ttu-id="1b440-117">对于 **用户** 或 **聊天** 资源：聊天、全部、聊天室。所有</span><span class="sxs-lookup"><span data-stu-id="1b440-117">For **user** or **chat** resource: Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="1b440-118">对于 **信道** 资源： ChannelMessage \*、ChannelMessage、group. All、Group. All。 all</span><span class="sxs-lookup"><span data-stu-id="1b440-118">For **channel** resource: ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="1b440-119">**注意** ：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="1b440-119">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="1b440-120">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="1b440-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="1b440-121">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="1b440-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="1b440-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b440-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents
GET /users/{id}/chats/{id}/messages/{id}/hostedContents
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1b440-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1b440-123">Optional query parameters</span></span>

<span data-ttu-id="1b440-124">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1b440-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b440-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b440-125">Request headers</span></span>

| <span data-ttu-id="1b440-126">名称</span><span class="sxs-lookup"><span data-stu-id="1b440-126">Name</span></span>      |<span data-ttu-id="1b440-127">说明</span><span class="sxs-lookup"><span data-stu-id="1b440-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1b440-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b440-128">Authorization</span></span> | <span data-ttu-id="1b440-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1b440-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b440-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b440-130">Request body</span></span>

<span data-ttu-id="1b440-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1b440-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b440-132">响应</span><span class="sxs-lookup"><span data-stu-id="1b440-132">Response</span></span>

<span data-ttu-id="1b440-133">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1b440-133">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b440-134">示例</span><span class="sxs-lookup"><span data-stu-id="1b440-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1b440-135">请求</span><span class="sxs-lookup"><span data-stu-id="1b440-135">Request</span></span>

<span data-ttu-id="1b440-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1b440-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b440-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b440-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontents"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents
```
# <a name="c"></a>[<span data-ttu-id="1b440-138">C#</span><span class="sxs-lookup"><span data-stu-id="1b440-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b440-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b440-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b440-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b440-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b440-141">Java</span><span class="sxs-lookup"><span data-stu-id="1b440-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hostedcontents-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1b440-142">响应</span><span class="sxs-lookup"><span data-stu-id="1b440-142">Response</span></span>

<span data-ttu-id="1b440-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1b440-143">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="1b440-144">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1b440-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1b440-145">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1b440-145">All the properties will be returned from an actual call.</span></span>

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


