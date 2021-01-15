---
title: 创建 linkedResource
description: 创建新的 linkedResource 对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8c99568099c99622373b91fff4a4b247e80f9288
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874401"
---
# <a name="create-linkedresource"></a><span data-ttu-id="adcf4-103">创建 linkedResource</span><span class="sxs-lookup"><span data-stu-id="adcf4-103">Create linkedResource</span></span>
<span data-ttu-id="adcf4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adcf4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="adcf4-105">创建 [linkedResource](../resources/linkedresource.md) 对象，将指定 [任务](../resources/todotask.md) 与合作伙伴应用程序中的项关联。</span><span class="sxs-lookup"><span data-stu-id="adcf4-105">Create a [linkedResource](../resources/linkedresource.md) object to associate a specified [task](../resources/todotask.md) with an item in a partner application.</span></span> <span data-ttu-id="adcf4-106">例如，可以将任务与 Outlook 中可跟踪该任务的电子邮件项目关联，也可以创建 **linkedResource** 对象来跟踪其关联。</span><span class="sxs-lookup"><span data-stu-id="adcf4-106">For example, you can associate a task with an email item in Outlook that spurred the task, and you can create a **linkedResource** object to track its association.</span></span>

<span data-ttu-id="adcf4-107">还可以在创建任务时创建 **linkedResource** [对象](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples)。</span><span class="sxs-lookup"><span data-stu-id="adcf4-107">You can also create a **linkedResource** object while [creating a task](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).</span></span>

## <a name="permissions"></a><span data-ttu-id="adcf4-108">权限</span><span class="sxs-lookup"><span data-stu-id="adcf4-108">Permissions</span></span>
<span data-ttu-id="adcf4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="adcf4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adcf4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="adcf4-111">Permission type</span></span>|<span data-ttu-id="adcf4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="adcf4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adcf4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="adcf4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="adcf4-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="adcf4-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="adcf4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="adcf4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adcf4-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="adcf4-116">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="adcf4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="adcf4-117">Application</span></span>|<span data-ttu-id="adcf4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="adcf4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="adcf4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="adcf4-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a><span data-ttu-id="adcf4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="adcf4-120">Request headers</span></span>
|<span data-ttu-id="adcf4-121">名称</span><span class="sxs-lookup"><span data-stu-id="adcf4-121">Name</span></span>|<span data-ttu-id="adcf4-122">说明</span><span class="sxs-lookup"><span data-stu-id="adcf4-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="adcf4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="adcf4-123">Authorization</span></span>|<span data-ttu-id="adcf4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="adcf4-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="adcf4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="adcf4-126">Content-Type</span></span>|<span data-ttu-id="adcf4-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="adcf4-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="adcf4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="adcf4-129">Request body</span></span>
<span data-ttu-id="adcf4-130">在请求正文中，提供 [linkedResource](../resources/linkedresource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="adcf4-130">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="adcf4-131">下表显示创建 [linkedResource](../resources/linkedresource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="adcf4-131">The following table shows the properties that are required when you create the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="adcf4-132">属性</span><span class="sxs-lookup"><span data-stu-id="adcf4-132">Property</span></span>|<span data-ttu-id="adcf4-133">类型</span><span class="sxs-lookup"><span data-stu-id="adcf4-133">Type</span></span>|<span data-ttu-id="adcf4-134">说明</span><span class="sxs-lookup"><span data-stu-id="adcf4-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adcf4-135">id</span><span class="sxs-lookup"><span data-stu-id="adcf4-135">id</span></span>|<span data-ttu-id="adcf4-136">String</span><span class="sxs-lookup"><span data-stu-id="adcf4-136">String</span></span>|<span data-ttu-id="adcf4-137">链接实体的服务器生成 ID 继承自 [实体](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="adcf4-137">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="adcf4-138">WebUrl</span><span class="sxs-lookup"><span data-stu-id="adcf4-138">webUrl</span></span>|<span data-ttu-id="adcf4-139">String</span><span class="sxs-lookup"><span data-stu-id="adcf4-139">String</span></span>|<span data-ttu-id="adcf4-140">指向链接实体的深层链接</span><span class="sxs-lookup"><span data-stu-id="adcf4-140">Deeplink to the linked entity</span></span> |
|<span data-ttu-id="adcf4-141">applicationName</span><span class="sxs-lookup"><span data-stu-id="adcf4-141">applicationName</span></span>|<span data-ttu-id="adcf4-142">String</span><span class="sxs-lookup"><span data-stu-id="adcf4-142">String</span></span>|<span data-ttu-id="adcf4-143">指示发送链接实体的源的应用名称的字段</span><span class="sxs-lookup"><span data-stu-id="adcf4-143">Field indicating app name of the source that is sending the linked entity</span></span> |
|<span data-ttu-id="adcf4-144">displayName</span><span class="sxs-lookup"><span data-stu-id="adcf4-144">displayName</span></span>|<span data-ttu-id="adcf4-145">String</span><span class="sxs-lookup"><span data-stu-id="adcf4-145">String</span></span>|<span data-ttu-id="adcf4-146">指示链接实体的标题的字段。</span><span class="sxs-lookup"><span data-stu-id="adcf4-146">Field indicating title of the linked entity.</span></span> |
|<span data-ttu-id="adcf4-147">externalId</span><span class="sxs-lookup"><span data-stu-id="adcf4-147">externalId</span></span>|<span data-ttu-id="adcf4-148">String</span><span class="sxs-lookup"><span data-stu-id="adcf4-148">String</span></span>|<span data-ttu-id="adcf4-149">第三方/合作伙伴系统上与此任务关联的对象的 ID</span><span class="sxs-lookup"><span data-stu-id="adcf4-149">Id of the object that is associated with this task on the third-party/partner system</span></span> |



## <a name="response"></a><span data-ttu-id="adcf4-150">响应</span><span class="sxs-lookup"><span data-stu-id="adcf4-150">Response</span></span>

<span data-ttu-id="adcf4-151">如果成功，此方法在响应 `201 Created` 正文中返回响应代码和 [linkedResource](../resources/linkedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="adcf4-151">If successful, this method returns a `201 Created` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="adcf4-152">示例</span><span class="sxs-lookup"><span data-stu-id="adcf4-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="adcf4-153">请求</span><span class="sxs-lookup"><span data-stu-id="adcf4-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="adcf4-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="adcf4-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "create_linkedresource_from_linkedresources"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
Content-Type: application/json
Content-length: 166

{
  "webUrl": "https://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```
# <a name="c"></a>[<span data-ttu-id="adcf4-155">C#</span><span class="sxs-lookup"><span data-stu-id="adcf4-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-linkedresource-from-linkedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adcf4-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adcf4-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-linkedresource-from-linkedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adcf4-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adcf4-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-linkedresource-from-linkedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="adcf4-158">Java</span><span class="sxs-lookup"><span data-stu-id="adcf4-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-linkedresource-from-linkedresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="adcf4-159">响应</span><span class="sxs-lookup"><span data-stu-id="adcf4-159">Response</span></span>
<span data-ttu-id="adcf4-160">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="adcf4-160">**Note:** The response object shown here might be shortened for readability.</span></span>
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



