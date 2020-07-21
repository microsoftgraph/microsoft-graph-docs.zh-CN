---
title: 从团队删除成员
description: 从团队删除 conversationMember。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0e81527c98ea20161db62516827d82c48c2706d2
ms.sourcegitcommit: 79267b6d78c3510ef609953c5a664e692794caaa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/21/2020
ms.locfileid: "45197028"
---
# <a name="delete-members"></a><span data-ttu-id="56d3f-103">删除成员</span><span class="sxs-lookup"><span data-stu-id="56d3f-103">Delete members</span></span>
<span data-ttu-id="56d3f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56d3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56d3f-105">从 [team](../resources/team.md) 删除新的 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="56d3f-105">Remove a new [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="56d3f-106">权限</span><span class="sxs-lookup"><span data-stu-id="56d3f-106">Permissions</span></span>
<span data-ttu-id="56d3f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56d3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56d3f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="56d3f-109">Permission type</span></span>|<span data-ttu-id="56d3f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="56d3f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56d3f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56d3f-111">Delegated (work or school account)</span></span>| <span data-ttu-id="56d3f-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56d3f-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="56d3f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56d3f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56d3f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="56d3f-114">Not supported.</span></span>    |
|<span data-ttu-id="56d3f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="56d3f-115">Application</span></span>| <span data-ttu-id="56d3f-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56d3f-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56d3f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56d3f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="56d3f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="56d3f-118">Request headers</span></span>
|<span data-ttu-id="56d3f-119">名称</span><span class="sxs-lookup"><span data-stu-id="56d3f-119">Name</span></span>|<span data-ttu-id="56d3f-120">说明</span><span class="sxs-lookup"><span data-stu-id="56d3f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="56d3f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="56d3f-121">Authorization</span></span>|<span data-ttu-id="56d3f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="56d3f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="56d3f-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="56d3f-124">Request body</span></span>
<span data-ttu-id="56d3f-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="56d3f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56d3f-126">响应</span><span class="sxs-lookup"><span data-stu-id="56d3f-126">Response</span></span>

<span data-ttu-id="56d3f-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="56d3f-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="56d3f-128">示例</span><span class="sxs-lookup"><span data-stu-id="56d3f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="56d3f-129">请求</span><span class="sxs-lookup"><span data-stu-id="56d3f-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="56d3f-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="56d3f-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/{teamsId}/members/{membership-id}
```
# <a name="c"></a>[<span data-ttu-id="56d3f-131">C#</span><span class="sxs-lookup"><span data-stu-id="56d3f-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-members-from-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56d3f-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56d3f-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-members-from-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56d3f-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56d3f-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-members-from-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="56d3f-134">响应</span><span class="sxs-lookup"><span data-stu-id="56d3f-134">Response</span></span>
<span data-ttu-id="56d3f-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="56d3f-135">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

