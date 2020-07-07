---
title: 从团队中移除成员
description: 从团队中删除 conversationMember。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8ad51fddf0acf4499271ffeb3c02e0433e52dedb
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051045"
---
# <a name="delete-members"></a><span data-ttu-id="79489-103">删除成员</span><span class="sxs-lookup"><span data-stu-id="79489-103">Delete members</span></span>
<span data-ttu-id="79489-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79489-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="79489-105">从[团队](../resources/team.md)中删除新的[conversationMember](../resources/conversationmember.md) 。</span><span class="sxs-lookup"><span data-stu-id="79489-105">Remove a new [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="79489-106">权限</span><span class="sxs-lookup"><span data-stu-id="79489-106">Permissions</span></span>
<span data-ttu-id="79489-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="79489-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="79489-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79489-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79489-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="79489-109">Permission type</span></span>|<span data-ttu-id="79489-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="79489-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79489-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79489-111">Delegated (work or school account)</span></span>| <span data-ttu-id="79489-112">TeamMember</span><span class="sxs-lookup"><span data-stu-id="79489-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="79489-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79489-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79489-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="79489-114">Not supported.</span></span>    |
|<span data-ttu-id="79489-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="79489-115">Application</span></span>| <span data-ttu-id="79489-116">TeamMember</span><span class="sxs-lookup"><span data-stu-id="79489-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79489-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79489-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{teamsId}/members
```

## <a name="request-headers"></a><span data-ttu-id="79489-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="79489-118">Request headers</span></span>
|<span data-ttu-id="79489-119">名称</span><span class="sxs-lookup"><span data-stu-id="79489-119">Name</span></span>|<span data-ttu-id="79489-120">说明</span><span class="sxs-lookup"><span data-stu-id="79489-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="79489-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="79489-121">Authorization</span></span>|<span data-ttu-id="79489-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="79489-122">Bearer {token}.</span></span> <span data-ttu-id="79489-123">Required.</span><span class="sxs-lookup"><span data-stu-id="79489-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79489-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="79489-124">Request body</span></span>
<span data-ttu-id="79489-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="79489-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79489-126">响应</span><span class="sxs-lookup"><span data-stu-id="79489-126">Response</span></span>

<span data-ttu-id="79489-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="79489-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="79489-128">示例</span><span class="sxs-lookup"><span data-stu-id="79489-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="79489-129">请求</span><span class="sxs-lookup"><span data-stu-id="79489-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/{teamsId}/members
```


### <a name="response"></a><span data-ttu-id="79489-130">响应</span><span class="sxs-lookup"><span data-stu-id="79489-130">Response</span></span>
<span data-ttu-id="79489-131">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="79489-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

