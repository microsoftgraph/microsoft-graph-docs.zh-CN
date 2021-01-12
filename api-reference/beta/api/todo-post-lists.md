---
title: 创建 todoTaskList
description: 创建新的列表对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6e09dd501de62009d4baf06f85381f275223e673
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796701"
---
# <a name="create-todotasklist"></a><span data-ttu-id="596ea-103">创建 todoTaskList</span><span class="sxs-lookup"><span data-stu-id="596ea-103">Create todoTaskList</span></span>
<span data-ttu-id="596ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="596ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="596ea-105">创建新的列表对象。</span><span class="sxs-lookup"><span data-stu-id="596ea-105">Create a new lists object.</span></span>

## <a name="permissions"></a><span data-ttu-id="596ea-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="596ea-106">Permissions</span></span>
<span data-ttu-id="596ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="596ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="596ea-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="596ea-109">Permission type</span></span>|<span data-ttu-id="596ea-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="596ea-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="596ea-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="596ea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="596ea-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="596ea-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="596ea-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="596ea-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="596ea-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="596ea-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="596ea-115">应用</span><span class="sxs-lookup"><span data-stu-id="596ea-115">Application</span></span>|<span data-ttu-id="596ea-116">不支持</span><span class="sxs-lookup"><span data-stu-id="596ea-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="596ea-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="596ea-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists
POST /users/{id|userPrincipalName}/todo/lists
```

## <a name="request-headers"></a><span data-ttu-id="596ea-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="596ea-118">Request headers</span></span>
|<span data-ttu-id="596ea-119">名称</span><span class="sxs-lookup"><span data-stu-id="596ea-119">Name</span></span>|<span data-ttu-id="596ea-120">说明</span><span class="sxs-lookup"><span data-stu-id="596ea-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="596ea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="596ea-121">Authorization</span></span>|<span data-ttu-id="596ea-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="596ea-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="596ea-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="596ea-124">Content-Type</span></span>|<span data-ttu-id="596ea-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="596ea-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="596ea-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="596ea-127">Request body</span></span>
<span data-ttu-id="596ea-128">在请求正文中，提供 [todoTaskList](../resources/todotasklist.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="596ea-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="596ea-129">下表显示创建 [todoTaskList 时所需的属性](../resources/todotasklist.md)。</span><span class="sxs-lookup"><span data-stu-id="596ea-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="596ea-130">属性</span><span class="sxs-lookup"><span data-stu-id="596ea-130">Property</span></span>|<span data-ttu-id="596ea-131">类型</span><span class="sxs-lookup"><span data-stu-id="596ea-131">Type</span></span>|<span data-ttu-id="596ea-132">说明</span><span class="sxs-lookup"><span data-stu-id="596ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="596ea-133">displayName</span><span class="sxs-lookup"><span data-stu-id="596ea-133">displayName</span></span>|<span data-ttu-id="596ea-134">String</span><span class="sxs-lookup"><span data-stu-id="596ea-134">String</span></span>|<span data-ttu-id="596ea-135">指示任务列表标题的域。</span><span class="sxs-lookup"><span data-stu-id="596ea-135">Field indicating title of the task list.</span></span>|

## <a name="response"></a><span data-ttu-id="596ea-136">响应</span><span class="sxs-lookup"><span data-stu-id="596ea-136">Response</span></span>

<span data-ttu-id="596ea-137">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [todoTaskList](../resources/todotasklist.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="596ea-137">If successful, this method returns a `201 Created` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="596ea-138">示例</span><span class="sxs-lookup"><span data-stu-id="596ea-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="596ea-139">请求</span><span class="sxs-lookup"><span data-stu-id="596ea-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="596ea-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="596ea-140">HTTP</span></span>](#tab/http)
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
  "displayName": "Travel items"
}
```
# <a name="javascript"></a>[<span data-ttu-id="596ea-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="596ea-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-todotasklist-from-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="596ea-142">C#</span><span class="sxs-lookup"><span data-stu-id="596ea-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-todotasklist-from-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="596ea-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="596ea-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-todotasklist-from-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="596ea-144">Java</span><span class="sxs-lookup"><span data-stu-id="596ea-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-todotasklist-from-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="596ea-145">响应</span><span class="sxs-lookup"><span data-stu-id="596ea-145">Response</span></span>
<span data-ttu-id="596ea-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="596ea-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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


