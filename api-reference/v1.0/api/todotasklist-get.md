---
title: 获取 todoTaskList
description: 读取 todoTaskList 对象的属性和关系。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f7aced0d3e023eacfde6faaecc8c63836bbb44b7
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797268"
---
# <a name="get-todotasklist"></a><span data-ttu-id="8aba8-103">获取 todoTaskList</span><span class="sxs-lookup"><span data-stu-id="8aba8-103">Get todoTaskList</span></span>
<span data-ttu-id="8aba8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8aba8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8aba8-105">读取 [todoTaskList](../resources/todotasklist.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8aba8-105">Read the properties and relationships of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8aba8-106">权限</span><span class="sxs-lookup"><span data-stu-id="8aba8-106">Permissions</span></span>
<span data-ttu-id="8aba8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8aba8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8aba8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8aba8-109">Permission type</span></span>|<span data-ttu-id="8aba8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8aba8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8aba8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8aba8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8aba8-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8aba8-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="8aba8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8aba8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8aba8-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8aba8-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="8aba8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8aba8-115">Application</span></span>|<span data-ttu-id="8aba8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8aba8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8aba8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8aba8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8aba8-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8aba8-118">Optional query parameters</span></span>
<span data-ttu-id="8aba8-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8aba8-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8aba8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8aba8-120">Request headers</span></span>
|<span data-ttu-id="8aba8-121">名称</span><span class="sxs-lookup"><span data-stu-id="8aba8-121">Name</span></span>|<span data-ttu-id="8aba8-122">说明</span><span class="sxs-lookup"><span data-stu-id="8aba8-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8aba8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8aba8-123">Authorization</span></span>|<span data-ttu-id="8aba8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8aba8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8aba8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8aba8-126">Request body</span></span>
<span data-ttu-id="8aba8-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8aba8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8aba8-128">响应</span><span class="sxs-lookup"><span data-stu-id="8aba8-128">Response</span></span>

<span data-ttu-id="8aba8-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [todoTaskList](../resources/todotasklist.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8aba8-129">If successful, this method returns a `200 OK` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8aba8-130">示例</span><span class="sxs-lookup"><span data-stu-id="8aba8-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8aba8-131">请求</span><span class="sxs-lookup"><span data-stu-id="8aba8-131">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAAABrJAAA="],
  "name": "get_todotasklist"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADIyAAAAABrJAAA=
```


### <a name="response"></a><span data-ttu-id="8aba8-132">响应</span><span class="sxs-lookup"><span data-stu-id="8aba8-132">Response</span></span>
><span data-ttu-id="8aba8-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8aba8-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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



