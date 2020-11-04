---
title: 更新 linkedResource
description: 更新 linkedResource 对象的属性。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0afbda988d1bdac20e6ff966a1ab51b31b075a62
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903403"
---
# <a name="update-linkedresource"></a><span data-ttu-id="fa4e2-103">更新 linkedResource</span><span class="sxs-lookup"><span data-stu-id="fa4e2-103">Update linkedResource</span></span>
<span data-ttu-id="fa4e2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa4e2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fa4e2-105">更新 [linkedResource](../resources/linkedresource.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fa4e2-105">Update the properties of a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa4e2-106">权限</span><span class="sxs-lookup"><span data-stu-id="fa4e2-106">Permissions</span></span>
<span data-ttu-id="fa4e2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa4e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa4e2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa4e2-109">Permission type</span></span>|<span data-ttu-id="fa4e2-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fa4e2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa4e2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa4e2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fa4e2-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa4e2-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="fa4e2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa4e2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa4e2-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa4e2-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="fa4e2-115">应用</span><span class="sxs-lookup"><span data-stu-id="fa4e2-115">Application</span></span>|<span data-ttu-id="fa4e2-116">不支持</span><span class="sxs-lookup"><span data-stu-id="fa4e2-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa4e2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa4e2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="fa4e2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa4e2-118">Request headers</span></span>
|<span data-ttu-id="fa4e2-119">名称</span><span class="sxs-lookup"><span data-stu-id="fa4e2-119">Name</span></span>|<span data-ttu-id="fa4e2-120">说明</span><span class="sxs-lookup"><span data-stu-id="fa4e2-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fa4e2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa4e2-121">Authorization</span></span>|<span data-ttu-id="fa4e2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fa4e2-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fa4e2-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa4e2-124">Content-Type</span></span>|<span data-ttu-id="fa4e2-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="fa4e2-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa4e2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa4e2-127">Request body</span></span>
<span data-ttu-id="fa4e2-128">在请求正文中，提供 [linkedResource](../resources/linkedresource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa4e2-128">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="fa4e2-129">下表显示了在更新 [linkedResource](../resources/linkedresource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fa4e2-129">The following table shows the properties that are required when you update the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="fa4e2-130">属性</span><span class="sxs-lookup"><span data-stu-id="fa4e2-130">Property</span></span>|<span data-ttu-id="fa4e2-131">类型</span><span class="sxs-lookup"><span data-stu-id="fa4e2-131">Type</span></span>|<span data-ttu-id="fa4e2-132">说明</span><span class="sxs-lookup"><span data-stu-id="fa4e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa4e2-133">id</span><span class="sxs-lookup"><span data-stu-id="fa4e2-133">id</span></span>|<span data-ttu-id="fa4e2-134">String</span><span class="sxs-lookup"><span data-stu-id="fa4e2-134">String</span></span>|<span data-ttu-id="fa4e2-135">从[实体](../resources/entity.md)继承的链接实体的服务器生成 Id</span><span class="sxs-lookup"><span data-stu-id="fa4e2-135">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|

## <a name="response"></a><span data-ttu-id="fa4e2-136">响应</span><span class="sxs-lookup"><span data-stu-id="fa4e2-136">Response</span></span>

<span data-ttu-id="fa4e2-137">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [linkedResource](../resources/linkedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fa4e2-137">If successful, this method returns a `200 OK` response code and an updated [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa4e2-138">示例</span><span class="sxs-lookup"><span data-stu-id="fa4e2-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fa4e2-139">请求</span><span class="sxs-lookup"><span data-stu-id="fa4e2-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fa4e2-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa4e2-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "update_linkedresource"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
Content-Type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "webUrl": "http://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft"
}
```
# <a name="c"></a>[<span data-ttu-id="fa4e2-141">C#</span><span class="sxs-lookup"><span data-stu-id="fa4e2-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa4e2-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa4e2-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa4e2-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa4e2-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fa4e2-144">Java</span><span class="sxs-lookup"><span data-stu-id="fa4e2-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-linkedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="fa4e2-145">响应</span><span class="sxs-lookup"><span data-stu-id="fa4e2-145">Response</span></span>
<span data-ttu-id="fa4e2-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fa4e2-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.type": "#microsoft.graph.linkedResource",
  "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
  "webUrl": "http://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```


