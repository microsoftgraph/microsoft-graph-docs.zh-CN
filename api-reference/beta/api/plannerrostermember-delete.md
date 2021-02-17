---
title: 删除 plannerRosterMember
description: 删除 plannerRosterMember 对象。
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: d6101b5c82bc2eb7a631d01df00f447398f87715
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272076"
---
# <a name="delete-plannerrostermember"></a><span data-ttu-id="27221-103">删除 plannerRosterMember</span><span class="sxs-lookup"><span data-stu-id="27221-103">Delete plannerRosterMember</span></span>
<span data-ttu-id="27221-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27221-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27221-105">删除 [plannerRosterMember](../resources/plannerrostermember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="27221-105">Delete a [plannerRosterMember](../resources/plannerrostermember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="27221-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="27221-106">Permissions</span></span>
<span data-ttu-id="27221-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27221-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27221-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="27221-109">Permission type</span></span>|<span data-ttu-id="27221-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="27221-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27221-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27221-111">Delegated (work or school account)</span></span>|<span data-ttu-id="27221-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27221-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="27221-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27221-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27221-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="27221-114">Not supported.</span></span>|
|<span data-ttu-id="27221-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="27221-115">Application</span></span>|<span data-ttu-id="27221-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="27221-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27221-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27221-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /planner/rosters/{plannerRosterId}/members/{plannerRosterMemberId}
```

## <a name="request-headers"></a><span data-ttu-id="27221-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="27221-118">Request headers</span></span>
|<span data-ttu-id="27221-119">名称</span><span class="sxs-lookup"><span data-stu-id="27221-119">Name</span></span>|<span data-ttu-id="27221-120">说明</span><span class="sxs-lookup"><span data-stu-id="27221-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="27221-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="27221-121">Authorization</span></span>|<span data-ttu-id="27221-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="27221-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27221-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="27221-124">Request body</span></span>
<span data-ttu-id="27221-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="27221-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27221-126">响应</span><span class="sxs-lookup"><span data-stu-id="27221-126">Response</span></span>

<span data-ttu-id="27221-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="27221-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="27221-128">示例</span><span class="sxs-lookup"><span data-stu-id="27221-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27221-129">请求</span><span class="sxs-lookup"><span data-stu-id="27221-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="27221-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="27221-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_plannerrostermember"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/planner/rosters/523a9d5a-f9d5-45c1-929f-b8525393515c/members/5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38
```
# <a name="c"></a>[<span data-ttu-id="27221-131">C#</span><span class="sxs-lookup"><span data-stu-id="27221-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-plannerrostermember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27221-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27221-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-plannerrostermember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27221-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27221-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-plannerrostermember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27221-134">Java</span><span class="sxs-lookup"><span data-stu-id="27221-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-plannerrostermember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="27221-135">响应</span><span class="sxs-lookup"><span data-stu-id="27221-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

