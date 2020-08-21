---
title: 删除 todoTaskList
description: 删除 todoTaskList 对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0e43ec8d9a8d758a8b064051b95b0ca8256117c1
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849886"
---
# <a name="delete-todotasklist"></a><span data-ttu-id="addf5-103">删除 todoTaskList</span><span class="sxs-lookup"><span data-stu-id="addf5-103">Delete todoTaskList</span></span>
<span data-ttu-id="addf5-104">命名空间：microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="addf5-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="addf5-105">删除 [todoTaskList](../resources/todotasklist.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="addf5-105">Deletes a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="addf5-106">权限</span><span class="sxs-lookup"><span data-stu-id="addf5-106">Permissions</span></span>
<span data-ttu-id="addf5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="addf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="addf5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="addf5-109">Permission type</span></span>|<span data-ttu-id="addf5-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="addf5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="addf5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="addf5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="addf5-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="addf5-112">Tasks.Read</span></span>|
|<span data-ttu-id="addf5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="addf5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="addf5-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="addf5-114">Tasks.Read</span></span>|
|<span data-ttu-id="addf5-115">应用</span><span class="sxs-lookup"><span data-stu-id="addf5-115">Application</span></span>|<span data-ttu-id="addf5-116">不支持</span><span class="sxs-lookup"><span data-stu-id="addf5-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="addf5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="addf5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="request-headers"></a><span data-ttu-id="addf5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="addf5-118">Request headers</span></span>
|<span data-ttu-id="addf5-119">名称</span><span class="sxs-lookup"><span data-stu-id="addf5-119">Name</span></span>|<span data-ttu-id="addf5-120">说明</span><span class="sxs-lookup"><span data-stu-id="addf5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="addf5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="addf5-121">Authorization</span></span>|<span data-ttu-id="addf5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="addf5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="addf5-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="addf5-124">Request body</span></span>
<span data-ttu-id="addf5-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="addf5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="addf5-126">响应</span><span class="sxs-lookup"><span data-stu-id="addf5-126">Response</span></span>

<span data-ttu-id="addf5-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="addf5-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="addf5-128">示例</span><span class="sxs-lookup"><span data-stu-id="addf5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="addf5-129">请求</span><span class="sxs-lookup"><span data-stu-id="addf5-129">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAhrbPXAAA="],
  "name": "delete_todotasklist"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/todo/lists/AAMkADIyAAAhrbPXAAA=
```


### <a name="response"></a><span data-ttu-id="addf5-130">响应</span><span class="sxs-lookup"><span data-stu-id="addf5-130">Response</span></span>
<span data-ttu-id="addf5-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="addf5-131">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

