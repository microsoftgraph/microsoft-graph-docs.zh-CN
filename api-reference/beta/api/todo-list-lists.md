---
title: 列表列表
description: 获取 todoTaskList 对象及其属性的列表。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 87b7cad3f24d8e0db1632edd43454a55d05e64b0
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849902"
---
# <a name="list-lists"></a><span data-ttu-id="1e32a-103">列表列表</span><span class="sxs-lookup"><span data-stu-id="1e32a-103">List lists</span></span>
<span data-ttu-id="1e32a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e32a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1e32a-105">获取 [todoTaskList 对象](../resources/todotasklist.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="1e32a-105">Get a list of the [todoTaskList](../resources/todotasklist.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e32a-106">权限</span><span class="sxs-lookup"><span data-stu-id="1e32a-106">Permissions</span></span>
<span data-ttu-id="1e32a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e32a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e32a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e32a-109">Permission type</span></span>|<span data-ttu-id="1e32a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1e32a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e32a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e32a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1e32a-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e32a-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="1e32a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e32a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e32a-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e32a-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="1e32a-115">应用</span><span class="sxs-lookup"><span data-stu-id="1e32a-115">Application</span></span>|<span data-ttu-id="1e32a-116">不支持</span><span class="sxs-lookup"><span data-stu-id="1e32a-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e32a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e32a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists
GET /users/{id|userPrincipalName}/todo/lists
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1e32a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1e32a-118">Optional query parameters</span></span>
<span data-ttu-id="1e32a-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1e32a-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1e32a-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="1e32a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e32a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e32a-121">Request headers</span></span>
|<span data-ttu-id="1e32a-122">名称</span><span class="sxs-lookup"><span data-stu-id="1e32a-122">Name</span></span>|<span data-ttu-id="1e32a-123">说明</span><span class="sxs-lookup"><span data-stu-id="1e32a-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1e32a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e32a-124">Authorization</span></span>|<span data-ttu-id="1e32a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1e32a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e32a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e32a-127">Request body</span></span>
<span data-ttu-id="1e32a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1e32a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e32a-129">响应</span><span class="sxs-lookup"><span data-stu-id="1e32a-129">Response</span></span>

<span data-ttu-id="1e32a-130">如果成功，此方法在响应 `200 OK` 正文中返回响应代码和 [todoTaskList](../resources/todotasklist.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1e32a-130">If successful, this method returns a `200 OK` response code and a collection of [todoTaskList](../resources/todotasklist.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1e32a-131">示例</span><span class="sxs-lookup"><span data-stu-id="1e32a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1e32a-132">请求</span><span class="sxs-lookup"><span data-stu-id="1e32a-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_todotasklist"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists
```


### <a name="response"></a><span data-ttu-id="1e32a-133">响应</span><span class="sxs-lookup"><span data-stu-id="1e32a-133">Response</span></span>
<span data-ttu-id="1e32a-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1e32a-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

