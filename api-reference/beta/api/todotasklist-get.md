---
title: 获取 todoTaskList
description: 读取 todoTaskList 对象的属性和关系。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8557c44cac027094d4420eca2dc57f9a691f1bf8
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873281"
---
# <a name="get-todotasklist"></a><span data-ttu-id="af080-103">获取 todoTaskList</span><span class="sxs-lookup"><span data-stu-id="af080-103">Get todoTaskList</span></span>
<span data-ttu-id="af080-104">命名空间：microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="af080-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="af080-105">读取 [todoTaskList 对象的属性和](../resources/todotasklist.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="af080-105">Read the properties and relationships of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="af080-106">权限</span><span class="sxs-lookup"><span data-stu-id="af080-106">Permissions</span></span>
<span data-ttu-id="af080-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="af080-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af080-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="af080-109">Permission type</span></span>|<span data-ttu-id="af080-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="af080-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af080-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="af080-111">Delegated (work or school account)</span></span>|<span data-ttu-id="af080-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af080-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="af080-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="af080-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af080-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af080-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="af080-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="af080-115">Application</span></span>|<span data-ttu-id="af080-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="af080-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af080-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="af080-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="af080-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="af080-118">Optional query parameters</span></span>
<span data-ttu-id="af080-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="af080-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="af080-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="af080-120">Request headers</span></span>
|<span data-ttu-id="af080-121">名称</span><span class="sxs-lookup"><span data-stu-id="af080-121">Name</span></span>|<span data-ttu-id="af080-122">说明</span><span class="sxs-lookup"><span data-stu-id="af080-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="af080-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="af080-123">Authorization</span></span>|<span data-ttu-id="af080-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="af080-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="af080-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="af080-126">Request body</span></span>
<span data-ttu-id="af080-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="af080-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af080-128">响应</span><span class="sxs-lookup"><span data-stu-id="af080-128">Response</span></span>

<span data-ttu-id="af080-129">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [todoTaskList](../resources/todotasklist.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="af080-129">If successful, this method returns a `200 OK` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="af080-130">示例</span><span class="sxs-lookup"><span data-stu-id="af080-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="af080-131">请求</span><span class="sxs-lookup"><span data-stu-id="af080-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="af080-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="af080-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAAABrJAAA="],
  "name": "get_todotasklist"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/AAMkADIyAAAAABrJAAA=
```
# <a name="c"></a>[<span data-ttu-id="af080-133">C#</span><span class="sxs-lookup"><span data-stu-id="af080-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af080-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af080-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af080-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af080-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="af080-136">Java</span><span class="sxs-lookup"><span data-stu-id="af080-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-todotasklist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="af080-137">响应</span><span class="sxs-lookup"><span data-stu-id="af080-137">Response</span></span>
><span data-ttu-id="af080-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="af080-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "value": {
    "@odata.type": "#microsoft.graph.todoTaskList",
    "id": "5daae1ed-e1ed-5daa-ede1-aa5dede1aa5d",
    "displayName": "Monthly tasks",
    "isOwner": "true",
    "isShared": "false",
    "wellknownListName": "defaultList"
  }
}
```



