---
title: 聊天中的"更新"选项卡
description: 更新聊天中指定选项卡的属性。
author: subray
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ac9781e0d8fd5137366d93c8fbf49bc946e6c51c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949992"
---
# <a name="update-tab-in-chat"></a><span data-ttu-id="acada-103">聊天中的"更新"选项卡</span><span class="sxs-lookup"><span data-stu-id="acada-103">Update tab in chat</span></span>

<span data-ttu-id="acada-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acada-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="acada-105">更新聊天中[指定选项卡](../resources/teamstab.md)[的属性](../resources/chat.md)。</span><span class="sxs-lookup"><span data-stu-id="acada-105">Update the properties of the specified [tab](../resources/teamstab.md) in a [chat](../resources/chat.md).</span></span> <span data-ttu-id="acada-106">这可用于配置选项卡的内容。</span><span class="sxs-lookup"><span data-stu-id="acada-106">This can be used to configure the content of the tab.</span></span>

> <span data-ttu-id="acada-107">**注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md) 实例关联，则实际上，将更新固定在会议中的选项卡。</span><span class="sxs-lookup"><span data-stu-id="acada-107">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the tab pinned in the meeting will be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="acada-108">权限</span><span class="sxs-lookup"><span data-stu-id="acada-108">Permissions</span></span>
<span data-ttu-id="acada-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="acada-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="acada-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="acada-111">Permission type</span></span>      | <span data-ttu-id="acada-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="acada-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acada-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="acada-113">Delegated (work or school account)</span></span> | <span data-ttu-id="acada-114">TeamsTab.ReadWriteForChat、TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acada-114">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="acada-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="acada-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acada-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="acada-116">Not supported.</span></span>    |
|<span data-ttu-id="acada-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="acada-117">Application</span></span> | <span data-ttu-id="acada-118">TeamsTab.ReadWriteForChat、TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acada-118">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="acada-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="acada-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /chats/{chat-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="acada-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="acada-120">Request headers</span></span>
| <span data-ttu-id="acada-121">标头</span><span class="sxs-lookup"><span data-stu-id="acada-121">Header</span></span>       | <span data-ttu-id="acada-122">值</span><span class="sxs-lookup"><span data-stu-id="acada-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="acada-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="acada-123">Authorization</span></span>  | <span data-ttu-id="acada-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="acada-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="acada-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="acada-126">Content-Type</span></span>  | <span data-ttu-id="acada-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="acada-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="acada-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="acada-129">Request body</span></span>
<span data-ttu-id="acada-130">在请求正文中，提供 tab 对象的 JSON [表示](../resources/teamstab.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="acada-130">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="acada-131">响应</span><span class="sxs-lookup"><span data-stu-id="acada-131">Response</span></span>

<span data-ttu-id="acada-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 **teamsTab** 资源。</span><span class="sxs-lookup"><span data-stu-id="acada-132">If successful, this method returns a `200 OK` response code and the updated **teamsTab** resource in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="acada-133">示例</span><span class="sxs-lookup"><span data-stu-id="acada-133">Examples</span></span>
### <a name="example-1-update-the-name-of-a-tab-in-a-chat"></a><span data-ttu-id="acada-134">示例 1：更新聊天中选项卡的名称</span><span class="sxs-lookup"><span data-stu-id="acada-134">Example 1: Update the name of a tab in a chat</span></span>

#### <a name="request"></a><span data-ttu-id="acada-135">请求</span><span class="sxs-lookup"><span data-stu-id="acada-135">Request</span></span>
<span data-ttu-id="acada-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="acada-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="acada-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="acada-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tabs_in_chat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs/794f0e4e-4d10-4bb5-9079-3a465a629eff
Content-type: application/json
Content-length: 211

{
  "displayName": "My Contoso Tab - updated again"
}
```
# <a name="c"></a>[<span data-ttu-id="acada-138">C#</span><span class="sxs-lookup"><span data-stu-id="acada-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tabs-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="acada-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="acada-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tabs-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="acada-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="acada-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tabs-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="acada-141">Java</span><span class="sxs-lookup"><span data-stu-id="acada-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tabs-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="acada-142">响应</span><span class="sxs-lookup"><span data-stu-id="acada-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsTab"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
  "displayName": "My Contoso Tab - updated again",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": "20",
  "webUrl": "https://teams.microsoft.com/l/entity/com.microsoft.teamspace.tab.web/_djb2_msteams_prefix_193fe248-24e6-478f-a66c-ede9ce6dd547?context=%7b%0d%0a++%22context%22%3a+%22chat%22%2c%0d%0a++%22chatId%22%3a+%2219%3ad65713bc498c4a428c71ef9353e6ce20%40thread.v2%22%2c%0d%0a++%22subEntityId%22%3a+null%0d%0a%7d&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924"
}
```

## <a name="see-also"></a><span data-ttu-id="acada-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="acada-143">See also</span></span>

- [<span data-ttu-id="acada-144">配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="acada-144">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
- [<span data-ttu-id="acada-145">更新频道中的选项卡</span><span class="sxs-lookup"><span data-stu-id="acada-145">Update tab in channel</span></span>](channel-patch-tabs.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update tab in chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


