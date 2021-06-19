---
title: 列出聊天操作
description: 检索聊天操作。
author: jecha
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fce94d591d6d1bde1e15f78674b18623ba80cb33
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031449"
---
# <a name="list-operations-on-a-chat"></a><span data-ttu-id="72d2e-103">列出聊天操作</span><span class="sxs-lookup"><span data-stu-id="72d2e-103">List operations on a chat</span></span>
<span data-ttu-id="72d2e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72d2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72d2e-105">列出Teams[聊天](../resources/teamsasyncoperation.md)中运行或运行的异步操作[的所有异步操作](../resources/chat.md)。</span><span class="sxs-lookup"><span data-stu-id="72d2e-105">List all [Teams async operations](../resources/teamsasyncoperation.md) that ran or are running on the specified [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="72d2e-106">权限</span><span class="sxs-lookup"><span data-stu-id="72d2e-106">Permissions</span></span>
<span data-ttu-id="72d2e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72d2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72d2e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="72d2e-109">Permission type</span></span>                        | <span data-ttu-id="72d2e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="72d2e-110">Permissions (from least to most privileged)</span></span>|
| :------------------------------------- | :--------------------------------------------------- |
| <span data-ttu-id="72d2e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72d2e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="72d2e-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72d2e-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span>|
| <span data-ttu-id="72d2e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72d2e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72d2e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="72d2e-114">Not supported.</span></span> |
| <span data-ttu-id="72d2e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="72d2e-115">Application</span></span>                            | <span data-ttu-id="72d2e-116">ChatSettings.Read.Chat *、ChatSettings.ReadWrite.Chat*、Chat.Manage.Chat\*、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72d2e-116">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |

> <span data-ttu-id="72d2e-117">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="72d2e-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="72d2e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72d2e-118">HTTP request</span></span>
<!-- { 
    "blockType": "ignored" 
} 
-->
``` http
GET /chats/{chat-id}/operations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72d2e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="72d2e-119">Optional query parameters</span></span>

<span data-ttu-id="72d2e-120">此方法支持 `$filter` 、 `$select` 、 和 `$top` `$skip` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="72d2e-120">This method supports the `$filter`, `$select`, `$top`, and `$skip` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72d2e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="72d2e-121">Request headers</span></span>

|<span data-ttu-id="72d2e-122">名称</span><span class="sxs-lookup"><span data-stu-id="72d2e-122">Name</span></span>|<span data-ttu-id="72d2e-123">说明</span><span class="sxs-lookup"><span data-stu-id="72d2e-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="72d2e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="72d2e-124">Authorization</span></span>|<span data-ttu-id="72d2e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="72d2e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="72d2e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="72d2e-127">Request body</span></span>

<span data-ttu-id="72d2e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="72d2e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72d2e-129">响应</span><span class="sxs-lookup"><span data-stu-id="72d2e-129">Response</span></span>

<span data-ttu-id="72d2e-130">如果成功，这将在响应正文中返回 响应代码和 `200 OK` [teamsAsyncOperation](../resources/teamsasyncoperation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="72d2e-130">If successful, this returns a `200 OK` response code and a collection of [teamsAsyncOperation](../resources/teamsasyncoperation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72d2e-131">示例</span><span class="sxs-lookup"><span data-stu-id="72d2e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72d2e-132">请求</span><span class="sxs-lookup"><span data-stu-id="72d2e-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_chat_operations"
}
-->
``` http
GET https://graph.microsoft.com/beta/chats/19:c253a29b5f694b55a6baad8e83510af7@thread.v2/operations
```

---

### <a name="response"></a><span data-ttu-id="72d2e-133">响应</span><span class="sxs-lookup"><span data-stu-id="72d2e-133">Response</span></span>
><span data-ttu-id="72d2e-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="72d2e-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAsyncOperation",
  "isCollection": true
}
-->
``` http
HTTP/1.1 202 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ac253a29b5f694b55a6baad8e83510af7%40thread.v2')/operations",
    "@odata.count": 1,
    "value": [
        {
            "id": "2432b57b-0abd-43db-aa7b-16eadd115d34-e88ae9aa-887e-4972-ac3e-bd578e38232e-cf58835e-43f0-4fc1-825e-5de55630e7e4",
            "operationType": "createChat",
            "createdDateTime": "2021-05-27T21:23:41.9085453Z",
            "status": "succeeded",
            "lastActionDateTime": "2021-05-27T21:23:45.1899277Z",
            "attemptsCount": 1,
            "targetResourceId": "19:c253a29b5f694b55a6baad8e83510af7@thread.v2",
            "targetResourceLocation": "/chats('19:c253a29b5f694b55a6baad8e83510af7@thread.v2')",
            "values": "{\"appIds\":[\"1542629c-01b3-4a6d-8f76-1938b779e48d\"]}",
            "error": null
        }
    ]
}
```
