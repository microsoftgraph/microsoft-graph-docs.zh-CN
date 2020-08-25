---
title: 删除 linkedResource
description: 删除一个 linkedResource 对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5bf6ab3c6791e84602efc8eb0d61be8d825ec012
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873315"
---
# <a name="delete-linkedresource"></a><span data-ttu-id="a201e-103">删除 linkedResource</span><span class="sxs-lookup"><span data-stu-id="a201e-103">Delete linkedResource</span></span>
<span data-ttu-id="a201e-104">命名空间： microsoft. graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="a201e-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="a201e-105">删除一个 [linkedResource](../resources/linkedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a201e-105">Deletes a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a201e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a201e-106">Permissions</span></span>
<span data-ttu-id="a201e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a201e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a201e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a201e-109">Permission type</span></span>|<span data-ttu-id="a201e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a201e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a201e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a201e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a201e-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a201e-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="a201e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a201e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a201e-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a201e-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="a201e-115">应用</span><span class="sxs-lookup"><span data-stu-id="a201e-115">Application</span></span>|<span data-ttu-id="a201e-116">不支持</span><span class="sxs-lookup"><span data-stu-id="a201e-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="a201e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a201e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="a201e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a201e-118">Request headers</span></span>
|<span data-ttu-id="a201e-119">名称</span><span class="sxs-lookup"><span data-stu-id="a201e-119">Name</span></span>|<span data-ttu-id="a201e-120">说明</span><span class="sxs-lookup"><span data-stu-id="a201e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a201e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a201e-121">Authorization</span></span>|<span data-ttu-id="a201e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a201e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a201e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="a201e-124">Request body</span></span>
<span data-ttu-id="a201e-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a201e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a201e-126">响应</span><span class="sxs-lookup"><span data-stu-id="a201e-126">Response</span></span>

<span data-ttu-id="a201e-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a201e-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a201e-128">示例</span><span class="sxs-lookup"><span data-stu-id="a201e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a201e-129">请求</span><span class="sxs-lookup"><span data-stu-id="a201e-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a201e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a201e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "delete_linkedresource"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
```
# <a name="c"></a>[<span data-ttu-id="a201e-131">C#</span><span class="sxs-lookup"><span data-stu-id="a201e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a201e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a201e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a201e-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a201e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a201e-134">响应</span><span class="sxs-lookup"><span data-stu-id="a201e-134">Response</span></span>
<span data-ttu-id="a201e-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a201e-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

