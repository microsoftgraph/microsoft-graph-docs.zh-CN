---
title: 删除 todoTaskList
description: 删除一个 todoTaskList 对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 83944ea1b4749a556646fe6133facb14e88d612c
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797247"
---
# <a name="delete-todotasklist"></a><span data-ttu-id="f5bdc-103">删除 todoTaskList</span><span class="sxs-lookup"><span data-stu-id="f5bdc-103">Delete todoTaskList</span></span>
<span data-ttu-id="f5bdc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5bdc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f5bdc-105">删除一个 [todoTaskList](../resources/todotasklist.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5bdc-105">Deletes a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5bdc-106">权限</span><span class="sxs-lookup"><span data-stu-id="f5bdc-106">Permissions</span></span>
<span data-ttu-id="f5bdc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5bdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5bdc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5bdc-109">Permission type</span></span>|<span data-ttu-id="f5bdc-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f5bdc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5bdc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5bdc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f5bdc-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f5bdc-112">Tasks.Read</span></span>|
|<span data-ttu-id="f5bdc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5bdc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5bdc-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f5bdc-114">Tasks.Read</span></span>|
|<span data-ttu-id="f5bdc-115">应用</span><span class="sxs-lookup"><span data-stu-id="f5bdc-115">Application</span></span>|<span data-ttu-id="f5bdc-116">不支持</span><span class="sxs-lookup"><span data-stu-id="f5bdc-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5bdc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5bdc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="request-headers"></a><span data-ttu-id="f5bdc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5bdc-118">Request headers</span></span>
|<span data-ttu-id="f5bdc-119">名称</span><span class="sxs-lookup"><span data-stu-id="f5bdc-119">Name</span></span>|<span data-ttu-id="f5bdc-120">说明</span><span class="sxs-lookup"><span data-stu-id="f5bdc-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f5bdc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5bdc-121">Authorization</span></span>|<span data-ttu-id="f5bdc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f5bdc-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5bdc-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5bdc-124">Request body</span></span>
<span data-ttu-id="f5bdc-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f5bdc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5bdc-126">响应</span><span class="sxs-lookup"><span data-stu-id="f5bdc-126">Response</span></span>

<span data-ttu-id="f5bdc-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f5bdc-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f5bdc-128">示例</span><span class="sxs-lookup"><span data-stu-id="f5bdc-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f5bdc-129">请求</span><span class="sxs-lookup"><span data-stu-id="f5bdc-129">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAhrbPXAAA="],
  "name": "delete_todotasklist"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADIyAAAhrbPXAAA=
```


### <a name="response"></a><span data-ttu-id="f5bdc-130">响应</span><span class="sxs-lookup"><span data-stu-id="f5bdc-130">Response</span></span>
<span data-ttu-id="f5bdc-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f5bdc-131">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



