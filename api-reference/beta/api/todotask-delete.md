---
title: 删除 todoTask
description: 删除一个 todoTask 对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e5cb89bc7e21ca777f36ca846e186f741b7b5667
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873344"
---
# <a name="delete-todotask"></a><span data-ttu-id="204f7-103">删除 todoTask</span><span class="sxs-lookup"><span data-stu-id="204f7-103">Delete todoTask</span></span>
<span data-ttu-id="204f7-104">命名空间： microsoft. graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="204f7-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="204f7-105">删除一个 [todoTask](../resources/todotask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="204f7-105">Deletes a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="204f7-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="204f7-106">Permissions</span></span>
<span data-ttu-id="204f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="204f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="204f7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="204f7-109">Permission type</span></span>|<span data-ttu-id="204f7-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="204f7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="204f7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="204f7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="204f7-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="204f7-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="204f7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="204f7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="204f7-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="204f7-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="204f7-115">应用</span><span class="sxs-lookup"><span data-stu-id="204f7-115">Application</span></span>|<span data-ttu-id="204f7-116">不支持</span><span class="sxs-lookup"><span data-stu-id="204f7-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="204f7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="204f7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{taskId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="204f7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="204f7-118">Request headers</span></span>
|<span data-ttu-id="204f7-119">名称</span><span class="sxs-lookup"><span data-stu-id="204f7-119">Name</span></span>|<span data-ttu-id="204f7-120">说明</span><span class="sxs-lookup"><span data-stu-id="204f7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="204f7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="204f7-121">Authorization</span></span>|<span data-ttu-id="204f7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="204f7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="204f7-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="204f7-124">Request body</span></span>
<span data-ttu-id="204f7-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="204f7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="204f7-126">响应</span><span class="sxs-lookup"><span data-stu-id="204f7-126">Response</span></span>

<span data-ttu-id="204f7-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="204f7-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="204f7-128">示例</span><span class="sxs-lookup"><span data-stu-id="204f7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="204f7-129">请求</span><span class="sxs-lookup"><span data-stu-id="204f7-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="204f7-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="204f7-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "name": "delete_todotask"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
```
# <a name="c"></a>[<span data-ttu-id="204f7-131">C#</span><span class="sxs-lookup"><span data-stu-id="204f7-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="204f7-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="204f7-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="204f7-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="204f7-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="204f7-134">响应</span><span class="sxs-lookup"><span data-stu-id="204f7-134">Response</span></span>
<span data-ttu-id="204f7-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="204f7-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

