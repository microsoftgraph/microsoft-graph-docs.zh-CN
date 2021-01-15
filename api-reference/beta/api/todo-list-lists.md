---
title: 列出列表
description: 获取 todoTaskList 对象及其属性的列表。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 67e6bc042770381112f8c44f8e4e51111de8035f
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873799"
---
# <a name="list-lists"></a><span data-ttu-id="f5710-103">列出列表</span><span class="sxs-lookup"><span data-stu-id="f5710-103">List lists</span></span>
<span data-ttu-id="f5710-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5710-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f5710-105">获取 [todoTaskList](../resources/todotasklist.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="f5710-105">Get a list of the [todoTaskList](../resources/todotasklist.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5710-106">权限</span><span class="sxs-lookup"><span data-stu-id="f5710-106">Permissions</span></span>
<span data-ttu-id="f5710-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5710-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5710-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5710-109">Permission type</span></span>|<span data-ttu-id="f5710-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f5710-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5710-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5710-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f5710-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5710-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f5710-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5710-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5710-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5710-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f5710-115">应用</span><span class="sxs-lookup"><span data-stu-id="f5710-115">Application</span></span>|<span data-ttu-id="f5710-116">不支持</span><span class="sxs-lookup"><span data-stu-id="f5710-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5710-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5710-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists
GET /users/{id|userPrincipalName}/todo/lists
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f5710-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f5710-118">Optional query parameters</span></span>
<span data-ttu-id="f5710-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f5710-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f5710-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f5710-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5710-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5710-121">Request headers</span></span>
|<span data-ttu-id="f5710-122">名称</span><span class="sxs-lookup"><span data-stu-id="f5710-122">Name</span></span>|<span data-ttu-id="f5710-123">说明</span><span class="sxs-lookup"><span data-stu-id="f5710-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f5710-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5710-124">Authorization</span></span>|<span data-ttu-id="f5710-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f5710-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5710-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5710-127">Request body</span></span>
<span data-ttu-id="f5710-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f5710-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5710-129">响应</span><span class="sxs-lookup"><span data-stu-id="f5710-129">Response</span></span>

<span data-ttu-id="f5710-130">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [todoTaskList](../resources/todotasklist.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f5710-130">If successful, this method returns a `200 OK` response code and a collection of [todoTaskList](../resources/todotasklist.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f5710-131">示例</span><span class="sxs-lookup"><span data-stu-id="f5710-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f5710-132">请求</span><span class="sxs-lookup"><span data-stu-id="f5710-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f5710-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5710-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_todotasklist"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists
```
# <a name="c"></a>[<span data-ttu-id="f5710-134">C#</span><span class="sxs-lookup"><span data-stu-id="f5710-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5710-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5710-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5710-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5710-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5710-137">Java</span><span class="sxs-lookup"><span data-stu-id="f5710-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-todotasklist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f5710-138">响应</span><span class="sxs-lookup"><span data-stu-id="f5710-138">Response</span></span>
<span data-ttu-id="f5710-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f5710-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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



