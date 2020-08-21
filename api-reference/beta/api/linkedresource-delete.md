---
title: 删除 linkedResource
description: 删除 linkedResource 对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 33fdb7e29ee2e5249f5eab577d997661f211519b
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849911"
---
# <a name="delete-linkedresource"></a><span data-ttu-id="546bb-103">删除 linkedResource</span><span class="sxs-lookup"><span data-stu-id="546bb-103">Delete linkedResource</span></span>
<span data-ttu-id="546bb-104">命名空间：microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="546bb-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="546bb-105">删除 [linkedResource](../resources/linkedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="546bb-105">Deletes a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="546bb-106">权限</span><span class="sxs-lookup"><span data-stu-id="546bb-106">Permissions</span></span>
<span data-ttu-id="546bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="546bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="546bb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="546bb-109">Permission type</span></span>|<span data-ttu-id="546bb-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="546bb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="546bb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="546bb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="546bb-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="546bb-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="546bb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="546bb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="546bb-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="546bb-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="546bb-115">应用</span><span class="sxs-lookup"><span data-stu-id="546bb-115">Application</span></span>|<span data-ttu-id="546bb-116">不支持</span><span class="sxs-lookup"><span data-stu-id="546bb-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="546bb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="546bb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="546bb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="546bb-118">Request headers</span></span>
|<span data-ttu-id="546bb-119">名称</span><span class="sxs-lookup"><span data-stu-id="546bb-119">Name</span></span>|<span data-ttu-id="546bb-120">说明</span><span class="sxs-lookup"><span data-stu-id="546bb-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="546bb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="546bb-121">Authorization</span></span>|<span data-ttu-id="546bb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="546bb-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="546bb-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="546bb-124">Request body</span></span>
<span data-ttu-id="546bb-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="546bb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="546bb-126">响应</span><span class="sxs-lookup"><span data-stu-id="546bb-126">Response</span></span>

<span data-ttu-id="546bb-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="546bb-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="546bb-128">示例</span><span class="sxs-lookup"><span data-stu-id="546bb-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="546bb-129">请求</span><span class="sxs-lookup"><span data-stu-id="546bb-129">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "delete_linkedresource"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
```


### <a name="response"></a><span data-ttu-id="546bb-130">响应</span><span class="sxs-lookup"><span data-stu-id="546bb-130">Response</span></span>
<span data-ttu-id="546bb-131">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="546bb-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

