---
title: 在聊天中获取选项卡
description: '检索聊天中指定选项卡的属性和关系。 '
author: subray
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 891bb59e4c2000f73c454e66e9b1b1398b22bb1c
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971326"
---
# <a name="get-tab-in-chat"></a><span data-ttu-id="96744-103">在聊天中获取选项卡</span><span class="sxs-lookup"><span data-stu-id="96744-103">Get tab in chat</span></span>

<span data-ttu-id="96744-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96744-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96744-105">检索聊天中指定 [选项卡](../resources/teamstab.md) 的属性和 [关系](../resources/chat.md)。</span><span class="sxs-lookup"><span data-stu-id="96744-105">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md) in a [chat](../resources/chat.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="96744-106">权限</span><span class="sxs-lookup"><span data-stu-id="96744-106">Permissions</span></span>
<span data-ttu-id="96744-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96744-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96744-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="96744-109">Permission type</span></span>      | <span data-ttu-id="96744-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96744-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96744-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96744-111">Delegated (work or school account)</span></span> | <span data-ttu-id="96744-112">TeamsTab.ReadWriteForChat、TeamsTab.Read.All、TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96744-112">TeamsTab.ReadWriteForChat, TeamsTab.Read.All, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="96744-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96744-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96744-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="96744-114">Not supported.</span></span>    |
|<span data-ttu-id="96744-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="96744-115">Application</span></span> | <span data-ttu-id="96744-116">TeamsTab.Read.Chat、TeamsTab.ReadWrite.Chat、TeamsTab.ReadWriteForChat.All、TeamsTab.Read.All、TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96744-116">TeamsTab.Read.Chat *, TeamsTab.ReadWrite.Chat*, TeamsTab.ReadWriteForChat.All, TeamsTab.Read.All, TeamsTab.ReadWrite.All</span></span> |

> <span data-ttu-id="96744-117">**注意**：标有 \* 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="96744-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="96744-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96744-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
GET /chats/{chat-id}/tabs/{tab-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96744-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="96744-119">Optional query parameters</span></span>

<span data-ttu-id="96744-120">此方法支持`$select` 和 `$expand` [OData 查询参数](/graph/query-parameters)，以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="96744-120">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96744-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="96744-121">Request headers</span></span>
| <span data-ttu-id="96744-122">标头</span><span class="sxs-lookup"><span data-stu-id="96744-122">Header</span></span>       | <span data-ttu-id="96744-123">值</span><span class="sxs-lookup"><span data-stu-id="96744-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="96744-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="96744-124">Authorization</span></span>  | <span data-ttu-id="96744-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96744-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="96744-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="96744-127">Request body</span></span>
<span data-ttu-id="96744-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96744-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96744-129">响应</span><span class="sxs-lookup"><span data-stu-id="96744-129">Response</span></span>

<span data-ttu-id="96744-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [tab](../resources/teamstab.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="96744-130">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="96744-131">示例</span><span class="sxs-lookup"><span data-stu-id="96744-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="96744-132">请求</span><span class="sxs-lookup"><span data-stu-id="96744-132">Request</span></span>
<span data-ttu-id="96744-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="96744-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="96744-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="96744-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tab_in_chat"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d?$expand=teamsApp
```
# <a name="c"></a>[<span data-ttu-id="96744-135">C#</span><span class="sxs-lookup"><span data-stu-id="96744-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tab-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96744-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96744-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tab-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96744-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96744-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tab-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96744-138">Java</span><span class="sxs-lookup"><span data-stu-id="96744-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tab-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="96744-139">响应</span><span class="sxs-lookup"><span data-stu-id="96744-139">Response</span></span>
<span data-ttu-id="96744-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="96744-140">The following is an example of the response.</span></span> 

><span data-ttu-id="96744-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="96744-141">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsTab"
}
-->  

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "tabId",
  "displayName": "My Contoso Tab - updated",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "teamsApp": {
      "id": "0d820ecd-def2-4297-adad-78056cde7c78",
      "externalId": null,
      "displayName": "Contoso",
      "distributionMethod": "store"
  },
  "sortOrderIndex": "20",
  "messageId": "1607411534158",
  "webUrl": "https://teams.microsoft.com/l/entity/com.microsoft.teamspace.tab.web/_djb2_msteams_prefix_193fe248-24e6-478f-a66c-ede9ce6dd547?context=%7b%0d%0a++%22context%22%3a+%22chat%22%2c%0d%0a++%22chatId%22%3a+%2219%3ad65713bc498c4a428c71ef9353e6ce20%40thread.v2%22%2c%0d%0a++%22subEntityId%22%3a+null%0d%0a%7d&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924"
}
```

## <a name="see-also"></a><span data-ttu-id="96744-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="96744-142">See also</span></span>

- [<span data-ttu-id="96744-143">获取频道中的选项卡</span><span class="sxs-lookup"><span data-stu-id="96744-143">Get tab in channel</span></span>](channel-get-tabs.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a tab in chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


