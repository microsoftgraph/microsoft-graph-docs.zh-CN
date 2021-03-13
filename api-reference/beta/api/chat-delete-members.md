---
title: 从聊天删除成员
description: 从聊天删除 conversationMember。
author: AkJo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d8696bbf255621f226409e3e91c4d6b0194f88cc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775904"
---
# <a name="remove-member-from-chat"></a><span data-ttu-id="5d03f-103">从聊天删除成员</span><span class="sxs-lookup"><span data-stu-id="5d03f-103">Remove member from chat</span></span>
<span data-ttu-id="5d03f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d03f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d03f-105">从[聊天](../resources/chat.md)中删除 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="5d03f-105">Remove a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5d03f-106">权限</span><span class="sxs-lookup"><span data-stu-id="5d03f-106">Permissions</span></span>
<span data-ttu-id="5d03f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d03f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d03f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d03f-109">Permission type</span></span>|<span data-ttu-id="5d03f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d03f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d03f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d03f-111">Delegated (work or school account)</span></span>| <span data-ttu-id="5d03f-112">ChatMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d03f-112">ChatMember.ReadWrite.All</span></span> |
|<span data-ttu-id="5d03f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d03f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d03f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d03f-114">Not supported.</span></span>    |
|<span data-ttu-id="5d03f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d03f-115">Application</span></span>| <span data-ttu-id="5d03f-116">ChatMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d03f-116">ChatMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d03f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d03f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /chats/{chat-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="5d03f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d03f-118">Request headers</span></span>
|<span data-ttu-id="5d03f-119">名称</span><span class="sxs-lookup"><span data-stu-id="5d03f-119">Name</span></span>|<span data-ttu-id="5d03f-120">说明</span><span class="sxs-lookup"><span data-stu-id="5d03f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5d03f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d03f-121">Authorization</span></span>|<span data-ttu-id="5d03f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5d03f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d03f-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d03f-124">Request body</span></span>
<span data-ttu-id="5d03f-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5d03f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d03f-126">响应</span><span class="sxs-lookup"><span data-stu-id="5d03f-126">Response</span></span>

<span data-ttu-id="5d03f-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5d03f-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5d03f-128">示例</span><span class="sxs-lookup"><span data-stu-id="5d03f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5d03f-129">请求</span><span class="sxs-lookup"><span data-stu-id="5d03f-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5d03f-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d03f-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_chat"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```
# <a name="c"></a>[<span data-ttu-id="5d03f-131">C#</span><span class="sxs-lookup"><span data-stu-id="5d03f-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-members-from-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d03f-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d03f-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-members-from-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d03f-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d03f-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-members-from-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d03f-134">Java</span><span class="sxs-lookup"><span data-stu-id="5d03f-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-members-from-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5d03f-135">响应</span><span class="sxs-lookup"><span data-stu-id="5d03f-135">Response</span></span>
<span data-ttu-id="5d03f-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5d03f-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="5d03f-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5d03f-137">See also</span></span>

- [<span data-ttu-id="5d03f-138">从频道中删除成员</span><span class="sxs-lookup"><span data-stu-id="5d03f-138">Remove member from channel</span></span>](channel-delete-members.md)
- [<span data-ttu-id="5d03f-139">从团队删除成员</span><span class="sxs-lookup"><span data-stu-id="5d03f-139">Remove member from team</span></span>](team-delete-members.md)

