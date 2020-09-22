---
title: 获取 todoTask
description: 读取 todoTask 对象的属性和关系。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 39f12ab34ce57367cb97f22ac8188b1dac1c35e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058599"
---
# <a name="get-todotask"></a><span data-ttu-id="4271c-103">获取 todoTask</span><span class="sxs-lookup"><span data-stu-id="4271c-103">Get todoTask</span></span>
<span data-ttu-id="4271c-104">命名空间： microsoft. graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="4271c-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="4271c-105">读取 [todoTask](../resources/todotask.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4271c-105">Read the properties and relationships of a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4271c-106">权限</span><span class="sxs-lookup"><span data-stu-id="4271c-106">Permissions</span></span>
<span data-ttu-id="4271c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4271c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4271c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4271c-109">Permission type</span></span>|<span data-ttu-id="4271c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4271c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4271c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4271c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4271c-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4271c-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="4271c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4271c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4271c-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4271c-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="4271c-115">应用</span><span class="sxs-lookup"><span data-stu-id="4271c-115">Application</span></span>|<span data-ttu-id="4271c-116">不支持</span><span class="sxs-lookup"><span data-stu-id="4271c-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="4271c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4271c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4271c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4271c-118">Optional query parameters</span></span>
<span data-ttu-id="4271c-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4271c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4271c-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="4271c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4271c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4271c-121">Request headers</span></span>
|<span data-ttu-id="4271c-122">名称</span><span class="sxs-lookup"><span data-stu-id="4271c-122">Name</span></span>|<span data-ttu-id="4271c-123">说明</span><span class="sxs-lookup"><span data-stu-id="4271c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4271c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4271c-124">Authorization</span></span>|<span data-ttu-id="4271c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4271c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4271c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4271c-127">Request body</span></span>
<span data-ttu-id="4271c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4271c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4271c-129">响应</span><span class="sxs-lookup"><span data-stu-id="4271c-129">Response</span></span>

<span data-ttu-id="4271c-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [todoTask](../resources/todotask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4271c-130">If successful, this method returns a `200 OK` response code and a [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4271c-131">示例</span><span class="sxs-lookup"><span data-stu-id="4271c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4271c-132">请求</span><span class="sxs-lookup"><span data-stu-id="4271c-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4271c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4271c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "name": "get_todotask"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
```
# <a name="c"></a>[<span data-ttu-id="4271c-134">C#</span><span class="sxs-lookup"><span data-stu-id="4271c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4271c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4271c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4271c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4271c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4271c-137">响应</span><span class="sxs-lookup"><span data-stu-id="4271c-137">Response</span></span>
<span data-ttu-id="4271c-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4271c-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.todoTask"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tasks/$entity",
    "@odata.etag": "W/\"s8/ERWT3WEeFpBGD0bDgAA+TWq9g==\"",
    "importance": "low",
    "isReminderOn": false,
    "status": "notStarted",
    "title": "Shop for dinner",
    "createdDateTime": "2020-07-22T10:39:03.7937971Z",
    "lastModifiedDateTime": "2020-07-22T12:02:10.8835421Z",
    "id": "721a35e2-35e2-721a-e235-1a72e2351a72",
    "body": {
        "content": "",
        "contentType": "text"
    },
    "dueDateTime": {
        "dateTime": "2020-08-25T04:00:00.0000000",
        "timeZone": "UTC"
    }
}
```



