---
title: 获取 todoTaskList
description: 读取 todoTaskList 对象的属性和关系。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1c26a61e95e213b10ad7894d02a30d38bd781970
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314746"
---
# <a name="get-todotasklist"></a><span data-ttu-id="9b5b0-103">获取 todoTaskList</span><span class="sxs-lookup"><span data-stu-id="9b5b0-103">Get todoTaskList</span></span>
<span data-ttu-id="9b5b0-104">命名空间： microsoft. graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="9b5b0-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="9b5b0-105">读取 [todoTaskList](../resources/todotasklist.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9b5b0-105">Read the properties and relationships of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b5b0-106">权限</span><span class="sxs-lookup"><span data-stu-id="9b5b0-106">Permissions</span></span>
<span data-ttu-id="9b5b0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b5b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b5b0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b5b0-109">Permission type</span></span>|<span data-ttu-id="9b5b0-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9b5b0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b5b0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b5b0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9b5b0-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b5b0-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="9b5b0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b5b0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b5b0-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b5b0-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="9b5b0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b5b0-115">Application</span></span>|<span data-ttu-id="9b5b0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b5b0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b5b0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b5b0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9b5b0-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9b5b0-118">Optional query parameters</span></span>
<span data-ttu-id="9b5b0-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9b5b0-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b5b0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b5b0-120">Request headers</span></span>
|<span data-ttu-id="9b5b0-121">名称</span><span class="sxs-lookup"><span data-stu-id="9b5b0-121">Name</span></span>|<span data-ttu-id="9b5b0-122">说明</span><span class="sxs-lookup"><span data-stu-id="9b5b0-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9b5b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b5b0-123">Authorization</span></span>|<span data-ttu-id="9b5b0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9b5b0-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b5b0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b5b0-126">Request body</span></span>
<span data-ttu-id="9b5b0-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9b5b0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b5b0-128">响应</span><span class="sxs-lookup"><span data-stu-id="9b5b0-128">Response</span></span>

<span data-ttu-id="9b5b0-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [todoTaskList](../resources/todotasklist.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9b5b0-129">If successful, this method returns a `200 OK` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9b5b0-130">示例</span><span class="sxs-lookup"><span data-stu-id="9b5b0-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9b5b0-131">请求</span><span class="sxs-lookup"><span data-stu-id="9b5b0-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9b5b0-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b5b0-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAAABrJAAA="],
  "name": "get_todotasklist"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/AAMkADIyAAAAABrJAAA=
```
# <a name="c"></a>[<span data-ttu-id="9b5b0-133">C#</span><span class="sxs-lookup"><span data-stu-id="9b5b0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b5b0-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b5b0-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b5b0-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b5b0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="9b5b0-136">响应</span><span class="sxs-lookup"><span data-stu-id="9b5b0-136">Response</span></span>
><span data-ttu-id="9b5b0-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9b5b0-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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



