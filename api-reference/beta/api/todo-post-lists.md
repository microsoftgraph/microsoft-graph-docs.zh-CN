---
title: 创建 todoTaskList
description: 创建新的列表对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: dcb83c76fbbb4d17763a32e31e345374a5928e63
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843147"
---
# <a name="create-todotasklist"></a><span data-ttu-id="46b8e-103">创建 todoTaskList</span><span class="sxs-lookup"><span data-stu-id="46b8e-103">Create todoTaskList</span></span>
<span data-ttu-id="46b8e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46b8e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="46b8e-105">创建新的列表对象。</span><span class="sxs-lookup"><span data-stu-id="46b8e-105">Create a new lists object.</span></span>

## <a name="permissions"></a><span data-ttu-id="46b8e-106">权限</span><span class="sxs-lookup"><span data-stu-id="46b8e-106">Permissions</span></span>
<span data-ttu-id="46b8e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46b8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46b8e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="46b8e-109">Permission type</span></span>|<span data-ttu-id="46b8e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="46b8e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46b8e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46b8e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46b8e-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46b8e-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="46b8e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46b8e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46b8e-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46b8e-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="46b8e-115">应用</span><span class="sxs-lookup"><span data-stu-id="46b8e-115">Application</span></span>|<span data-ttu-id="46b8e-116">不支持</span><span class="sxs-lookup"><span data-stu-id="46b8e-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="46b8e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46b8e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists
POST /users/{id|userPrincipalName}/todo/lists
```

## <a name="request-headers"></a><span data-ttu-id="46b8e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="46b8e-118">Request headers</span></span>
|<span data-ttu-id="46b8e-119">名称</span><span class="sxs-lookup"><span data-stu-id="46b8e-119">Name</span></span>|<span data-ttu-id="46b8e-120">说明</span><span class="sxs-lookup"><span data-stu-id="46b8e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="46b8e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="46b8e-121">Authorization</span></span>|<span data-ttu-id="46b8e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="46b8e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="46b8e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="46b8e-124">Content-Type</span></span>|<span data-ttu-id="46b8e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="46b8e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46b8e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="46b8e-127">Request body</span></span>
<span data-ttu-id="46b8e-128">在请求正文中，提供 [todoTaskList](../resources/todotasklist.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="46b8e-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="46b8e-129">下表显示创建 [todoTaskList](../resources/todotasklist.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="46b8e-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="46b8e-130">属性</span><span class="sxs-lookup"><span data-stu-id="46b8e-130">Property</span></span>|<span data-ttu-id="46b8e-131">类型</span><span class="sxs-lookup"><span data-stu-id="46b8e-131">Type</span></span>|<span data-ttu-id="46b8e-132">说明</span><span class="sxs-lookup"><span data-stu-id="46b8e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46b8e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="46b8e-133">displayName</span></span>|<span data-ttu-id="46b8e-134">String</span><span class="sxs-lookup"><span data-stu-id="46b8e-134">String</span></span>|<span data-ttu-id="46b8e-135">指示任务列表的标题的字段。</span><span class="sxs-lookup"><span data-stu-id="46b8e-135">Field indicating title of the task list.</span></span>|

## <a name="response"></a><span data-ttu-id="46b8e-136">响应</span><span class="sxs-lookup"><span data-stu-id="46b8e-136">Response</span></span>

<span data-ttu-id="46b8e-137">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [todoTaskList](../resources/todotasklist.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="46b8e-137">If successful, this method returns a `201 Created` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="46b8e-138">示例</span><span class="sxs-lookup"><span data-stu-id="46b8e-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="46b8e-139">请求</span><span class="sxs-lookup"><span data-stu-id="46b8e-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="46b8e-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="46b8e-140">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="46b8e-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46b8e-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-todotasklist-from-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="46b8e-142">C#</span><span class="sxs-lookup"><span data-stu-id="46b8e-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-todotasklist-from-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46b8e-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46b8e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-todotasklist-from-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="46b8e-144">响应</span><span class="sxs-lookup"><span data-stu-id="46b8e-144">Response</span></span>
<span data-ttu-id="46b8e-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="46b8e-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
