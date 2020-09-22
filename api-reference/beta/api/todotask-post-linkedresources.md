---
title: 创建 linkedResources
description: 创建新的 linkedResources 对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e5a5a702c55db40c77304c577b440f34dc610e8b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058583"
---
# <a name="create-linkedresources"></a><span data-ttu-id="e0883-103">创建 linkedResources</span><span class="sxs-lookup"><span data-stu-id="e0883-103">Create linkedResources</span></span>
<span data-ttu-id="e0883-104">命名空间： microsoft. graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="e0883-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="e0883-105">创建新的 linkedResources 对象。</span><span class="sxs-lookup"><span data-stu-id="e0883-105">Create a new linkedResources object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0883-106">权限</span><span class="sxs-lookup"><span data-stu-id="e0883-106">Permissions</span></span>
<span data-ttu-id="e0883-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0883-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0883-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0883-109">Permission type</span></span>|<span data-ttu-id="e0883-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e0883-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0883-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0883-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e0883-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0883-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="e0883-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0883-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0883-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0883-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="e0883-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0883-115">Application</span></span>|<span data-ttu-id="e0883-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0883-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0883-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0883-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a><span data-ttu-id="e0883-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0883-118">Request headers</span></span>
|<span data-ttu-id="e0883-119">名称</span><span class="sxs-lookup"><span data-stu-id="e0883-119">Name</span></span>|<span data-ttu-id="e0883-120">说明</span><span class="sxs-lookup"><span data-stu-id="e0883-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e0883-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0883-121">Authorization</span></span>|<span data-ttu-id="e0883-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0883-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e0883-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0883-124">Content-Type</span></span>|<span data-ttu-id="e0883-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e0883-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0883-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0883-127">Request body</span></span>
<span data-ttu-id="e0883-128">在请求正文中，提供 [linkedResource](../resources/linkedresource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0883-128">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="e0883-129">下表显示创建 [linkedResource](../resources/linkedresource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e0883-129">The following table shows the properties that are required when you create the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="e0883-130">属性</span><span class="sxs-lookup"><span data-stu-id="e0883-130">Property</span></span>|<span data-ttu-id="e0883-131">类型</span><span class="sxs-lookup"><span data-stu-id="e0883-131">Type</span></span>|<span data-ttu-id="e0883-132">说明</span><span class="sxs-lookup"><span data-stu-id="e0883-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0883-133">id</span><span class="sxs-lookup"><span data-stu-id="e0883-133">id</span></span>|<span data-ttu-id="e0883-134">String</span><span class="sxs-lookup"><span data-stu-id="e0883-134">String</span></span>|<span data-ttu-id="e0883-135">从[实体](../resources/entity.md)继承的链接实体的服务器生成 Id</span><span class="sxs-lookup"><span data-stu-id="e0883-135">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="e0883-136">webUrl</span><span class="sxs-lookup"><span data-stu-id="e0883-136">webUrl</span></span>|<span data-ttu-id="e0883-137">String</span><span class="sxs-lookup"><span data-stu-id="e0883-137">String</span></span>|<span data-ttu-id="e0883-138">Deeplink 到链接实体</span><span class="sxs-lookup"><span data-stu-id="e0883-138">Deeplink to the linked entity</span></span> |
|<span data-ttu-id="e0883-139">applicationName</span><span class="sxs-lookup"><span data-stu-id="e0883-139">applicationName</span></span>|<span data-ttu-id="e0883-140">String</span><span class="sxs-lookup"><span data-stu-id="e0883-140">String</span></span>|<span data-ttu-id="e0883-141">指示发送链接实体的源的应用程序名称的字段</span><span class="sxs-lookup"><span data-stu-id="e0883-141">Field indicating app name of the source that is sending the linked entity</span></span> |
|<span data-ttu-id="e0883-142">displayName</span><span class="sxs-lookup"><span data-stu-id="e0883-142">displayName</span></span>|<span data-ttu-id="e0883-143">String</span><span class="sxs-lookup"><span data-stu-id="e0883-143">String</span></span>|<span data-ttu-id="e0883-144">指示链接实体的标题的字段。</span><span class="sxs-lookup"><span data-stu-id="e0883-144">Field indicating title of the linked entity.</span></span> |
|<span data-ttu-id="e0883-145">externalId</span><span class="sxs-lookup"><span data-stu-id="e0883-145">externalId</span></span>|<span data-ttu-id="e0883-146">String</span><span class="sxs-lookup"><span data-stu-id="e0883-146">String</span></span>|<span data-ttu-id="e0883-147">与第三方/合作伙伴系统上的此任务相关联的对象的 Id</span><span class="sxs-lookup"><span data-stu-id="e0883-147">Id of the object that is associated with this task on the third-party/partner system</span></span> |



## <a name="response"></a><span data-ttu-id="e0883-148">响应</span><span class="sxs-lookup"><span data-stu-id="e0883-148">Response</span></span>

<span data-ttu-id="e0883-149">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [linkedResource](../resources/linkedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0883-149">If successful, this method returns a `201 Created` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e0883-150">示例</span><span class="sxs-lookup"><span data-stu-id="e0883-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e0883-151">请求</span><span class="sxs-lookup"><span data-stu-id="e0883-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e0883-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0883-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "create_linkedresource_from_linkedresources"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
Content-Type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "webUrl": "http:://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="e0883-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0883-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-linkedresource-from-linkedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="e0883-154">C#</span><span class="sxs-lookup"><span data-stu-id="e0883-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-linkedresource-from-linkedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0883-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0883-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-linkedresource-from-linkedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e0883-156">响应</span><span class="sxs-lookup"><span data-stu-id="e0883-156">Response</span></span>
<span data-ttu-id="e0883-157">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e0883-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.linkedResource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
  "webUrl": "http:://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```



