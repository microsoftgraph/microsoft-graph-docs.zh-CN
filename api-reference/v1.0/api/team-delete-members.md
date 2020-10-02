---
title: 从团队删除成员
description: 从团队删除 conversationMember。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e132e5b15affb2ba649dd84818d595b69c8269e4
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330320"
---
# <a name="remove-members-from-team"></a><span data-ttu-id="ec5f7-103">从团队删除成员</span><span class="sxs-lookup"><span data-stu-id="ec5f7-103">Remove members from team</span></span>
<span data-ttu-id="ec5f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec5f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ec5f7-105">从 [team](../resources/team.md) 删除新的 [conversationMember](../resources/conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="ec5f7-105">Remove a new [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ec5f7-106">权限</span><span class="sxs-lookup"><span data-stu-id="ec5f7-106">Permissions</span></span>
<span data-ttu-id="ec5f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec5f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec5f7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec5f7-109">Permission type</span></span>|<span data-ttu-id="ec5f7-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ec5f7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec5f7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec5f7-111">Delegated (work or school account)</span></span>| <span data-ttu-id="ec5f7-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec5f7-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="ec5f7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec5f7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec5f7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec5f7-114">Not supported.</span></span>    |
|<span data-ttu-id="ec5f7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec5f7-115">Application</span></span>| <span data-ttu-id="ec5f7-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec5f7-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec5f7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec5f7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-id}/members/{membership-id}
DELETE /teams/{team-id}/channels/{channel-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="ec5f7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec5f7-118">Request headers</span></span>
|<span data-ttu-id="ec5f7-119">名称</span><span class="sxs-lookup"><span data-stu-id="ec5f7-119">Name</span></span>|<span data-ttu-id="ec5f7-120">说明</span><span class="sxs-lookup"><span data-stu-id="ec5f7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ec5f7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec5f7-121">Authorization</span></span>|<span data-ttu-id="ec5f7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ec5f7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec5f7-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec5f7-124">Request body</span></span>
<span data-ttu-id="ec5f7-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ec5f7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec5f7-126">响应</span><span class="sxs-lookup"><span data-stu-id="ec5f7-126">Response</span></span>

<span data-ttu-id="ec5f7-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ec5f7-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ec5f7-128">示例</span><span class="sxs-lookup"><span data-stu-id="ec5f7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ec5f7-129">请求</span><span class="sxs-lookup"><span data-stu-id="ec5f7-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ec5f7-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec5f7-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/teams/{teamsId}/members/{membership-id}
```
# <a name="c"></a>[<span data-ttu-id="ec5f7-131">C#</span><span class="sxs-lookup"><span data-stu-id="ec5f7-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-members-from-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec5f7-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec5f7-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-members-from-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec5f7-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec5f7-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-members-from-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec5f7-134">Java</span><span class="sxs-lookup"><span data-stu-id="ec5f7-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-members-from-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ec5f7-135">响应</span><span class="sxs-lookup"><span data-stu-id="ec5f7-135">Response</span></span>
<span data-ttu-id="ec5f7-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ec5f7-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
