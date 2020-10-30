---
title: 创建 linkedResource
description: 创建新的 linkedResource 对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f915765192cf039c2095bac7e64a573d9b43b595
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797208"
---
# <a name="create-linkedresource"></a><span data-ttu-id="f2c3d-103">创建 linkedResource</span><span class="sxs-lookup"><span data-stu-id="f2c3d-103">Create linkedResource</span></span>
<span data-ttu-id="f2c3d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2c3d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f2c3d-105">创建一个 [linkedResource](../resources/linkedresource.md) 对象，以便将指定的 [任务](../resources/todotask.md) 与合作伙伴应用程序中的项目相关联。</span><span class="sxs-lookup"><span data-stu-id="f2c3d-105">Create a [linkedResource](../resources/linkedresource.md) object to associate a specified [task](../resources/todotask.md) with an item in a partner application.</span></span> <span data-ttu-id="f2c3d-106">例如，可以将任务与 Outlook 中促使任务的电子邮件项目相关联，也可以创建 **linkedResource** 对象来跟踪其关联情况。</span><span class="sxs-lookup"><span data-stu-id="f2c3d-106">For example, you can associate a task with an email item in Outlook that spurred the task, and you can create a **linkedResource** object to track its association.</span></span>

<span data-ttu-id="f2c3d-107">您还可以在 [创建任务](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples)时创建 **linkedResource** 对象。</span><span class="sxs-lookup"><span data-stu-id="f2c3d-107">You can also create a **linkedResource** object while [creating a task](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).</span></span>

## <a name="permissions"></a><span data-ttu-id="f2c3d-108">权限</span><span class="sxs-lookup"><span data-stu-id="f2c3d-108">Permissions</span></span>
<span data-ttu-id="f2c3d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2c3d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2c3d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2c3d-111">Permission type</span></span>|<span data-ttu-id="f2c3d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f2c3d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2c3d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2c3d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2c3d-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2c3d-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f2c3d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2c3d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2c3d-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2c3d-116">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f2c3d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2c3d-117">Application</span></span>|<span data-ttu-id="f2c3d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2c3d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2c3d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2c3d-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a><span data-ttu-id="f2c3d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2c3d-120">Request headers</span></span>
|<span data-ttu-id="f2c3d-121">名称</span><span class="sxs-lookup"><span data-stu-id="f2c3d-121">Name</span></span>|<span data-ttu-id="f2c3d-122">说明</span><span class="sxs-lookup"><span data-stu-id="f2c3d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f2c3d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2c3d-123">Authorization</span></span>|<span data-ttu-id="f2c3d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2c3d-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f2c3d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f2c3d-126">Content-Type</span></span>|<span data-ttu-id="f2c3d-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f2c3d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2c3d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2c3d-129">Request body</span></span>
<span data-ttu-id="f2c3d-130">在请求正文中，提供 [linkedResource](../resources/linkedresource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2c3d-130">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="f2c3d-131">下表显示创建 [linkedResource](../resources/linkedresource.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f2c3d-131">The following table shows the properties that are required when you create the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="f2c3d-132">属性</span><span class="sxs-lookup"><span data-stu-id="f2c3d-132">Property</span></span>|<span data-ttu-id="f2c3d-133">类型</span><span class="sxs-lookup"><span data-stu-id="f2c3d-133">Type</span></span>|<span data-ttu-id="f2c3d-134">说明</span><span class="sxs-lookup"><span data-stu-id="f2c3d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2c3d-135">id</span><span class="sxs-lookup"><span data-stu-id="f2c3d-135">id</span></span>|<span data-ttu-id="f2c3d-136">String</span><span class="sxs-lookup"><span data-stu-id="f2c3d-136">String</span></span>|<span data-ttu-id="f2c3d-137">从[实体](../resources/entity.md)继承的链接实体的服务器生成 Id</span><span class="sxs-lookup"><span data-stu-id="f2c3d-137">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="f2c3d-138">WebUrl</span><span class="sxs-lookup"><span data-stu-id="f2c3d-138">webUrl</span></span>|<span data-ttu-id="f2c3d-139">String</span><span class="sxs-lookup"><span data-stu-id="f2c3d-139">String</span></span>|<span data-ttu-id="f2c3d-140">Deeplink 到链接实体</span><span class="sxs-lookup"><span data-stu-id="f2c3d-140">Deeplink to the linked entity</span></span> |
|<span data-ttu-id="f2c3d-141">applicationName</span><span class="sxs-lookup"><span data-stu-id="f2c3d-141">applicationName</span></span>|<span data-ttu-id="f2c3d-142">String</span><span class="sxs-lookup"><span data-stu-id="f2c3d-142">String</span></span>|<span data-ttu-id="f2c3d-143">指示发送链接实体的源的应用程序名称的字段</span><span class="sxs-lookup"><span data-stu-id="f2c3d-143">Field indicating app name of the source that is sending the linked entity</span></span> |
|<span data-ttu-id="f2c3d-144">displayName</span><span class="sxs-lookup"><span data-stu-id="f2c3d-144">displayName</span></span>|<span data-ttu-id="f2c3d-145">String</span><span class="sxs-lookup"><span data-stu-id="f2c3d-145">String</span></span>|<span data-ttu-id="f2c3d-146">指示链接实体的标题的字段。</span><span class="sxs-lookup"><span data-stu-id="f2c3d-146">Field indicating title of the linked entity.</span></span> |
|<span data-ttu-id="f2c3d-147">externalId</span><span class="sxs-lookup"><span data-stu-id="f2c3d-147">externalId</span></span>|<span data-ttu-id="f2c3d-148">String</span><span class="sxs-lookup"><span data-stu-id="f2c3d-148">String</span></span>|<span data-ttu-id="f2c3d-149">与第三方/合作伙伴系统上的此任务相关联的对象的 Id</span><span class="sxs-lookup"><span data-stu-id="f2c3d-149">Id of the object that is associated with this task on the third-party/partner system</span></span> |



## <a name="response"></a><span data-ttu-id="f2c3d-150">响应</span><span class="sxs-lookup"><span data-stu-id="f2c3d-150">Response</span></span>

<span data-ttu-id="f2c3d-151">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [linkedResource](../resources/linkedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2c3d-151">If successful, this method returns a `201 Created` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2c3d-152">示例</span><span class="sxs-lookup"><span data-stu-id="f2c3d-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2c3d-153">请求</span><span class="sxs-lookup"><span data-stu-id="f2c3d-153">Request</span></span>

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


### <a name="response"></a><span data-ttu-id="f2c3d-154">响应</span><span class="sxs-lookup"><span data-stu-id="f2c3d-154">Response</span></span>
<span data-ttu-id="f2c3d-155">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f2c3d-155">**Note:** The response object shown here might be shortened for readability.</span></span>
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



