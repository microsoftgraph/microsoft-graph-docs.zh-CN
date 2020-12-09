---
title: 聊天中的更新选项卡
description: 更新聊天中指定选项卡的属性。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e7b8a1bb20b9e80dc8e86768ae5edf3216090287
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607485"
---
# <a name="update-tab-in-chat"></a><span data-ttu-id="98d43-103">聊天中的更新选项卡</span><span class="sxs-lookup"><span data-stu-id="98d43-103">Update tab in chat</span></span>

<span data-ttu-id="98d43-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98d43-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98d43-105">更新[聊天](../resources/chat.md)中指定[选项卡](../resources/teamstab.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="98d43-105">Update the properties of the specified [tab](../resources/teamstab.md) in a [chat](../resources/chat.md).</span></span> <span data-ttu-id="98d43-106">这可用于配置选项卡的内容。</span><span class="sxs-lookup"><span data-stu-id="98d43-106">This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="98d43-107">权限</span><span class="sxs-lookup"><span data-stu-id="98d43-107">Permissions</span></span>
<span data-ttu-id="98d43-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98d43-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="98d43-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="98d43-110">Permission type</span></span>      | <span data-ttu-id="98d43-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="98d43-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98d43-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98d43-112">Delegated (work or school account)</span></span> | <span data-ttu-id="98d43-113">TeamsTab、ReadWriteForChat、TeamsTab</span><span class="sxs-lookup"><span data-stu-id="98d43-113">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="98d43-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98d43-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98d43-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="98d43-115">Not supported.</span></span>    |
|<span data-ttu-id="98d43-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="98d43-116">Application</span></span> | <span data-ttu-id="98d43-117">TeamsTab、ReadWriteForChat、TeamsTab</span><span class="sxs-lookup"><span data-stu-id="98d43-117">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="98d43-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98d43-118">HTTP request</span></span>
```http
PATCH /chats/{chat-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="98d43-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="98d43-119">Request headers</span></span>
| <span data-ttu-id="98d43-120">标头</span><span class="sxs-lookup"><span data-stu-id="98d43-120">Header</span></span>       | <span data-ttu-id="98d43-121">值</span><span class="sxs-lookup"><span data-stu-id="98d43-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="98d43-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="98d43-122">Authorization</span></span>  | <span data-ttu-id="98d43-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="98d43-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="98d43-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="98d43-125">Content-Type</span></span>  | <span data-ttu-id="98d43-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="98d43-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="98d43-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="98d43-128">Request body</span></span>
<span data-ttu-id="98d43-129">在请求正文中，提供 [tab](../resources/teamstab.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98d43-129">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="98d43-130">响应</span><span class="sxs-lookup"><span data-stu-id="98d43-130">Response</span></span>

<span data-ttu-id="98d43-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 **teamsTab** 资源。</span><span class="sxs-lookup"><span data-stu-id="98d43-131">If successful, this method returns a `200 OK` response code and the updated **teamsTab** resource in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="98d43-132">示例</span><span class="sxs-lookup"><span data-stu-id="98d43-132">Examples</span></span>
### <a name="example-1-update-the-name-of-a-tab-in-a-chat"></a><span data-ttu-id="98d43-133">示例1：更新聊天中的选项卡名称</span><span class="sxs-lookup"><span data-stu-id="98d43-133">Example 1: Update the name of a tab in a chat</span></span>

#### <a name="request"></a><span data-ttu-id="98d43-134">请求</span><span class="sxs-lookup"><span data-stu-id="98d43-134">Request</span></span>
<span data-ttu-id="98d43-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="98d43-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tabs_in_chat"
}-->
```http
PATCH https://graph.microsoft.com/beta/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs/794f0e4e-4d10-4bb5-9079-3a465a629eff
Content-type: application/json
Content-length: 211

{
  "displayName": "My Contoso Tab - updated again"
}
```
#### <a name="response"></a><span data-ttu-id="98d43-136">响应</span><span class="sxs-lookup"><span data-stu-id="98d43-136">Response</span></span>

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

## <a name="see-also"></a><span data-ttu-id="98d43-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="98d43-137">See also</span></span>

- [<span data-ttu-id="98d43-138">配置内置选项卡类型</span><span class="sxs-lookup"><span data-stu-id="98d43-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
- [<span data-ttu-id="98d43-139">通道中的 "更新" 选项卡</span><span class="sxs-lookup"><span data-stu-id="98d43-139">Update tab in channel</span></span>](channel-patch-tabs.md)

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


