---
title: 从聊天中删除选项卡
description: '从 (聊天) 取消固定选项卡。 '
author: subray
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 70fb781618c094406948b52e4c8068163ad1808e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777585"
---
# <a name="delete-tab-from-chat"></a><span data-ttu-id="b6a21-103">从聊天中删除选项卡</span><span class="sxs-lookup"><span data-stu-id="b6a21-103">Delete tab from chat</span></span>

<span data-ttu-id="b6a21-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6a21-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b6a21-105">从 (聊天) 取消固定[选项卡。](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="b6a21-105">Remove (unpin) a tab from the specified [chat](../resources/chat.md).</span></span> 

> <span data-ttu-id="b6a21-106">**注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md) 实例关联，则实际上选项卡将从会议中删除。</span><span class="sxs-lookup"><span data-stu-id="b6a21-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the tab will get removed from the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6a21-107">权限</span><span class="sxs-lookup"><span data-stu-id="b6a21-107">Permissions</span></span>
<span data-ttu-id="b6a21-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b6a21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6a21-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6a21-110">Permission type</span></span>      | <span data-ttu-id="b6a21-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b6a21-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6a21-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6a21-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b6a21-113">TeamsTab.ReadWriteForChat、TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6a21-113">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="b6a21-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6a21-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6a21-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6a21-115">Not supported.</span></span>    |
|<span data-ttu-id="b6a21-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6a21-116">Application</span></span> | <span data-ttu-id="b6a21-117">TeamsTab.ReadWriteForChat、TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6a21-117">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="b6a21-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6a21-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /chats/{chat-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="b6a21-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6a21-119">Request headers</span></span>
| <span data-ttu-id="b6a21-120">标头</span><span class="sxs-lookup"><span data-stu-id="b6a21-120">Header</span></span>       | <span data-ttu-id="b6a21-121">值</span><span class="sxs-lookup"><span data-stu-id="b6a21-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b6a21-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6a21-122">Authorization</span></span>  | <span data-ttu-id="b6a21-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b6a21-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b6a21-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6a21-125">Request body</span></span>
<span data-ttu-id="b6a21-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b6a21-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6a21-127">响应</span><span class="sxs-lookup"><span data-stu-id="b6a21-127">Response</span></span>

<span data-ttu-id="b6a21-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b6a21-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6a21-130">示例</span><span class="sxs-lookup"><span data-stu-id="b6a21-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6a21-131">请求</span><span class="sxs-lookup"><span data-stu-id="b6a21-131">Request</span></span>
<span data-ttu-id="b6a21-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b6a21-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_tab_in_chat"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d
```


### <a name="response"></a><span data-ttu-id="b6a21-133">响应</span><span class="sxs-lookup"><span data-stu-id="b6a21-133">Response</span></span>
<span data-ttu-id="b6a21-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b6a21-134">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
}
-->

```http
HTTP/1.1 204 No Content
```
## <a name="see-also"></a><span data-ttu-id="b6a21-135">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b6a21-135">See also</span></span>

- [<span data-ttu-id="b6a21-136">从频道中删除选项卡</span><span class="sxs-lookup"><span data-stu-id="b6a21-136">Delete tab from channel</span></span>](channel-delete-tabs.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete tab from chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


