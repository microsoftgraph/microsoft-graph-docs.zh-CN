---
title: 获取 todoTaskList
description: 读取 todoTaskList 对象的属性和关系。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 215f791f5a845df3de07166550055fca22f50735
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873203"
---
# <a name="get-todotasklist"></a><span data-ttu-id="9d21f-103">获取 todoTaskList</span><span class="sxs-lookup"><span data-stu-id="9d21f-103">Get todoTaskList</span></span>
<span data-ttu-id="9d21f-104">命名空间： microsoft. graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="9d21f-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="9d21f-105">读取 [todoTaskList](../resources/todotasklist.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9d21f-105">Read the properties and relationships of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d21f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9d21f-106">Permissions</span></span>
<span data-ttu-id="9d21f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d21f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d21f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d21f-109">Permission type</span></span>|<span data-ttu-id="9d21f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9d21f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d21f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d21f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9d21f-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d21f-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="9d21f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d21f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d21f-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d21f-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="9d21f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d21f-115">Application</span></span>|<span data-ttu-id="9d21f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d21f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d21f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d21f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9d21f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9d21f-118">Optional query parameters</span></span>
<span data-ttu-id="9d21f-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9d21f-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d21f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d21f-120">Request headers</span></span>
|<span data-ttu-id="9d21f-121">名称</span><span class="sxs-lookup"><span data-stu-id="9d21f-121">Name</span></span>|<span data-ttu-id="9d21f-122">说明</span><span class="sxs-lookup"><span data-stu-id="9d21f-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9d21f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d21f-123">Authorization</span></span>|<span data-ttu-id="9d21f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9d21f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d21f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d21f-126">Request body</span></span>
<span data-ttu-id="9d21f-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9d21f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d21f-128">响应</span><span class="sxs-lookup"><span data-stu-id="9d21f-128">Response</span></span>

<span data-ttu-id="9d21f-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [todoTaskList](../resources/todotasklist.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9d21f-129">If successful, this method returns a `200 OK` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9d21f-130">示例</span><span class="sxs-lookup"><span data-stu-id="9d21f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9d21f-131">请求</span><span class="sxs-lookup"><span data-stu-id="9d21f-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9d21f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d21f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAAABrJAAA="],
  "name": "get_todotasklist"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/AAMkADIyAAAAABrJAAA=
```
# <a name="c"></a>[<span data-ttu-id="9d21f-133">C#</span><span class="sxs-lookup"><span data-stu-id="9d21f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d21f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d21f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d21f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d21f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9d21f-136">响应</span><span class="sxs-lookup"><span data-stu-id="9d21f-136">Response</span></span>
<span data-ttu-id="9d21f-137">**注意：** 下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9d21f-137">**Note:** Here is an example of the response.</span></span> <span data-ttu-id="9d21f-138">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9d21f-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9d21f-139">将从实际调用中返回所有属性。。</span><span class="sxs-lookup"><span data-stu-id="9d21f-139">All of the properties will be returned from an actual call..</span></span>
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

