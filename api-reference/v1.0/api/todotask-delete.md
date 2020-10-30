---
title: 删除 todoTask
description: 删除一个 todoTask 对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ca86b2344e67c86418c8bc5d2d3914148994f1e9
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797275"
---
# <a name="delete-todotask"></a><span data-ttu-id="01a51-103">删除 todoTask</span><span class="sxs-lookup"><span data-stu-id="01a51-103">Delete todoTask</span></span>
<span data-ttu-id="01a51-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01a51-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="01a51-105">删除一个 [todoTask](../resources/todotask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="01a51-105">Deletes a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="01a51-106">权限</span><span class="sxs-lookup"><span data-stu-id="01a51-106">Permissions</span></span>
<span data-ttu-id="01a51-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01a51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01a51-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="01a51-109">Permission type</span></span>|<span data-ttu-id="01a51-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="01a51-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01a51-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01a51-111">Delegated (work or school account)</span></span>|<span data-ttu-id="01a51-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01a51-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="01a51-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01a51-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01a51-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01a51-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="01a51-115">应用</span><span class="sxs-lookup"><span data-stu-id="01a51-115">Application</span></span>|<span data-ttu-id="01a51-116">不支持</span><span class="sxs-lookup"><span data-stu-id="01a51-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="01a51-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01a51-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{taskId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="01a51-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="01a51-118">Request headers</span></span>
|<span data-ttu-id="01a51-119">名称</span><span class="sxs-lookup"><span data-stu-id="01a51-119">Name</span></span>|<span data-ttu-id="01a51-120">说明</span><span class="sxs-lookup"><span data-stu-id="01a51-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="01a51-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="01a51-121">Authorization</span></span>|<span data-ttu-id="01a51-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01a51-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="01a51-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="01a51-124">Request body</span></span>
<span data-ttu-id="01a51-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="01a51-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01a51-126">响应</span><span class="sxs-lookup"><span data-stu-id="01a51-126">Response</span></span>

<span data-ttu-id="01a51-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="01a51-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="01a51-128">示例</span><span class="sxs-lookup"><span data-stu-id="01a51-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="01a51-129">请求</span><span class="sxs-lookup"><span data-stu-id="01a51-129">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "name": "delete_todotask"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
```


### <a name="response"></a><span data-ttu-id="01a51-130">响应</span><span class="sxs-lookup"><span data-stu-id="01a51-130">Response</span></span>
<span data-ttu-id="01a51-131">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="01a51-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



