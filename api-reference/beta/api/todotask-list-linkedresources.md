---
title: 列出 linkedResources
description: 从 linkedResources 导航属性中获取 linkedResources。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c3d780e05c71112ddabd1d5d6a64b22d6f771d40
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873256"
---
# <a name="list-linkedresources"></a><span data-ttu-id="948f2-103">列出 linkedResources</span><span class="sxs-lookup"><span data-stu-id="948f2-103">List linkedResources</span></span>
<span data-ttu-id="948f2-104">命名空间： microsoft. graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="948f2-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="948f2-105">从 linkedResources 导航属性中获取 linkedResources。</span><span class="sxs-lookup"><span data-stu-id="948f2-105">Get the linkedResources from the linkedResources navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="948f2-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="948f2-106">Permissions</span></span>
<span data-ttu-id="948f2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="948f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="948f2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="948f2-109">Permission type</span></span>|<span data-ttu-id="948f2-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="948f2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="948f2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="948f2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="948f2-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="948f2-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="948f2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="948f2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="948f2-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="948f2-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="948f2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="948f2-115">Application</span></span>|<span data-ttu-id="948f2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="948f2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="948f2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="948f2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="948f2-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="948f2-118">Optional query parameters</span></span>
<span data-ttu-id="948f2-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="948f2-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="948f2-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="948f2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="948f2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="948f2-121">Request headers</span></span>
|<span data-ttu-id="948f2-122">名称</span><span class="sxs-lookup"><span data-stu-id="948f2-122">Name</span></span>|<span data-ttu-id="948f2-123">说明</span><span class="sxs-lookup"><span data-stu-id="948f2-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="948f2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="948f2-124">Authorization</span></span>|<span data-ttu-id="948f2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="948f2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="948f2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="948f2-127">Request body</span></span>
<span data-ttu-id="948f2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="948f2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="948f2-129">响应</span><span class="sxs-lookup"><span data-stu-id="948f2-129">Response</span></span>

<span data-ttu-id="948f2-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [linkedResource](../resources/linkedresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="948f2-130">If successful, this method returns a `200 OK` response code and a collection of [linkedResource](../resources/linkedresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="948f2-131">示例</span><span class="sxs-lookup"><span data-stu-id="948f2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="948f2-132">请求</span><span class="sxs-lookup"><span data-stu-id="948f2-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="948f2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="948f2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "get_linkedresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
```
# <a name="c"></a>[<span data-ttu-id="948f2-134">C#</span><span class="sxs-lookup"><span data-stu-id="948f2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="948f2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="948f2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="948f2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="948f2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="948f2-137">响应</span><span class="sxs-lookup"><span data-stu-id="948f2-137">Response</span></span>
<span data-ttu-id="948f2-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="948f2-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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

