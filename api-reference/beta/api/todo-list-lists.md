---
title: 列出列表
description: 获取 todoTaskList 对象及其属性的列表。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c4735dff24dbccb8fbb7106a819b0b36bb132d01
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953817"
---
# <a name="list-lists"></a><span data-ttu-id="60b4c-103">列出列表</span><span class="sxs-lookup"><span data-stu-id="60b4c-103">List lists</span></span>
<span data-ttu-id="60b4c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60b4c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="60b4c-105">获取 [todoTaskList 对象](../resources/todotasklist.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="60b4c-105">Get a list of the [todoTaskList](../resources/todotasklist.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="60b4c-106">权限</span><span class="sxs-lookup"><span data-stu-id="60b4c-106">Permissions</span></span>
<span data-ttu-id="60b4c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60b4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60b4c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="60b4c-109">Permission type</span></span>|<span data-ttu-id="60b4c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="60b4c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60b4c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60b4c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="60b4c-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60b4c-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="60b4c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60b4c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60b4c-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60b4c-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="60b4c-115">应用</span><span class="sxs-lookup"><span data-stu-id="60b4c-115">Application</span></span>|<span data-ttu-id="60b4c-116">不支持</span><span class="sxs-lookup"><span data-stu-id="60b4c-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="60b4c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60b4c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists
GET /users/{id|userPrincipalName}/todo/lists
```

## <a name="optional-query-parameters"></a><span data-ttu-id="60b4c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="60b4c-118">Optional query parameters</span></span>
<span data-ttu-id="60b4c-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="60b4c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="60b4c-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="60b4c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="60b4c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="60b4c-121">Request headers</span></span>
|<span data-ttu-id="60b4c-122">名称</span><span class="sxs-lookup"><span data-stu-id="60b4c-122">Name</span></span>|<span data-ttu-id="60b4c-123">说明</span><span class="sxs-lookup"><span data-stu-id="60b4c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="60b4c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="60b4c-124">Authorization</span></span>|<span data-ttu-id="60b4c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="60b4c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60b4c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="60b4c-127">Request body</span></span>
<span data-ttu-id="60b4c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="60b4c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60b4c-129">响应</span><span class="sxs-lookup"><span data-stu-id="60b4c-129">Response</span></span>

<span data-ttu-id="60b4c-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [todoTaskList](../resources/todotasklist.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="60b4c-130">If successful, this method returns a `200 OK` response code and a collection of [todoTaskList](../resources/todotasklist.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60b4c-131">示例</span><span class="sxs-lookup"><span data-stu-id="60b4c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="60b4c-132">请求</span><span class="sxs-lookup"><span data-stu-id="60b4c-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="60b4c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="60b4c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_todotasklist_1"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists
```
# <a name="c"></a>[<span data-ttu-id="60b4c-134">C#</span><span class="sxs-lookup"><span data-stu-id="60b4c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotasklist-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60b4c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60b4c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotasklist-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60b4c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60b4c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotasklist-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="60b4c-137">Java</span><span class="sxs-lookup"><span data-stu-id="60b4c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-todotasklist-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="60b4c-138">响应</span><span class="sxs-lookup"><span data-stu-id="60b4c-138">Response</span></span>
<span data-ttu-id="60b4c-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="60b4c-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.todoTaskList)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.todoTaskList",
      "id": "AAMkADIyAAAAABrJAAA=",
      "displayName": "Tasks",
      "isOwner": true,
      "isShared": false,
      "wellknownListName": "defaultList"
    },
        {
      "@odata.type": "#microsoft.graph.todoTaskList",
      "id": "AAMkADIyAAAEFTTrJAAA=",
      "displayName": "Monthly Tasks",
      "isOwner":true,
      "isShared": false,
      "wellknownListName": "none"
    }
  ]
}
```



