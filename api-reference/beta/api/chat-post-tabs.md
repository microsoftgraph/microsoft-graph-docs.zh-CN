---
title: 向聊天添加选项卡
description: '将 (固定) 选项卡添加到指定聊天。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f422823b8646bd695c94640b15f456e3e372e0d5
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971256"
---
# <a name="add-tab-to-chat"></a><span data-ttu-id="7c7cc-103">向聊天添加选项卡</span><span class="sxs-lookup"><span data-stu-id="7c7cc-103">Add tab to chat</span></span>

<span data-ttu-id="7c7cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c7cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c7cc-105">将 (固定) [选项卡](../resources/teamstab.md) 添加到指定的 [聊天中](../resources/chat.md)。</span><span class="sxs-lookup"><span data-stu-id="7c7cc-105">Add (pin) a [tab](../resources/teamstab.md) to the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="7c7cc-106">相应的应用必须已安装 [在聊天 中](../api/chat-list-installedapps.md)。</span><span class="sxs-lookup"><span data-stu-id="7c7cc-106">The corresponding app must already be [installed in the chat](../api/chat-list-installedapps.md).</span></span>

> <span data-ttu-id="7c7cc-107">**注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md) 实例关联，则实际上选项卡将添加到会议。</span><span class="sxs-lookup"><span data-stu-id="7c7cc-107">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the tab will get added to the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c7cc-108">权限</span><span class="sxs-lookup"><span data-stu-id="7c7cc-108">Permissions</span></span>
<span data-ttu-id="7c7cc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c7cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c7cc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c7cc-111">Permission type</span></span>      | <span data-ttu-id="7c7cc-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c7cc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c7cc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c7cc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7c7cc-114">TeamsTab.Create、TeamsTab.ReadWriteForChat、TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c7cc-114">TeamsTab.Create, TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="7c7cc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c7cc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c7cc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c7cc-116">Not supported.</span></span>    |
| <span data-ttu-id="7c7cc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c7cc-117">Application</span></span>                            | <span data-ttu-id="7c7cc-118">TeamsTab.Create.Chat、TeamsTab.ReadWrite.Chat、TeamsTab.Create、TeamsTab.ReadWriteForChat.All、TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c7cc-118">TeamsTab.Create.Chat *, TeamsTab.ReadWrite.Chat*, TeamsTab.Create, TeamsTab.ReadWriteForChat.All, TeamsTab.ReadWrite.All</span></span> |

> <span data-ttu-id="7c7cc-119">**注意**：标有 \* 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="7c7cc-119">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="7c7cc-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c7cc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /chats/{chat-id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="7c7cc-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c7cc-121">Request headers</span></span>
| <span data-ttu-id="7c7cc-122">标头</span><span class="sxs-lookup"><span data-stu-id="7c7cc-122">Header</span></span>       | <span data-ttu-id="7c7cc-123">值</span><span class="sxs-lookup"><span data-stu-id="7c7cc-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7c7cc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c7cc-124">Authorization</span></span>  | <span data-ttu-id="7c7cc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c7cc-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7c7cc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c7cc-127">Request body</span></span>

<span data-ttu-id="7c7cc-128">在请求正文中，包括 [teamsTab](../resources/teamstab.md)的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c7cc-128">In the request body include a JSON representation of a [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="7c7cc-129">响应</span><span class="sxs-lookup"><span data-stu-id="7c7cc-129">Response</span></span>

<span data-ttu-id="7c7cc-130">如果成功，此方法在 `201 Created` 正文中返回 响应代码和 [teamsTab](../resources/teamstab.md) 资源的实例。</span><span class="sxs-lookup"><span data-stu-id="7c7cc-130">If successful, this method returns a `201 Created` response code and an instance of the [teamsTab](../resources/teamstab.md) resource in the body.</span></span>

## <a name="example"></a><span data-ttu-id="7c7cc-131">示例</span><span class="sxs-lookup"><span data-stu-id="7c7cc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c7cc-132">请求</span><span class="sxs-lookup"><span data-stu-id="7c7cc-132">Request</span></span>

<span data-ttu-id="7c7cc-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7c7cc-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7c7cc-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c7cc-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_tab_to_chat"
}
-->

```http
POST https://graph.microsoft.com/beta/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs
Content-Type: application/json

{
  "displayName": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="7c7cc-135">C#</span><span class="sxs-lookup"><span data-stu-id="7c7cc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-tab-to-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c7cc-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c7cc-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-tab-to-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c7cc-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c7cc-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-tab-to-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c7cc-138">Java</span><span class="sxs-lookup"><span data-stu-id="7c7cc-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-tab-to-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7c7cc-139">响应</span><span class="sxs-lookup"><span data-stu-id="7c7cc-139">Response</span></span>

<span data-ttu-id="7c7cc-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7c7cc-140">The following is an example of the response.</span></span> 

><span data-ttu-id="7c7cc-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7c7cc-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsTab"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
  "displayName": "My Contoso Tab",
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

## <a name="see-also"></a><span data-ttu-id="7c7cc-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7c7cc-142">See also</span></span>

- [<span data-ttu-id="7c7cc-143">配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="7c7cc-143">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
- [<span data-ttu-id="7c7cc-144">将选项卡添加到频道</span><span class="sxs-lookup"><span data-stu-id="7c7cc-144">Add tab to channel</span></span>](channel-post-tabs.md)
- [<span data-ttu-id="7c7cc-145">将应用添加到聊天</span><span class="sxs-lookup"><span data-stu-id="7c7cc-145">Add app to chat</span></span>](chat-post-installedapps.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add tab to chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


