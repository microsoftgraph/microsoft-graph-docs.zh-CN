---
title: 从团队中移除成员
description: 从团队中删除 conversationMember。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2dc5359684f0b4d73f08551ea720dc095f482337
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091443"
---
# <a name="delete-members"></a><span data-ttu-id="64b35-103">删除成员</span><span class="sxs-lookup"><span data-stu-id="64b35-103">Delete members</span></span>
<span data-ttu-id="64b35-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64b35-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64b35-105">从[团队](../resources/team.md)中删除新的[conversationMember](../resources/conversationmember.md) 。</span><span class="sxs-lookup"><span data-stu-id="64b35-105">Remove a new [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="64b35-106">权限</span><span class="sxs-lookup"><span data-stu-id="64b35-106">Permissions</span></span>
<span data-ttu-id="64b35-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="64b35-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="64b35-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64b35-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64b35-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="64b35-109">Permission type</span></span>|<span data-ttu-id="64b35-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="64b35-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64b35-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64b35-111">Delegated (work or school account)</span></span>| <span data-ttu-id="64b35-112">TeamMember</span><span class="sxs-lookup"><span data-stu-id="64b35-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="64b35-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64b35-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64b35-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="64b35-114">Not supported.</span></span>    |
|<span data-ttu-id="64b35-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="64b35-115">Application</span></span>| <span data-ttu-id="64b35-116">TeamMember</span><span class="sxs-lookup"><span data-stu-id="64b35-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64b35-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64b35-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-id}/members/{member-id}
```

## <a name="request-headers"></a><span data-ttu-id="64b35-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="64b35-118">Request headers</span></span>
|<span data-ttu-id="64b35-119">名称</span><span class="sxs-lookup"><span data-stu-id="64b35-119">Name</span></span>|<span data-ttu-id="64b35-120">说明</span><span class="sxs-lookup"><span data-stu-id="64b35-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="64b35-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="64b35-121">Authorization</span></span>|<span data-ttu-id="64b35-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="64b35-122">Bearer {token}.</span></span> <span data-ttu-id="64b35-123">Required.</span><span class="sxs-lookup"><span data-stu-id="64b35-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64b35-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="64b35-124">Request body</span></span>
<span data-ttu-id="64b35-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="64b35-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64b35-126">响应</span><span class="sxs-lookup"><span data-stu-id="64b35-126">Response</span></span>

<span data-ttu-id="64b35-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="64b35-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="64b35-128">示例</span><span class="sxs-lookup"><span data-stu-id="64b35-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="64b35-129">请求</span><span class="sxs-lookup"><span data-stu-id="64b35-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="64b35-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="64b35-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/{teamsId}/members
```
# <a name="c"></a>[<span data-ttu-id="64b35-131">C#</span><span class="sxs-lookup"><span data-stu-id="64b35-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-members-from-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64b35-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64b35-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-members-from-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64b35-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64b35-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-members-from-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="64b35-134">响应</span><span class="sxs-lookup"><span data-stu-id="64b35-134">Response</span></span>
<span data-ttu-id="64b35-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="64b35-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

