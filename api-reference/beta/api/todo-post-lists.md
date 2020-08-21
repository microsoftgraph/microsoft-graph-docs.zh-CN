---
title: 创建 todoTaskList
description: 创建新的列表对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2628721edff8ad1dad559e590c3dade972220c73
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849899"
---
# <a name="create-todotasklist"></a><span data-ttu-id="890e5-103">创建 todoTaskList</span><span class="sxs-lookup"><span data-stu-id="890e5-103">Create todoTaskList</span></span>
<span data-ttu-id="890e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="890e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="890e5-105">创建新的列表对象。</span><span class="sxs-lookup"><span data-stu-id="890e5-105">Create a new lists object.</span></span>

## <a name="permissions"></a><span data-ttu-id="890e5-106">权限</span><span class="sxs-lookup"><span data-stu-id="890e5-106">Permissions</span></span>
<span data-ttu-id="890e5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="890e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="890e5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="890e5-109">Permission type</span></span>|<span data-ttu-id="890e5-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="890e5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="890e5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="890e5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="890e5-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="890e5-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="890e5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="890e5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="890e5-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="890e5-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="890e5-115">应用</span><span class="sxs-lookup"><span data-stu-id="890e5-115">Application</span></span>|<span data-ttu-id="890e5-116">不支持</span><span class="sxs-lookup"><span data-stu-id="890e5-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="890e5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="890e5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists
POST /users/{id|userPrincipalName}/todo/lists
```

## <a name="request-headers"></a><span data-ttu-id="890e5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="890e5-118">Request headers</span></span>
|<span data-ttu-id="890e5-119">名称</span><span class="sxs-lookup"><span data-stu-id="890e5-119">Name</span></span>|<span data-ttu-id="890e5-120">说明</span><span class="sxs-lookup"><span data-stu-id="890e5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="890e5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="890e5-121">Authorization</span></span>|<span data-ttu-id="890e5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="890e5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="890e5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="890e5-124">Content-Type</span></span>|<span data-ttu-id="890e5-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="890e5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="890e5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="890e5-127">Request body</span></span>
<span data-ttu-id="890e5-128">在请求正文中，提供 [todoTaskList](../resources/todotasklist.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="890e5-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="890e5-129">下表显示创建 [todoTaskList 时所需的属性](../resources/todotasklist.md)。</span><span class="sxs-lookup"><span data-stu-id="890e5-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="890e5-130">属性</span><span class="sxs-lookup"><span data-stu-id="890e5-130">Property</span></span>|<span data-ttu-id="890e5-131">类型</span><span class="sxs-lookup"><span data-stu-id="890e5-131">Type</span></span>|<span data-ttu-id="890e5-132">说明</span><span class="sxs-lookup"><span data-stu-id="890e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="890e5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="890e5-133">displayName</span></span>|<span data-ttu-id="890e5-134">String</span><span class="sxs-lookup"><span data-stu-id="890e5-134">String</span></span>|<span data-ttu-id="890e5-135">指示任务列表标题的域。</span><span class="sxs-lookup"><span data-stu-id="890e5-135">Field indicating title of the task list.</span></span>|

## <a name="response"></a><span data-ttu-id="890e5-136">响应</span><span class="sxs-lookup"><span data-stu-id="890e5-136">Response</span></span>

<span data-ttu-id="890e5-137">如果成功，此方法在响应 `201 Created` 正文中返回响应代码和 [todoTaskList](../resources/todotasklist.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="890e5-137">If successful, this method returns a `201 Created` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="890e5-138">示例</span><span class="sxs-lookup"><span data-stu-id="890e5-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="890e5-139">请求</span><span class="sxs-lookup"><span data-stu-id="890e5-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_todotasklist_from_lists"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists
Content-Type: application/json
Content-length: 60

{
  "displayName": "Travel items",
}
```


### <a name="response"></a><span data-ttu-id="890e5-140">响应</span><span class="sxs-lookup"><span data-stu-id="890e5-140">Response</span></span>
<span data-ttu-id="890e5-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="890e5-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.todoTaskList"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.todoTaskList",
  "id": "AAMkADIyAAAhrbPWAAA=",
  "displayName": "Travel items",
  "isOwner": true,
  "isShared": false,
  "wellknownListName": "none"
}
```