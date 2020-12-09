---
title: 聊天中的 "获取" 选项卡
description: '检索聊天中指定选项卡的属性和关系。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e85806eaa874a2e09c291354102763f0068ba8cb
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607497"
---
# <a name="get-tab-in-chat"></a><span data-ttu-id="800cf-103">聊天中的 "获取" 选项卡</span><span class="sxs-lookup"><span data-stu-id="800cf-103">Get tab in chat</span></span>

<span data-ttu-id="800cf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="800cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="800cf-105">检索[聊天](../resources/chat.md)中指定[选项卡](../resources/teamstab.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="800cf-105">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md) in a [chat](../resources/chat.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="800cf-106">权限</span><span class="sxs-lookup"><span data-stu-id="800cf-106">Permissions</span></span>
<span data-ttu-id="800cf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="800cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="800cf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="800cf-109">Permission type</span></span>      | <span data-ttu-id="800cf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="800cf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="800cf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="800cf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="800cf-112">TeamsTab，TeamsTab，All，TeamsTab。 All</span><span class="sxs-lookup"><span data-stu-id="800cf-112">TeamsTab.ReadWriteForChat, TeamsTab.Read.All, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="800cf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="800cf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="800cf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="800cf-114">Not supported.</span></span>    |
|<span data-ttu-id="800cf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="800cf-115">Application</span></span> | <span data-ttu-id="800cf-116">TeamsTab，TeamsTab，all，TeamsTab。 All</span><span class="sxs-lookup"><span data-stu-id="800cf-116">TeamsTab.ReadWriteForChat.All, TeamsTab.Read.All, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="800cf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="800cf-117">HTTP request</span></span>
```http
GET /chats/{chat-id}/tabs/{tab-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="800cf-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="800cf-118">Optional query parameters</span></span>

<span data-ttu-id="800cf-119">此方法支持 `$select` 和 `$expand` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="800cf-119">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="800cf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="800cf-120">Request headers</span></span>
| <span data-ttu-id="800cf-121">标头</span><span class="sxs-lookup"><span data-stu-id="800cf-121">Header</span></span>       | <span data-ttu-id="800cf-122">值</span><span class="sxs-lookup"><span data-stu-id="800cf-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="800cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="800cf-123">Authorization</span></span>  | <span data-ttu-id="800cf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="800cf-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="800cf-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="800cf-126">Request body</span></span>
<span data-ttu-id="800cf-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="800cf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="800cf-128">响应</span><span class="sxs-lookup"><span data-stu-id="800cf-128">Response</span></span>

<span data-ttu-id="800cf-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [tab](../resources/teamstab.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="800cf-129">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="800cf-130">示例</span><span class="sxs-lookup"><span data-stu-id="800cf-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="800cf-131">请求</span><span class="sxs-lookup"><span data-stu-id="800cf-131">Request</span></span>
<span data-ttu-id="800cf-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="800cf-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tab_in_chat"
}-->
```http
GET https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d?$expand=teamsApp
```
### <a name="response"></a><span data-ttu-id="800cf-133">响应</span><span class="sxs-lookup"><span data-stu-id="800cf-133">Response</span></span>
<span data-ttu-id="800cf-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="800cf-134">The following is an example of the response.</span></span> 

><span data-ttu-id="800cf-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="800cf-135">**Note:** The response object shown here might be shortened for readability.</span></span> 

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

## <a name="see-also"></a><span data-ttu-id="800cf-136">另请参阅</span><span class="sxs-lookup"><span data-stu-id="800cf-136">See also</span></span>

- [<span data-ttu-id="800cf-137">通道中的获取选项卡</span><span class="sxs-lookup"><span data-stu-id="800cf-137">Get tab in channel</span></span>](channel-get-tabs.md)

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


