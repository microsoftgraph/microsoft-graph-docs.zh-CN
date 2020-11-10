---
title: 列出 Todo 任务
description: 从指定的 todoTaskList 的 "任务" 导航属性中获取 todoTask 资源。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 361f2c4f026f546fe6fc121bae932f132b22079d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972522"
---
# <a name="list-tasks"></a><span data-ttu-id="d6c9e-103">列出任务</span><span class="sxs-lookup"><span data-stu-id="d6c9e-103">List tasks</span></span>
<span data-ttu-id="d6c9e-104">命名空间： microsoft. graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="d6c9e-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="d6c9e-105">从指定的 [todoTaskList](../resources/todotasklist.md)的 " **任务** " 导航属性中获取 **todoTask** 资源。</span><span class="sxs-lookup"><span data-stu-id="d6c9e-105">Get the **todoTask** resources from the **tasks** navigation property of a specified [todoTaskList](../resources/todotasklist.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d6c9e-106">权限</span><span class="sxs-lookup"><span data-stu-id="d6c9e-106">Permissions</span></span>
<span data-ttu-id="d6c9e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6c9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6c9e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6c9e-109">Permission type</span></span>|<span data-ttu-id="d6c9e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d6c9e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6c9e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6c9e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d6c9e-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6c9e-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="d6c9e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6c9e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6c9e-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6c9e-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="d6c9e-115">应用</span><span class="sxs-lookup"><span data-stu-id="d6c9e-115">Application</span></span>|<span data-ttu-id="d6c9e-116">不支持</span><span class="sxs-lookup"><span data-stu-id="d6c9e-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6c9e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6c9e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6c9e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d6c9e-118">Optional query parameters</span></span>
<span data-ttu-id="d6c9e-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d6c9e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d6c9e-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d6c9e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6c9e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6c9e-121">Request headers</span></span>
|<span data-ttu-id="d6c9e-122">名称</span><span class="sxs-lookup"><span data-stu-id="d6c9e-122">Name</span></span>|<span data-ttu-id="d6c9e-123">说明</span><span class="sxs-lookup"><span data-stu-id="d6c9e-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d6c9e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6c9e-124">Authorization</span></span>|<span data-ttu-id="d6c9e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6c9e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6c9e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6c9e-127">Request body</span></span>
<span data-ttu-id="d6c9e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d6c9e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6c9e-129">响应</span><span class="sxs-lookup"><span data-stu-id="d6c9e-129">Response</span></span>

<span data-ttu-id="d6c9e-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [todoTask](../resources/todotask.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d6c9e-130">If successful, this method returns a `200 OK` response code and a collection of [todoTask](../resources/todotask.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d6c9e-131">示例</span><span class="sxs-lookup"><span data-stu-id="d6c9e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d6c9e-132">请求</span><span class="sxs-lookup"><span data-stu-id="d6c9e-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d6c9e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6c9e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["35e2-35e2-721a-e235-1a72e2351a7"],
  "name": "get_todotask"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/35e2-35e2-721a-e235-1a72e2351a7/tasks
```
# <a name="c"></a>[<span data-ttu-id="d6c9e-134">C#</span><span class="sxs-lookup"><span data-stu-id="d6c9e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6c9e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6c9e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6c9e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6c9e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6c9e-137">Java</span><span class="sxs-lookup"><span data-stu-id="d6c9e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-todotask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d6c9e-138">响应</span><span class="sxs-lookup"><span data-stu-id="d6c9e-138">Response</span></span>
<span data-ttu-id="d6c9e-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d6c9e-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.todoTask)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "value":[
      {
         "@odata.etag":"W/\"xzyPKP0BiUGgld+lMKXwbQAAgdhkVw==\"",
         "importance":"low",
         "isReminderOn":false,
         "status":"notStarted",
         "title":"Linked entity new task 1",
         "createdDateTime":"2020-07-08T11:15:19.9359889Z",
         "lastModifiedDateTime":"2020-07-08T11:15:20.0614375Z",
         "id":"AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtMDACLTAwCgBGAAAD",
         "body":{
            "content":"",
            "contentType":"text"
         },
         "linkedResources@odata.context":"https://graph.microsoft.com/beta/$metadata#users('todoservicetest2412201901%40outlook.com')/todo/lists('35e2-35e2-721a-e235-1a72e2351a7')/tasks('AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtMDACLTAwCgBGAAAD')/linkedResources",
         "linkedResources":[
            {
               "applicationName":"Partner App Name",
               "displayName":"Partner App Name",
               "externalId":"teset1243434",
               "id":"30911960-7321-4cba-9ba0-cdb68e2984c7"
            }
         ]
      }
   ]
}
```



