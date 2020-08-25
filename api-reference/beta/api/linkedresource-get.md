---
title: 获取 linkedResource
description: 读取 linkedResource 对象的属性和关系。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e041281a1922fce22f9e9b5ab8d38d1d0e572359
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873050"
---
# <a name="get-linkedresource"></a><span data-ttu-id="0ce53-103">获取 linkedResource</span><span class="sxs-lookup"><span data-stu-id="0ce53-103">Get linkedResource</span></span>
<span data-ttu-id="0ce53-104">命名空间： microsoft. graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="0ce53-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="0ce53-105">读取 [linkedResource](../resources/linkedresource.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0ce53-105">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ce53-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0ce53-106">Permissions</span></span>
<span data-ttu-id="0ce53-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ce53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ce53-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ce53-109">Permission type</span></span>|<span data-ttu-id="0ce53-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0ce53-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ce53-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ce53-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0ce53-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ce53-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="0ce53-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ce53-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ce53-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ce53-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="0ce53-115">应用</span><span class="sxs-lookup"><span data-stu-id="0ce53-115">Application</span></span>|<span data-ttu-id="0ce53-116">不支持</span><span class="sxs-lookup"><span data-stu-id="0ce53-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ce53-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ce53-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="0ce53-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ce53-118">Request headers</span></span>
|<span data-ttu-id="0ce53-119">名称</span><span class="sxs-lookup"><span data-stu-id="0ce53-119">Name</span></span>|<span data-ttu-id="0ce53-120">说明</span><span class="sxs-lookup"><span data-stu-id="0ce53-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0ce53-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ce53-121">Authorization</span></span>|<span data-ttu-id="0ce53-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ce53-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ce53-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ce53-124">Request body</span></span>
<span data-ttu-id="0ce53-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0ce53-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ce53-126">响应</span><span class="sxs-lookup"><span data-stu-id="0ce53-126">Response</span></span>

<span data-ttu-id="0ce53-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [linkedResource](../resources/linkedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0ce53-127">If successful, this method returns a `200 OK` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ce53-128">示例</span><span class="sxs-lookup"><span data-stu-id="0ce53-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ce53-129">请求</span><span class="sxs-lookup"><span data-stu-id="0ce53-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0ce53-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ce53-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "get_linkedresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
```
# <a name="c"></a>[<span data-ttu-id="0ce53-131">C#</span><span class="sxs-lookup"><span data-stu-id="0ce53-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ce53-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ce53-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ce53-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ce53-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0ce53-134">响应</span><span class="sxs-lookup"><span data-stu-id="0ce53-134">Response</span></span>
<span data-ttu-id="0ce53-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0ce53-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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
