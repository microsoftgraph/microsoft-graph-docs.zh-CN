---
title: 获取 linkedResource
description: 读取 linkedResource 对象的属性和关系。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 830a7aba64221e1eb6918c0c66deb636a391d0d0
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873813"
---
# <a name="get-linkedresource"></a><span data-ttu-id="8610d-103">获取 linkedResource</span><span class="sxs-lookup"><span data-stu-id="8610d-103">Get linkedResource</span></span>
<span data-ttu-id="8610d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8610d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8610d-105">读取 [linkedResource 对象的属性和](../resources/linkedresource.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="8610d-105">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8610d-106">权限</span><span class="sxs-lookup"><span data-stu-id="8610d-106">Permissions</span></span>
<span data-ttu-id="8610d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8610d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8610d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8610d-109">Permission type</span></span>|<span data-ttu-id="8610d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8610d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8610d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8610d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8610d-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8610d-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="8610d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8610d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8610d-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8610d-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="8610d-115">应用</span><span class="sxs-lookup"><span data-stu-id="8610d-115">Application</span></span>|<span data-ttu-id="8610d-116">不支持</span><span class="sxs-lookup"><span data-stu-id="8610d-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="8610d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8610d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="8610d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8610d-118">Request headers</span></span>
|<span data-ttu-id="8610d-119">名称</span><span class="sxs-lookup"><span data-stu-id="8610d-119">Name</span></span>|<span data-ttu-id="8610d-120">说明</span><span class="sxs-lookup"><span data-stu-id="8610d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8610d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8610d-121">Authorization</span></span>|<span data-ttu-id="8610d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8610d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8610d-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8610d-124">Request body</span></span>
<span data-ttu-id="8610d-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8610d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8610d-126">响应</span><span class="sxs-lookup"><span data-stu-id="8610d-126">Response</span></span>

<span data-ttu-id="8610d-127">如果成功，此方法在响应 `200 OK` 正文中返回响应代码和 [linkedResource](../resources/linkedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8610d-127">If successful, this method returns a `200 OK` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8610d-128">示例</span><span class="sxs-lookup"><span data-stu-id="8610d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8610d-129">请求</span><span class="sxs-lookup"><span data-stu-id="8610d-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8610d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="8610d-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "get_linkedresource"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
```
# <a name="c"></a>[<span data-ttu-id="8610d-131">C#</span><span class="sxs-lookup"><span data-stu-id="8610d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8610d-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8610d-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8610d-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8610d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8610d-134">Java</span><span class="sxs-lookup"><span data-stu-id="8610d-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-linkedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8610d-135">响应</span><span class="sxs-lookup"><span data-stu-id="8610d-135">Response</span></span>
<span data-ttu-id="8610d-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8610d-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.linkedResource"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
     "@odata.type": "#microsoft.graph.linkedResource",
      "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
      "webUrl": "http://microsoft.com",
      "applicationName": "Microsoft",
      "displayName": "Microsoft",
      "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
  }
}
```


