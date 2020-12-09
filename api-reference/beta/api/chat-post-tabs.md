---
title: 将选项卡添加到聊天
description: '将选项卡上 (插针添加到指定的聊天) 。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6182daa44d0e5ac8deb86a1fb8fe61c5f1376b2f
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607489"
---
# <a name="add-tab-to-chat"></a><span data-ttu-id="70710-103">将选项卡添加到聊天</span><span class="sxs-lookup"><span data-stu-id="70710-103">Add tab to chat</span></span>

<span data-ttu-id="70710-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70710-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70710-105">将 [选项卡上](../resources/teamstab.md) (pin 添加) 到指定的 [聊天](../resources/chat.md)中。</span><span class="sxs-lookup"><span data-stu-id="70710-105">Add (pin) a [tab](../resources/teamstab.md) to the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="70710-106">必须已 [在聊天中安装](../api/chat-list-installedapps.md)相应的应用程序。</span><span class="sxs-lookup"><span data-stu-id="70710-106">The corresponding app must already be [installed in the chat](../api/chat-list-installedapps.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="70710-107">权限</span><span class="sxs-lookup"><span data-stu-id="70710-107">Permissions</span></span>
<span data-ttu-id="70710-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70710-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70710-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="70710-110">Permission type</span></span>      | <span data-ttu-id="70710-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70710-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70710-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70710-112">Delegated (work or school account)</span></span> | <span data-ttu-id="70710-113">TeamsTab、TeamsTab、ReadWriteForChat、TeamsTab。</span><span class="sxs-lookup"><span data-stu-id="70710-113">TeamsTab.Create, TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="70710-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70710-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70710-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="70710-115">Not supported.</span></span>    |
| <span data-ttu-id="70710-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="70710-116">Application</span></span>                            | <span data-ttu-id="70710-117">TeamsTab、TeamsTab、ReadWriteForChat、All。</span><span class="sxs-lookup"><span data-stu-id="70710-117">TeamsTab.Create, TeamsTab.ReadWriteForChat.All, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="70710-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70710-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /chats/{chat-id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="70710-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="70710-119">Request headers</span></span>
| <span data-ttu-id="70710-120">标头</span><span class="sxs-lookup"><span data-stu-id="70710-120">Header</span></span>       | <span data-ttu-id="70710-121">值</span><span class="sxs-lookup"><span data-stu-id="70710-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="70710-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="70710-122">Authorization</span></span>  | <span data-ttu-id="70710-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="70710-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="70710-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="70710-125">Request body</span></span>

<span data-ttu-id="70710-126">在请求正文中，包含 [teamsTab](../resources/teamstab.md)的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70710-126">In the request body include a JSON representation of a [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="70710-127">响应</span><span class="sxs-lookup"><span data-stu-id="70710-127">Response</span></span>

<span data-ttu-id="70710-128">如果成功，此方法 `201 Created` 在正文中返回响应代码和 [teamsTab](../resources/teamstab.md) 资源的实例。</span><span class="sxs-lookup"><span data-stu-id="70710-128">If successful, this method returns a `201 Created` response code and an instance of the [teamsTab](../resources/teamstab.md) resource in the body.</span></span>

## <a name="example"></a><span data-ttu-id="70710-129">示例</span><span class="sxs-lookup"><span data-stu-id="70710-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="70710-130">请求</span><span class="sxs-lookup"><span data-stu-id="70710-130">Request</span></span>

<span data-ttu-id="70710-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="70710-131">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="70710-132">响应</span><span class="sxs-lookup"><span data-stu-id="70710-132">Response</span></span>

<span data-ttu-id="70710-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="70710-133">The following is an example of the response.</span></span> 

><span data-ttu-id="70710-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="70710-134">**Note:** The response object shown here might be shortened for readability.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="70710-135">另请参阅</span><span class="sxs-lookup"><span data-stu-id="70710-135">See also</span></span>

- [<span data-ttu-id="70710-136">配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="70710-136">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
- [<span data-ttu-id="70710-137">将选项卡添加到频道</span><span class="sxs-lookup"><span data-stu-id="70710-137">Add tab to channel</span></span>](channel-post-tabs.md)
- [<span data-ttu-id="70710-138">将应用程序添加到聊天</span><span class="sxs-lookup"><span data-stu-id="70710-138">Add app to chat</span></span>](chat-post-installedapps.md)


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


