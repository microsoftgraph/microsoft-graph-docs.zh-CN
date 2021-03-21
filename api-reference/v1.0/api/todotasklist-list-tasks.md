---
title: 列出 Todo 任务
description: 从指定的 todoTaskList 的任务导航属性获取 todoTask 资源。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f95864aa3988f7e5598376e202c9b8d697184458
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963366"
---
# <a name="list-tasks"></a><span data-ttu-id="1df99-103">列出任务</span><span class="sxs-lookup"><span data-stu-id="1df99-103">List tasks</span></span>
<span data-ttu-id="1df99-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1df99-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1df99-105">从 **指定的 todoTaskList** 的任务导航属性获取 [todoTask 资源](../resources/todotasklist.md)。</span><span class="sxs-lookup"><span data-stu-id="1df99-105">Get the **todoTask** resources from the **tasks** navigation property of a specified [todoTaskList](../resources/todotasklist.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1df99-106">权限</span><span class="sxs-lookup"><span data-stu-id="1df99-106">Permissions</span></span>
<span data-ttu-id="1df99-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1df99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1df99-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1df99-109">Permission type</span></span>|<span data-ttu-id="1df99-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1df99-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1df99-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1df99-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1df99-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1df99-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="1df99-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1df99-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1df99-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1df99-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="1df99-115">应用</span><span class="sxs-lookup"><span data-stu-id="1df99-115">Application</span></span>|<span data-ttu-id="1df99-116">不支持</span><span class="sxs-lookup"><span data-stu-id="1df99-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="1df99-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1df99-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1df99-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1df99-118">Optional query parameters</span></span>
<span data-ttu-id="1df99-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1df99-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1df99-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="1df99-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1df99-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1df99-121">Request headers</span></span>
|<span data-ttu-id="1df99-122">名称</span><span class="sxs-lookup"><span data-stu-id="1df99-122">Name</span></span>|<span data-ttu-id="1df99-123">说明</span><span class="sxs-lookup"><span data-stu-id="1df99-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1df99-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1df99-124">Authorization</span></span>|<span data-ttu-id="1df99-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1df99-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1df99-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1df99-127">Request body</span></span>
<span data-ttu-id="1df99-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1df99-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1df99-129">响应</span><span class="sxs-lookup"><span data-stu-id="1df99-129">Response</span></span>

<span data-ttu-id="1df99-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [todoTask](../resources/todotask.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1df99-130">If successful, this method returns a `200 OK` response code and a collection of [todoTask](../resources/todotask.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1df99-131">示例</span><span class="sxs-lookup"><span data-stu-id="1df99-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1df99-132">请求</span><span class="sxs-lookup"><span data-stu-id="1df99-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1df99-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1df99-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["35e2-35e2-721a-e235-1a72e2351a7"],
  "name": "get_todotask_2"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/35e2-35e2-721a-e235-1a72e2351a7/tasks
```
# <a name="c"></a>[<span data-ttu-id="1df99-134">C#</span><span class="sxs-lookup"><span data-stu-id="1df99-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotask-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1df99-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1df99-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotask-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1df99-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1df99-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotask-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1df99-137">Java</span><span class="sxs-lookup"><span data-stu-id="1df99-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-todotask-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1df99-138">响应</span><span class="sxs-lookup"><span data-stu-id="1df99-138">Response</span></span>
<span data-ttu-id="1df99-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1df99-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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



