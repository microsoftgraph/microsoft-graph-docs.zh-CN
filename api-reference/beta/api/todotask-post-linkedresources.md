---
title: 创建 linkedResources
description: 创建新的 linkedResources 对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5180b5a38dafceb30871e574208d5321c8b0c38c
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849890"
---
# <a name="create-linkedresources"></a><span data-ttu-id="e597c-103">创建 linkedResources</span><span class="sxs-lookup"><span data-stu-id="e597c-103">Create linkedResources</span></span>
<span data-ttu-id="e597c-104">命名空间：microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="e597c-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="e597c-105">创建新的 linkedResources 对象。</span><span class="sxs-lookup"><span data-stu-id="e597c-105">Create a new linkedResources object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e597c-106">权限</span><span class="sxs-lookup"><span data-stu-id="e597c-106">Permissions</span></span>
<span data-ttu-id="e597c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e597c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e597c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e597c-109">Permission type</span></span>|<span data-ttu-id="e597c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e597c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e597c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e597c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e597c-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e597c-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="e597c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e597c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e597c-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e597c-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="e597c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e597c-115">Application</span></span>|<span data-ttu-id="e597c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e597c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e597c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e597c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a><span data-ttu-id="e597c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e597c-118">Request headers</span></span>
|<span data-ttu-id="e597c-119">名称</span><span class="sxs-lookup"><span data-stu-id="e597c-119">Name</span></span>|<span data-ttu-id="e597c-120">说明</span><span class="sxs-lookup"><span data-stu-id="e597c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e597c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e597c-121">Authorization</span></span>|<span data-ttu-id="e597c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e597c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e597c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e597c-124">Content-Type</span></span>|<span data-ttu-id="e597c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e597c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e597c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e597c-127">Request body</span></span>
<span data-ttu-id="e597c-128">在请求正文中，提供 [linkedResource](../resources/linkedresource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e597c-128">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="e597c-129">下表显示创建 [linkedResource 时所需的属性](../resources/linkedresource.md)。</span><span class="sxs-lookup"><span data-stu-id="e597c-129">The following table shows the properties that are required when you create the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="e597c-130">属性</span><span class="sxs-lookup"><span data-stu-id="e597c-130">Property</span></span>|<span data-ttu-id="e597c-131">类型</span><span class="sxs-lookup"><span data-stu-id="e597c-131">Type</span></span>|<span data-ttu-id="e597c-132">说明</span><span class="sxs-lookup"><span data-stu-id="e597c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e597c-133">id</span><span class="sxs-lookup"><span data-stu-id="e597c-133">id</span></span>|<span data-ttu-id="e597c-134">String</span><span class="sxs-lookup"><span data-stu-id="e597c-134">String</span></span>|<span data-ttu-id="e597c-135">继承自实体的链接实体生成的 [服务器 ID](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="e597c-135">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="e597c-136">webUrl</span><span class="sxs-lookup"><span data-stu-id="e597c-136">webUrl</span></span>|<span data-ttu-id="e597c-137">String</span><span class="sxs-lookup"><span data-stu-id="e597c-137">String</span></span>|<span data-ttu-id="e597c-138">到链接的实体的深度链接</span><span class="sxs-lookup"><span data-stu-id="e597c-138">Deeplink to the linked entity</span></span> |
|<span data-ttu-id="e597c-139">applicationName</span><span class="sxs-lookup"><span data-stu-id="e597c-139">applicationName</span></span>|<span data-ttu-id="e597c-140">String</span><span class="sxs-lookup"><span data-stu-id="e597c-140">String</span></span>|<span data-ttu-id="e597c-141">指示发送已链接实体的源的应用名称的字段</span><span class="sxs-lookup"><span data-stu-id="e597c-141">Field indicating app name of the source that is sending the linked entity</span></span> |
|<span data-ttu-id="e597c-142">displayName</span><span class="sxs-lookup"><span data-stu-id="e597c-142">displayName</span></span>|<span data-ttu-id="e597c-143">String</span><span class="sxs-lookup"><span data-stu-id="e597c-143">String</span></span>|<span data-ttu-id="e597c-144">指示所链接实体的标题的域。</span><span class="sxs-lookup"><span data-stu-id="e597c-144">Field indicating title of the linked entity.</span></span> |
|<span data-ttu-id="e597c-145">externalId</span><span class="sxs-lookup"><span data-stu-id="e597c-145">externalId</span></span>|<span data-ttu-id="e597c-146">String</span><span class="sxs-lookup"><span data-stu-id="e597c-146">String</span></span>|<span data-ttu-id="e597c-147">与第三方/合作伙伴系统上的此任务相关联的对象的 ID</span><span class="sxs-lookup"><span data-stu-id="e597c-147">Id of the object that is associated with this task on the third-party/partner system</span></span> |



## <a name="response"></a><span data-ttu-id="e597c-148">响应</span><span class="sxs-lookup"><span data-stu-id="e597c-148">Response</span></span>

<span data-ttu-id="e597c-149">如果成功，此方法在响应 `201 Created` 正文中返回 [响应代码和 linkedResource](../resources/linkedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e597c-149">If successful, this method returns a `201 Created` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e597c-150">示例</span><span class="sxs-lookup"><span data-stu-id="e597c-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e597c-151">请求</span><span class="sxs-lookup"><span data-stu-id="e597c-151">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="e597c-152">响应</span><span class="sxs-lookup"><span data-stu-id="e597c-152">Response</span></span>
<span data-ttu-id="e597c-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e597c-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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

