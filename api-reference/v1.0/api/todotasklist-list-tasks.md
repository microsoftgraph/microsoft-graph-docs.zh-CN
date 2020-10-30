---
title: 列出 Todo 任务
description: 从指定的 todoTaskList 的 "任务" 导航属性中获取 todoTask 资源。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6192d552d4413a8d49babb3c6b40115f4316e39f
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797267"
---
# <a name="list-tasks"></a><span data-ttu-id="494d6-103">列出任务</span><span class="sxs-lookup"><span data-stu-id="494d6-103">List tasks</span></span>
<span data-ttu-id="494d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="494d6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="494d6-105">从指定的 [todoTaskList](../resources/todotasklist.md)的 " **任务** " 导航属性中获取 **todoTask** 资源。</span><span class="sxs-lookup"><span data-stu-id="494d6-105">Get the **todoTask** resources from the **tasks** navigation property of a specified [todoTaskList](../resources/todotasklist.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="494d6-106">权限</span><span class="sxs-lookup"><span data-stu-id="494d6-106">Permissions</span></span>
<span data-ttu-id="494d6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="494d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="494d6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="494d6-109">Permission type</span></span>|<span data-ttu-id="494d6-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="494d6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="494d6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="494d6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="494d6-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="494d6-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="494d6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="494d6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="494d6-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="494d6-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="494d6-115">应用</span><span class="sxs-lookup"><span data-stu-id="494d6-115">Application</span></span>|<span data-ttu-id="494d6-116">不支持</span><span class="sxs-lookup"><span data-stu-id="494d6-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="494d6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="494d6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="optional-query-parameters"></a><span data-ttu-id="494d6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="494d6-118">Optional query parameters</span></span>
<span data-ttu-id="494d6-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="494d6-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="494d6-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="494d6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="494d6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="494d6-121">Request headers</span></span>
|<span data-ttu-id="494d6-122">名称</span><span class="sxs-lookup"><span data-stu-id="494d6-122">Name</span></span>|<span data-ttu-id="494d6-123">说明</span><span class="sxs-lookup"><span data-stu-id="494d6-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="494d6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="494d6-124">Authorization</span></span>|<span data-ttu-id="494d6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="494d6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="494d6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="494d6-127">Request body</span></span>
<span data-ttu-id="494d6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="494d6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="494d6-129">响应</span><span class="sxs-lookup"><span data-stu-id="494d6-129">Response</span></span>

<span data-ttu-id="494d6-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [todoTask](../resources/todotask.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="494d6-130">If successful, this method returns a `200 OK` response code and a collection of [todoTask](../resources/todotask.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="494d6-131">示例</span><span class="sxs-lookup"><span data-stu-id="494d6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="494d6-132">请求</span><span class="sxs-lookup"><span data-stu-id="494d6-132">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["35e2-35e2-721a-e235-1a72e2351a7"],
  "name": "get_todotask"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/35e2-35e2-721a-e235-1a72e2351a7/tasks
```


### <a name="response"></a><span data-ttu-id="494d6-133">响应</span><span class="sxs-lookup"><span data-stu-id="494d6-133">Response</span></span>
<span data-ttu-id="494d6-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="494d6-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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



