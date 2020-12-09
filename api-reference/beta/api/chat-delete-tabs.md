---
title: 从聊天中删除选项卡
description: '从指定的聊天) 选项卡中删除 ("取消固定"。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c83e8c9d1c501b27c46a6df3958008fb4447c06b
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607498"
---
# <a name="delete-tab-from-chat"></a><span data-ttu-id="6bc29-103">从聊天中删除选项卡</span><span class="sxs-lookup"><span data-stu-id="6bc29-103">Delete tab from chat</span></span>

<span data-ttu-id="6bc29-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bc29-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bc29-105">从指定的 [聊天](../resources/chat.md)) 选项卡中删除 ("取消固定"。</span><span class="sxs-lookup"><span data-stu-id="6bc29-105">Remove (unpin) a tab from the specified [chat](../resources/chat.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="6bc29-106">权限</span><span class="sxs-lookup"><span data-stu-id="6bc29-106">Permissions</span></span>
<span data-ttu-id="6bc29-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6bc29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bc29-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6bc29-109">Permission type</span></span>      | <span data-ttu-id="6bc29-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6bc29-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6bc29-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6bc29-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6bc29-112">TeamsTab、ReadWriteForChat、TeamsTab</span><span class="sxs-lookup"><span data-stu-id="6bc29-112">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="6bc29-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6bc29-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bc29-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6bc29-114">Not supported.</span></span>    |
|<span data-ttu-id="6bc29-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6bc29-115">Application</span></span> | <span data-ttu-id="6bc29-116">TeamsTab、ReadWriteForChat、TeamsTab</span><span class="sxs-lookup"><span data-stu-id="6bc29-116">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="6bc29-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6bc29-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /chats/{chat-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="6bc29-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6bc29-118">Request headers</span></span>
| <span data-ttu-id="6bc29-119">标头</span><span class="sxs-lookup"><span data-stu-id="6bc29-119">Header</span></span>       | <span data-ttu-id="6bc29-120">值</span><span class="sxs-lookup"><span data-stu-id="6bc29-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6bc29-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bc29-121">Authorization</span></span>  | <span data-ttu-id="6bc29-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6bc29-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6bc29-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="6bc29-124">Request body</span></span>
<span data-ttu-id="6bc29-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6bc29-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6bc29-126">响应</span><span class="sxs-lookup"><span data-stu-id="6bc29-126">Response</span></span>

<span data-ttu-id="6bc29-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6bc29-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bc29-129">示例</span><span class="sxs-lookup"><span data-stu-id="6bc29-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="6bc29-130">请求</span><span class="sxs-lookup"><span data-stu-id="6bc29-130">Request</span></span>
<span data-ttu-id="6bc29-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6bc29-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tab_in_chat"
}-->
```http
DELETE https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/tabs/d731fca0-0f14-4537-971a-0ef9101ff13d
```
### <a name="response"></a><span data-ttu-id="6bc29-132">响应</span><span class="sxs-lookup"><span data-stu-id="6bc29-132">Response</span></span>
<span data-ttu-id="6bc29-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6bc29-133">The following is an example of the response.</span></span> <span data-ttu-id="6bc29-134">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6bc29-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6bc29-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6bc29-135">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
}
-->

```http
HTTP/1.1 204 No Content
```
## <a name="see-also"></a><span data-ttu-id="6bc29-136">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6bc29-136">See also</span></span>

- [<span data-ttu-id="6bc29-137">从频道中删除选项卡</span><span class="sxs-lookup"><span data-stu-id="6bc29-137">Delete tab from channel</span></span>](channel-delete-tabs.md)

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


