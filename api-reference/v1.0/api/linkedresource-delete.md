---
title: 删除 linkedResource
description: 删除一个 linkedResource 对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8c6ca34116903301200b7cf3d04de9f6c6069087
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903450"
---
# <a name="delete-linkedresource"></a><span data-ttu-id="05049-103">删除 linkedResource</span><span class="sxs-lookup"><span data-stu-id="05049-103">Delete linkedResource</span></span>
<span data-ttu-id="05049-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05049-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="05049-105">删除一个 [linkedResource](../resources/linkedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05049-105">Deletes a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="05049-106">权限</span><span class="sxs-lookup"><span data-stu-id="05049-106">Permissions</span></span>
<span data-ttu-id="05049-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05049-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05049-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="05049-109">Permission type</span></span>|<span data-ttu-id="05049-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="05049-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05049-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05049-111">Delegated (work or school account)</span></span>|<span data-ttu-id="05049-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05049-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="05049-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05049-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05049-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05049-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="05049-115">应用</span><span class="sxs-lookup"><span data-stu-id="05049-115">Application</span></span>|<span data-ttu-id="05049-116">不支持</span><span class="sxs-lookup"><span data-stu-id="05049-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="05049-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05049-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="05049-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="05049-118">Request headers</span></span>
|<span data-ttu-id="05049-119">名称</span><span class="sxs-lookup"><span data-stu-id="05049-119">Name</span></span>|<span data-ttu-id="05049-120">说明</span><span class="sxs-lookup"><span data-stu-id="05049-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="05049-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="05049-121">Authorization</span></span>|<span data-ttu-id="05049-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="05049-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="05049-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="05049-124">Request body</span></span>
<span data-ttu-id="05049-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="05049-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05049-126">响应</span><span class="sxs-lookup"><span data-stu-id="05049-126">Response</span></span>

<span data-ttu-id="05049-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="05049-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="05049-128">示例</span><span class="sxs-lookup"><span data-stu-id="05049-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="05049-129">请求</span><span class="sxs-lookup"><span data-stu-id="05049-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="05049-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="05049-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "delete_linkedresource"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
```
# <a name="c"></a>[<span data-ttu-id="05049-131">C#</span><span class="sxs-lookup"><span data-stu-id="05049-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05049-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05049-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05049-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05049-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="05049-134">Java</span><span class="sxs-lookup"><span data-stu-id="05049-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-linkedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="05049-135">响应</span><span class="sxs-lookup"><span data-stu-id="05049-135">Response</span></span>
<span data-ttu-id="05049-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="05049-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



