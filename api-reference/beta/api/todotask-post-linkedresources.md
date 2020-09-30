---
title: 创建 linkedResource
description: 创建新的 linkedResource 对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 56ad2b1f83475cc6b5af748c129f0cd84cdc07b0
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313686"
---
# <a name="create-linkedresource"></a><span data-ttu-id="fd494-103">创建 linkedResource</span><span class="sxs-lookup"><span data-stu-id="fd494-103">Create linkedResource</span></span>
<span data-ttu-id="fd494-104">命名空间： microsoft. graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="fd494-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="fd494-105">创建新的 **linkedResource** 对象。</span><span class="sxs-lookup"><span data-stu-id="fd494-105">Create a new **linkedResource** object.</span></span>

<span data-ttu-id="fd494-106">您还可以在[创建 todoTask](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples)时创建**linkedResource**对象。</span><span class="sxs-lookup"><span data-stu-id="fd494-106">You can also create a **linkedResource** object while [creating a todoTask](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).</span></span>

## <a name="permissions"></a><span data-ttu-id="fd494-107">权限</span><span class="sxs-lookup"><span data-stu-id="fd494-107">Permissions</span></span>
<span data-ttu-id="fd494-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fd494-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd494-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd494-110">Permission type</span></span>|<span data-ttu-id="fd494-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fd494-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd494-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd494-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd494-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd494-113">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="fd494-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd494-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd494-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd494-115">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="fd494-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd494-116">Application</span></span>|<span data-ttu-id="fd494-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd494-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd494-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd494-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a><span data-ttu-id="fd494-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd494-119">Request headers</span></span>
|<span data-ttu-id="fd494-120">名称</span><span class="sxs-lookup"><span data-stu-id="fd494-120">Name</span></span>|<span data-ttu-id="fd494-121">说明</span><span class="sxs-lookup"><span data-stu-id="fd494-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fd494-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd494-122">Authorization</span></span>|<span data-ttu-id="fd494-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fd494-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fd494-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd494-125">Content-Type</span></span>|<span data-ttu-id="fd494-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="fd494-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd494-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd494-128">Request body</span></span>
<span data-ttu-id="fd494-129">在请求正文中，提供 [linkedResource](../resources/linkedresource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd494-129">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="fd494-130">下表显示创建 [linkedResource](../resources/linkedresource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fd494-130">The following table shows the properties that are required when you create the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="fd494-131">属性</span><span class="sxs-lookup"><span data-stu-id="fd494-131">Property</span></span>|<span data-ttu-id="fd494-132">类型</span><span class="sxs-lookup"><span data-stu-id="fd494-132">Type</span></span>|<span data-ttu-id="fd494-133">说明</span><span class="sxs-lookup"><span data-stu-id="fd494-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd494-134">id</span><span class="sxs-lookup"><span data-stu-id="fd494-134">id</span></span>|<span data-ttu-id="fd494-135">字符串</span><span class="sxs-lookup"><span data-stu-id="fd494-135">String</span></span>|<span data-ttu-id="fd494-136">从[实体](../resources/entity.md)继承的链接实体的服务器生成 Id</span><span class="sxs-lookup"><span data-stu-id="fd494-136">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="fd494-137">webUrl</span><span class="sxs-lookup"><span data-stu-id="fd494-137">webUrl</span></span>|<span data-ttu-id="fd494-138">String</span><span class="sxs-lookup"><span data-stu-id="fd494-138">String</span></span>|<span data-ttu-id="fd494-139">Deeplink 到链接实体</span><span class="sxs-lookup"><span data-stu-id="fd494-139">Deeplink to the linked entity</span></span> |
|<span data-ttu-id="fd494-140">applicationName</span><span class="sxs-lookup"><span data-stu-id="fd494-140">applicationName</span></span>|<span data-ttu-id="fd494-141">String</span><span class="sxs-lookup"><span data-stu-id="fd494-141">String</span></span>|<span data-ttu-id="fd494-142">指示发送链接实体的源的应用程序名称的字段</span><span class="sxs-lookup"><span data-stu-id="fd494-142">Field indicating app name of the source that is sending the linked entity</span></span> |
|<span data-ttu-id="fd494-143">displayName</span><span class="sxs-lookup"><span data-stu-id="fd494-143">displayName</span></span>|<span data-ttu-id="fd494-144">字符串</span><span class="sxs-lookup"><span data-stu-id="fd494-144">String</span></span>|<span data-ttu-id="fd494-145">指示链接实体的标题的字段。</span><span class="sxs-lookup"><span data-stu-id="fd494-145">Field indicating title of the linked entity.</span></span> |
|<span data-ttu-id="fd494-146">externalId</span><span class="sxs-lookup"><span data-stu-id="fd494-146">externalId</span></span>|<span data-ttu-id="fd494-147">String</span><span class="sxs-lookup"><span data-stu-id="fd494-147">String</span></span>|<span data-ttu-id="fd494-148">与第三方/合作伙伴系统上的此任务相关联的对象的 Id</span><span class="sxs-lookup"><span data-stu-id="fd494-148">Id of the object that is associated with this task on the third-party/partner system</span></span> |



## <a name="response"></a><span data-ttu-id="fd494-149">响应</span><span class="sxs-lookup"><span data-stu-id="fd494-149">Response</span></span>

<span data-ttu-id="fd494-150">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [linkedResource](../resources/linkedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fd494-150">If successful, this method returns a `201 Created` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fd494-151">示例</span><span class="sxs-lookup"><span data-stu-id="fd494-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fd494-152">请求</span><span class="sxs-lookup"><span data-stu-id="fd494-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fd494-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd494-153">HTTP</span></span>](#tab/http)
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
  "webUrl": "https://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="fd494-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd494-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-linkedresource-from-linkedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="fd494-155">C#</span><span class="sxs-lookup"><span data-stu-id="fd494-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-linkedresource-from-linkedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd494-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd494-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-linkedresource-from-linkedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="fd494-157">响应</span><span class="sxs-lookup"><span data-stu-id="fd494-157">Response</span></span>
<span data-ttu-id="fd494-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fd494-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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



