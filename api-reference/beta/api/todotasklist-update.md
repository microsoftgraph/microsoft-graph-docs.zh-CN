---
title: 更新 todoTaskList
description: 更新 todoTaskList 对象的属性。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f7689ee98e8bcc511285fbf87f3f010e2b22a08b
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312776"
---
# <a name="update-todotasklist"></a><span data-ttu-id="75114-103">更新 todoTaskList</span><span class="sxs-lookup"><span data-stu-id="75114-103">Update todoTaskList</span></span>
<span data-ttu-id="75114-104">命名空间： microsoft. graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="75114-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="75114-105">更新 [todoTaskList](../resources/todotasklist.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="75114-105">Update the properties of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="75114-106">权限</span><span class="sxs-lookup"><span data-stu-id="75114-106">Permissions</span></span>
<span data-ttu-id="75114-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75114-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75114-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="75114-109">Permission type</span></span>|<span data-ttu-id="75114-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="75114-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75114-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75114-111">Delegated (work or school account)</span></span>|<span data-ttu-id="75114-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75114-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="75114-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75114-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75114-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75114-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="75114-115">应用</span><span class="sxs-lookup"><span data-stu-id="75114-115">Application</span></span>|<span data-ttu-id="75114-116">不支持</span><span class="sxs-lookup"><span data-stu-id="75114-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="75114-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75114-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="75114-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="75114-118">Request headers</span></span>
|<span data-ttu-id="75114-119">名称</span><span class="sxs-lookup"><span data-stu-id="75114-119">Name</span></span>|<span data-ttu-id="75114-120">说明</span><span class="sxs-lookup"><span data-stu-id="75114-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="75114-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="75114-121">Authorization</span></span>|<span data-ttu-id="75114-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="75114-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="75114-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="75114-124">Content-Type</span></span>|<span data-ttu-id="75114-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="75114-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75114-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="75114-127">Request body</span></span>
<span data-ttu-id="75114-128">在请求正文中，提供 [todoTaskList](../resources/todotasklist.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75114-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="75114-129">下表显示创建 [todoTaskList](../resources/todotasklist.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="75114-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="75114-130">属性</span><span class="sxs-lookup"><span data-stu-id="75114-130">Property</span></span>|<span data-ttu-id="75114-131">类型</span><span class="sxs-lookup"><span data-stu-id="75114-131">Type</span></span>|<span data-ttu-id="75114-132">说明</span><span class="sxs-lookup"><span data-stu-id="75114-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75114-133">displayName</span><span class="sxs-lookup"><span data-stu-id="75114-133">displayName</span></span>|<span data-ttu-id="75114-134">字符串</span><span class="sxs-lookup"><span data-stu-id="75114-134">String</span></span>|<span data-ttu-id="75114-135">指示任务列表更新的标题的字段。</span><span class="sxs-lookup"><span data-stu-id="75114-135">Field indicating updated title of the task list.</span></span>|



## <a name="response"></a><span data-ttu-id="75114-136">响应</span><span class="sxs-lookup"><span data-stu-id="75114-136">Response</span></span>

<span data-ttu-id="75114-137">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [todoTaskList](../resources/todotasklist.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="75114-137">If successful, this method returns a `200 OK` response code and an updated [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="75114-138">示例</span><span class="sxs-lookup"><span data-stu-id="75114-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="75114-139">请求</span><span class="sxs-lookup"><span data-stu-id="75114-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="75114-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="75114-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAhrbPWAAA="],
  "name": "update_todotasklist"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/todo/lists/AAMkADIyAAAhrbPWAAA=
Content-Type: application/json
Content-length: 167

{
  "displayName": "Vacation Plan"
}
```
# <a name="javascript"></a>[<span data-ttu-id="75114-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75114-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="75114-142">C#</span><span class="sxs-lookup"><span data-stu-id="75114-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75114-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75114-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="75114-144">响应</span><span class="sxs-lookup"><span data-stu-id="75114-144">Response</span></span>
<span data-ttu-id="75114-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="75114-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.todoTaskList"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.todoTaskList",
  "id": "AAMkADIyAAAhrbPWAAA=",
  "displayName": "Vacation Plan",
  "isOwner": true,
  "isShared": false,
  "wellknownListName": "none"
}
```



