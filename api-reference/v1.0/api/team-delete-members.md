---
title: 从团队删除成员
description: 从团队删除 conversationMember。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0e98aed4edc959314473d645934e8e8bfbba1143
ms.sourcegitcommit: 3c0fa2d13ede0fdfa66d966d4ec32cb468c3befa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/25/2020
ms.locfileid: "48273688"
---
# <a name="remove-members-from-team"></a><span data-ttu-id="65740-103">从团队删除成员</span><span class="sxs-lookup"><span data-stu-id="65740-103">Remove members from team</span></span>
<span data-ttu-id="65740-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65740-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="65740-105">从 [team](../resources/team.md) 删除新的 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="65740-105">Remove a new [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="65740-106">权限</span><span class="sxs-lookup"><span data-stu-id="65740-106">Permissions</span></span>
<span data-ttu-id="65740-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65740-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65740-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="65740-109">Permission type</span></span>|<span data-ttu-id="65740-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="65740-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65740-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65740-111">Delegated (work or school account)</span></span>| <span data-ttu-id="65740-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65740-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="65740-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65740-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65740-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="65740-114">Not supported.</span></span>    |
|<span data-ttu-id="65740-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="65740-115">Application</span></span>| <span data-ttu-id="65740-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65740-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65740-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65740-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="65740-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="65740-118">Request headers</span></span>
|<span data-ttu-id="65740-119">名称</span><span class="sxs-lookup"><span data-stu-id="65740-119">Name</span></span>|<span data-ttu-id="65740-120">说明</span><span class="sxs-lookup"><span data-stu-id="65740-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="65740-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="65740-121">Authorization</span></span>|<span data-ttu-id="65740-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="65740-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65740-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="65740-124">Request body</span></span>
<span data-ttu-id="65740-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="65740-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65740-126">响应</span><span class="sxs-lookup"><span data-stu-id="65740-126">Response</span></span>

<span data-ttu-id="65740-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="65740-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="65740-128">示例</span><span class="sxs-lookup"><span data-stu-id="65740-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="65740-129">请求</span><span class="sxs-lookup"><span data-stu-id="65740-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="65740-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="65740-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/teams/{teamsId}/members/{membership-id}
```
# <a name="c"></a>[<span data-ttu-id="65740-131">C#</span><span class="sxs-lookup"><span data-stu-id="65740-131">C#</span></span>](#tab/csharp)

[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65740-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65740-132">JavaScript</span></span>](#tab/javascript)

[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65740-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65740-133">Objective-C</span></span>](#tab/objc)

[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="65740-134">响应</span><span class="sxs-lookup"><span data-stu-id="65740-134">Response</span></span>
<span data-ttu-id="65740-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="65740-135">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
