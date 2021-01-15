---
title: 删除 todoTaskList
description: 删除 todoTaskList 对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c5ae6511310158c8521667c03bbe3310ff70c067
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873337"
---
# <a name="delete-todotasklist"></a><span data-ttu-id="e64a9-103">删除 todoTaskList</span><span class="sxs-lookup"><span data-stu-id="e64a9-103">Delete todoTaskList</span></span>
<span data-ttu-id="e64a9-104">命名空间：microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="e64a9-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="e64a9-105">删除 [todoTaskList](../resources/todotasklist.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e64a9-105">Deletes a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e64a9-106">权限</span><span class="sxs-lookup"><span data-stu-id="e64a9-106">Permissions</span></span>
<span data-ttu-id="e64a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e64a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e64a9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e64a9-109">Permission type</span></span>|<span data-ttu-id="e64a9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e64a9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e64a9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e64a9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e64a9-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="e64a9-112">Tasks.Read</span></span>|
|<span data-ttu-id="e64a9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e64a9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e64a9-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="e64a9-114">Tasks.Read</span></span>|
|<span data-ttu-id="e64a9-115">应用</span><span class="sxs-lookup"><span data-stu-id="e64a9-115">Application</span></span>|<span data-ttu-id="e64a9-116">不支持</span><span class="sxs-lookup"><span data-stu-id="e64a9-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="e64a9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e64a9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="request-headers"></a><span data-ttu-id="e64a9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e64a9-118">Request headers</span></span>
|<span data-ttu-id="e64a9-119">名称</span><span class="sxs-lookup"><span data-stu-id="e64a9-119">Name</span></span>|<span data-ttu-id="e64a9-120">说明</span><span class="sxs-lookup"><span data-stu-id="e64a9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e64a9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e64a9-121">Authorization</span></span>|<span data-ttu-id="e64a9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e64a9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e64a9-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e64a9-124">Request body</span></span>
<span data-ttu-id="e64a9-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e64a9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e64a9-126">响应</span><span class="sxs-lookup"><span data-stu-id="e64a9-126">Response</span></span>

<span data-ttu-id="e64a9-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e64a9-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e64a9-128">示例</span><span class="sxs-lookup"><span data-stu-id="e64a9-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e64a9-129">请求</span><span class="sxs-lookup"><span data-stu-id="e64a9-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e64a9-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="e64a9-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAhrbPXAAA="],
  "name": "delete_todotasklist"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/todo/lists/AAMkADIyAAAhrbPXAAA=
```
# <a name="c"></a>[<span data-ttu-id="e64a9-131">C#</span><span class="sxs-lookup"><span data-stu-id="e64a9-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e64a9-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e64a9-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e64a9-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e64a9-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e64a9-134">Java</span><span class="sxs-lookup"><span data-stu-id="e64a9-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-todotasklist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e64a9-135">响应</span><span class="sxs-lookup"><span data-stu-id="e64a9-135">Response</span></span>
<span data-ttu-id="e64a9-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e64a9-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



