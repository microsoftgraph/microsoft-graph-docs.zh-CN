---
title: 从聊天删除成员
description: 从聊天删除 conversationMember。
author: AkJo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f1ed1c4b461bebf3bcef1e5e3a4149a043dad30e
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714353"
---
# <a name="remove-member-from-chat"></a><span data-ttu-id="efe21-103">从聊天删除成员</span><span class="sxs-lookup"><span data-stu-id="efe21-103">Remove member from chat</span></span>
<span data-ttu-id="efe21-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efe21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efe21-105">从[聊天](../resources/chat.md)中删除 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="efe21-105">Remove a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="efe21-106">权限</span><span class="sxs-lookup"><span data-stu-id="efe21-106">Permissions</span></span>
<span data-ttu-id="efe21-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="efe21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efe21-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="efe21-109">Permission type</span></span>|<span data-ttu-id="efe21-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="efe21-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efe21-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efe21-111">Delegated (work or school account)</span></span>| <span data-ttu-id="efe21-112">ChatMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efe21-112">ChatMember.ReadWrite.All</span></span> |
|<span data-ttu-id="efe21-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efe21-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efe21-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="efe21-114">Not supported.</span></span>    |
|<span data-ttu-id="efe21-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="efe21-115">Application</span></span>| <span data-ttu-id="efe21-116">ChatMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efe21-116">ChatMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="efe21-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efe21-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /chats/{chat-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="efe21-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="efe21-118">Request headers</span></span>
|<span data-ttu-id="efe21-119">名称</span><span class="sxs-lookup"><span data-stu-id="efe21-119">Name</span></span>|<span data-ttu-id="efe21-120">说明</span><span class="sxs-lookup"><span data-stu-id="efe21-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="efe21-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="efe21-121">Authorization</span></span>|<span data-ttu-id="efe21-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="efe21-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="efe21-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="efe21-124">Request body</span></span>
<span data-ttu-id="efe21-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="efe21-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efe21-126">响应</span><span class="sxs-lookup"><span data-stu-id="efe21-126">Response</span></span>

<span data-ttu-id="efe21-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="efe21-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="efe21-128">示例</span><span class="sxs-lookup"><span data-stu-id="efe21-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="efe21-129">请求</span><span class="sxs-lookup"><span data-stu-id="efe21-129">Request</span></span>

> [!NOTE]
> <span data-ttu-id="efe21-130">此功能存在一些已知问题。</span><span class="sxs-lookup"><span data-stu-id="efe21-130">There are some known issues with this functionality.</span></span> <span data-ttu-id="efe21-131">有关详细信息，请参阅[已知问题](/graph/known-issues.md#unable-to-remove-members-from-chat)。</span><span class="sxs-lookup"><span data-stu-id="efe21-131">For details, see [known issues](/graph/known-issues.md#unable-to-remove-members-from-chat).</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_members_from_chat"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```

### <a name="response"></a><span data-ttu-id="efe21-132">响应</span><span class="sxs-lookup"><span data-stu-id="efe21-132">Response</span></span>
<span data-ttu-id="efe21-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="efe21-133">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="efe21-134">另请参阅</span><span class="sxs-lookup"><span data-stu-id="efe21-134">See also</span></span>

- [<span data-ttu-id="efe21-135">从频道中删除成员</span><span class="sxs-lookup"><span data-stu-id="efe21-135">Remove member from channel</span></span>](channel-delete-members.md)
- [<span data-ttu-id="efe21-136">从团队删除成员</span><span class="sxs-lookup"><span data-stu-id="efe21-136">Remove member from team</span></span>](team-delete-members.md)

