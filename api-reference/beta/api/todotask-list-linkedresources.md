---
title: 列出 linkedResources
description: 从 linkedResources 导航属性中获取 linkedResources。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 34edae5bbaaed3484e913d16963c0650864d7e7f
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849891"
---
# <a name="list-linkedresources"></a><span data-ttu-id="03c3c-103">列出 linkedResources</span><span class="sxs-lookup"><span data-stu-id="03c3c-103">List linkedResources</span></span>
<span data-ttu-id="03c3c-104">命名空间：microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="03c3c-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="03c3c-105">从 linkedResources 导航属性中获取 linkedResources。</span><span class="sxs-lookup"><span data-stu-id="03c3c-105">Get the linkedResources from the linkedResources navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="03c3c-106">权限</span><span class="sxs-lookup"><span data-stu-id="03c3c-106">Permissions</span></span>
<span data-ttu-id="03c3c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03c3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03c3c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="03c3c-109">Permission type</span></span>|<span data-ttu-id="03c3c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="03c3c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03c3c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03c3c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="03c3c-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03c3c-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="03c3c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03c3c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03c3c-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03c3c-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="03c3c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="03c3c-115">Application</span></span>|<span data-ttu-id="03c3c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="03c3c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03c3c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03c3c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="03c3c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="03c3c-118">Optional query parameters</span></span>
<span data-ttu-id="03c3c-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="03c3c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="03c3c-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="03c3c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="03c3c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="03c3c-121">Request headers</span></span>
|<span data-ttu-id="03c3c-122">名称</span><span class="sxs-lookup"><span data-stu-id="03c3c-122">Name</span></span>|<span data-ttu-id="03c3c-123">说明</span><span class="sxs-lookup"><span data-stu-id="03c3c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="03c3c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="03c3c-124">Authorization</span></span>|<span data-ttu-id="03c3c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="03c3c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03c3c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="03c3c-127">Request body</span></span>
<span data-ttu-id="03c3c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="03c3c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03c3c-129">响应</span><span class="sxs-lookup"><span data-stu-id="03c3c-129">Response</span></span>

<span data-ttu-id="03c3c-130">如果成功，此方法在响应 `200 OK` 正文中返回响应代码和 [linkedResource](../resources/linkedresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="03c3c-130">If successful, this method returns a `200 OK` response code and a collection of [linkedResource](../resources/linkedresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="03c3c-131">示例</span><span class="sxs-lookup"><span data-stu-id="03c3c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="03c3c-132">请求</span><span class="sxs-lookup"><span data-stu-id="03c3c-132">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "get_linkedresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
```


### <a name="response"></a><span data-ttu-id="03c3c-133">响应</span><span class="sxs-lookup"><span data-stu-id="03c3c-133">Response</span></span>
<span data-ttu-id="03c3c-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="03c3c-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.linkedResource)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.linkedResource",
      "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
      "webUrl": "http:://microsoft.com",
      "applicationName": "Microsoft",
      "displayName": "Microsoft",
      "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
    }
  ]
}
```

