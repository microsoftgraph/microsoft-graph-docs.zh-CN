---
title: 从聊天删除成员
description: 从聊天删除 conversationMember。
author: AkJo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 82fd2908a15991ae96fb0d50285d82fbcec7cdea
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777592"
---
# <a name="remove-member-from-chat"></a><span data-ttu-id="2b6f9-103">从聊天删除成员</span><span class="sxs-lookup"><span data-stu-id="2b6f9-103">Remove member from chat</span></span>
<span data-ttu-id="2b6f9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b6f9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2b6f9-105">从[聊天](../resources/chat.md)中删除 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="2b6f9-105">Remove a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2b6f9-106">权限</span><span class="sxs-lookup"><span data-stu-id="2b6f9-106">Permissions</span></span>
<span data-ttu-id="2b6f9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b6f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b6f9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b6f9-109">Permission type</span></span>|<span data-ttu-id="2b6f9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b6f9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b6f9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b6f9-111">Delegated (work or school account)</span></span>| <span data-ttu-id="2b6f9-112">ChatMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b6f9-112">ChatMember.ReadWrite.All</span></span> |
|<span data-ttu-id="2b6f9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b6f9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b6f9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b6f9-114">Not supported.</span></span>    |
|<span data-ttu-id="2b6f9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b6f9-115">Application</span></span>| <span data-ttu-id="2b6f9-116">ChatMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b6f9-116">ChatMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b6f9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b6f9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /chats/{chat-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="2b6f9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b6f9-118">Request headers</span></span>
|<span data-ttu-id="2b6f9-119">名称</span><span class="sxs-lookup"><span data-stu-id="2b6f9-119">Name</span></span>|<span data-ttu-id="2b6f9-120">说明</span><span class="sxs-lookup"><span data-stu-id="2b6f9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2b6f9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b6f9-121">Authorization</span></span>|<span data-ttu-id="2b6f9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b6f9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b6f9-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b6f9-124">Request body</span></span>
<span data-ttu-id="2b6f9-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2b6f9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b6f9-126">响应</span><span class="sxs-lookup"><span data-stu-id="2b6f9-126">Response</span></span>

<span data-ttu-id="2b6f9-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2b6f9-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2b6f9-128">示例</span><span class="sxs-lookup"><span data-stu-id="2b6f9-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2b6f9-129">请求</span><span class="sxs-lookup"><span data-stu-id="2b6f9-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_members_from_chat"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```


### <a name="response"></a><span data-ttu-id="2b6f9-130">响应</span><span class="sxs-lookup"><span data-stu-id="2b6f9-130">Response</span></span>
<span data-ttu-id="2b6f9-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2b6f9-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="2b6f9-132">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2b6f9-132">See also</span></span>

- [<span data-ttu-id="2b6f9-133">从频道中删除成员</span><span class="sxs-lookup"><span data-stu-id="2b6f9-133">Remove member from channel</span></span>](channel-delete-members.md)
- [<span data-ttu-id="2b6f9-134">从团队删除成员</span><span class="sxs-lookup"><span data-stu-id="2b6f9-134">Remove member from team</span></span>](team-delete-members.md)

