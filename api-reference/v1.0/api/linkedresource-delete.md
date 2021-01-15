---
title: 删除 linkedResource
description: 删除 linkedResource 对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0dd863891d9071a45a3984609b6f71a02cec5e78
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873162"
---
# <a name="delete-linkedresource"></a><span data-ttu-id="96f26-103">删除 linkedResource</span><span class="sxs-lookup"><span data-stu-id="96f26-103">Delete linkedResource</span></span>
<span data-ttu-id="96f26-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96f26-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="96f26-105">删除 [linkedResource](../resources/linkedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="96f26-105">Deletes a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="96f26-106">权限</span><span class="sxs-lookup"><span data-stu-id="96f26-106">Permissions</span></span>
<span data-ttu-id="96f26-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96f26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96f26-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="96f26-109">Permission type</span></span>|<span data-ttu-id="96f26-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96f26-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96f26-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96f26-111">Delegated (work or school account)</span></span>|<span data-ttu-id="96f26-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96f26-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="96f26-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96f26-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96f26-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96f26-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="96f26-115">应用</span><span class="sxs-lookup"><span data-stu-id="96f26-115">Application</span></span>|<span data-ttu-id="96f26-116">不支持</span><span class="sxs-lookup"><span data-stu-id="96f26-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="96f26-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96f26-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="96f26-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="96f26-118">Request headers</span></span>
|<span data-ttu-id="96f26-119">名称</span><span class="sxs-lookup"><span data-stu-id="96f26-119">Name</span></span>|<span data-ttu-id="96f26-120">说明</span><span class="sxs-lookup"><span data-stu-id="96f26-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="96f26-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="96f26-121">Authorization</span></span>|<span data-ttu-id="96f26-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96f26-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96f26-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="96f26-124">Request body</span></span>
<span data-ttu-id="96f26-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96f26-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96f26-126">响应</span><span class="sxs-lookup"><span data-stu-id="96f26-126">Response</span></span>

<span data-ttu-id="96f26-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="96f26-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="96f26-128">示例</span><span class="sxs-lookup"><span data-stu-id="96f26-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="96f26-129">请求</span><span class="sxs-lookup"><span data-stu-id="96f26-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="96f26-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="96f26-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "delete_linkedresource"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
```
# <a name="c"></a>[<span data-ttu-id="96f26-131">C#</span><span class="sxs-lookup"><span data-stu-id="96f26-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96f26-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96f26-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96f26-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96f26-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96f26-134">Java</span><span class="sxs-lookup"><span data-stu-id="96f26-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-linkedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="96f26-135">响应</span><span class="sxs-lookup"><span data-stu-id="96f26-135">Response</span></span>
<span data-ttu-id="96f26-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="96f26-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



