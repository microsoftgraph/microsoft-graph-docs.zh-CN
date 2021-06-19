---
title: 获取 teamsAsyncOperation
description: 获取 teamsAsyncOperation 的详细信息。
author: jecha
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1b0451a481c51986fcf62c922fd24df0197e8fdd
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031482"
---
# <a name="get-teamsasyncoperation"></a><span data-ttu-id="3eca6-103">获取 teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="3eca6-103">Get teamsAsyncOperation</span></span>
<span data-ttu-id="3eca6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3eca6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3eca6-105">获取特定[Teams运行或](../resources/teamsasyncoperation.md)运行的指定异步操作。</span><span class="sxs-lookup"><span data-stu-id="3eca6-105">Get the specified [Teams async operation](../resources/teamsasyncoperation.md) that ran or is running on a specific resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="3eca6-106">权限</span><span class="sxs-lookup"><span data-stu-id="3eca6-106">Permissions</span></span>
<span data-ttu-id="3eca6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3eca6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3eca6-109">以下权限用于获取聊天上的操作：</span><span class="sxs-lookup"><span data-stu-id="3eca6-109">The following permissions are for getting the operation on a chat:</span></span>

| <span data-ttu-id="3eca6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3eca6-110">Permission type</span></span>                        | <span data-ttu-id="3eca6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3eca6-111">Permissions (from least to most privileged)</span></span>|
| :------------------------------------- | :--------------------------------------------------- |
| <span data-ttu-id="3eca6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3eca6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3eca6-113">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3eca6-113">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span>|
| <span data-ttu-id="3eca6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3eca6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3eca6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3eca6-115">Not supported.</span></span> |
| <span data-ttu-id="3eca6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3eca6-116">Application</span></span>                            | <span data-ttu-id="3eca6-117">ChatSettings.Read.Chat *、ChatSettings.ReadWrite.Chat*、Chat.Manage.Chat\*、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eca6-117">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |

> <span data-ttu-id="3eca6-118">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="3eca6-118">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="3eca6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3eca6-119">HTTP request</span></span>
<!-- { 
    "blockType": "ignored" 
} 
-->
``` http
GET /chats/{chat-id}/operations/{operation-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3eca6-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3eca6-120">Optional query parameters</span></span>

<span data-ttu-id="3eca6-121">此方法支持 `$select` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3eca6-121">This method supports the `$select` [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3eca6-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="3eca6-122">Request headers</span></span>

|<span data-ttu-id="3eca6-123">名称</span><span class="sxs-lookup"><span data-stu-id="3eca6-123">Name</span></span>|<span data-ttu-id="3eca6-124">说明</span><span class="sxs-lookup"><span data-stu-id="3eca6-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3eca6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3eca6-125">Authorization</span></span>|<span data-ttu-id="3eca6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3eca6-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3eca6-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3eca6-128">Request body</span></span>

<span data-ttu-id="3eca6-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3eca6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3eca6-130">响应</span><span class="sxs-lookup"><span data-stu-id="3eca6-130">Response</span></span>

<span data-ttu-id="3eca6-131">如果成功，这将在响应 `200 OK` 正文中返回 响应代码和 [teamsAsyncOperation](../resources/teamsasyncoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3eca6-131">If successful, this returns a `200 OK` response code and a [teamsAsyncOperation](../resources/teamsasyncoperation.md) object in the response body.</span></span>

## <a name="example-get-operation-on-chat"></a><span data-ttu-id="3eca6-132">示例：获取聊天操作</span><span class="sxs-lookup"><span data-stu-id="3eca6-132">Example: Get operation on chat</span></span>

### <a name="request"></a><span data-ttu-id="3eca6-133">请求</span><span class="sxs-lookup"><span data-stu-id="3eca6-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chat_operation"
}
-->
``` http
GET https://graph.microsoft.com/beta/chats/19:c253a29b5f694b55a6baad8e83510af7@thread.v2/operations/2432b57b-0abd-43db-aa7b-16eadd115d34-e88ae9aa-887e-4972-ac3e-bd578e38232e-cf58835e-43f0-4fc1-825e-5de55630e7e4
```

### <a name="response"></a><span data-ttu-id="3eca6-134">响应</span><span class="sxs-lookup"><span data-stu-id="3eca6-134">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsAsyncOperation"
}
-->
``` http
HTTP/1.1 202 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ac253a29b5f694b55a6baad8e83510af7%40thread.v2')/operations/$entity",
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
```
