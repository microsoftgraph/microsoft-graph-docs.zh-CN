---
title: 更新 governanceRoleAssignmentRequests
description: 使管理员能够更新其决策 (`AdminApproved`或`AdminDenied`) 中的状态的 governanceRoleAssignmentRequests 上`PendingAdminDecision`。
ms.openlocfilehash: 0f52b810b861e18a679ae8aea4ffdf7fd2d67abd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048956"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="e8ffc-103">更新 governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="e8ffc-103">Update governanceRoleAssignmentRequests</span></span>

> <span data-ttu-id="e8ffc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e8ffc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8ffc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e8ffc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8ffc-106">使管理员能够更新其决策 (`AdminApproved`或`AdminDenied`) 上[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)中的状态的`PendingAdminDecision`。</span><span class="sxs-lookup"><span data-stu-id="e8ffc-106">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8ffc-107">权限</span><span class="sxs-lookup"><span data-stu-id="e8ffc-107">Permissions</span></span>
<span data-ttu-id="e8ffc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8ffc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8ffc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8ffc-110">Permission type</span></span>      | <span data-ttu-id="e8ffc-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="e8ffc-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8ffc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8ffc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e8ffc-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e8ffc-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="e8ffc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8ffc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8ffc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8ffc-115">Not supported.</span></span>    |
|<span data-ttu-id="e8ffc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8ffc-116">Application</span></span> | <span data-ttu-id="e8ffc-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e8ffc-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="e8ffc-118">除了权限范围，此 API 要求至少有一个请求程序`Active`管理员角色分配 (`owner`或`user access administrator`) 上的资源， [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)属于。</span><span class="sxs-lookup"><span data-stu-id="e8ffc-118">Besides the permission scope, this API requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource, which the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

## <a name="http-request"></a><span data-ttu-id="e8ffc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8ffc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

### <a name="request-headers"></a><span data-ttu-id="e8ffc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8ffc-120">Request headers</span></span>
| <span data-ttu-id="e8ffc-121">名称</span><span class="sxs-lookup"><span data-stu-id="e8ffc-121">Name</span></span>           | <span data-ttu-id="e8ffc-122">说明</span><span class="sxs-lookup"><span data-stu-id="e8ffc-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e8ffc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8ffc-123">Authorization</span></span>  | <span data-ttu-id="e8ffc-124">持有者 {code}</span><span class="sxs-lookup"><span data-stu-id="e8ffc-124">Bearer {code}</span></span>|
| <span data-ttu-id="e8ffc-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="e8ffc-125">Content-type</span></span>  | <span data-ttu-id="e8ffc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8ffc-126">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="e8ffc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8ffc-127">Request body</span></span>
|<span data-ttu-id="e8ffc-128">参数</span><span class="sxs-lookup"><span data-stu-id="e8ffc-128">Parameters</span></span>      |<span data-ttu-id="e8ffc-129">类型</span><span class="sxs-lookup"><span data-stu-id="e8ffc-129">Type</span></span>                   |<span data-ttu-id="e8ffc-130">必需</span><span class="sxs-lookup"><span data-stu-id="e8ffc-130">Required</span></span> |<span data-ttu-id="e8ffc-131">说明</span><span class="sxs-lookup"><span data-stu-id="e8ffc-131">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="e8ffc-132">原因</span><span class="sxs-lookup"><span data-stu-id="e8ffc-132">reason</span></span>        |<span data-ttu-id="e8ffc-133">字符串</span><span class="sxs-lookup"><span data-stu-id="e8ffc-133">String</span></span>                 |<span data-ttu-id="e8ffc-134">✓</span><span class="sxs-lookup"><span data-stu-id="e8ffc-134">✓</span></span>        |<span data-ttu-id="e8ffc-135">提供由管理员为其决策的原因。</span><span class="sxs-lookup"><span data-stu-id="e8ffc-135">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="e8ffc-136">决策</span><span class="sxs-lookup"><span data-stu-id="e8ffc-136">decision</span></span>        |<span data-ttu-id="e8ffc-137">字符串</span><span class="sxs-lookup"><span data-stu-id="e8ffc-137">String</span></span>                 |<span data-ttu-id="e8ffc-138">✓</span><span class="sxs-lookup"><span data-stu-id="e8ffc-138">✓</span></span>        |<span data-ttu-id="e8ffc-139">角色分配请求的管理员决策。</span><span class="sxs-lookup"><span data-stu-id="e8ffc-139">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="e8ffc-140">值应更新为`AdminApproved`或`AdminDenied`。</span><span class="sxs-lookup"><span data-stu-id="e8ffc-140">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="e8ffc-141">计划</span><span class="sxs-lookup"><span data-stu-id="e8ffc-141">schedule</span></span>      |[<span data-ttu-id="e8ffc-142">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e8ffc-142">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="e8ffc-143">角色分配请求的时间表。</span><span class="sxs-lookup"><span data-stu-id="e8ffc-143">The schedule of the role assignment request.</span></span> <span data-ttu-id="e8ffc-144">状态的`AdminApproved`，需要。</span><span class="sxs-lookup"><span data-stu-id="e8ffc-144">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="e8ffc-145">assignmentState</span><span class="sxs-lookup"><span data-stu-id="e8ffc-145">assignmentState</span></span>      |<span data-ttu-id="e8ffc-146">字符串</span><span class="sxs-lookup"><span data-stu-id="e8ffc-146">String</span></span>|         | <span data-ttu-id="e8ffc-147">状态的工作分配，以及的值可以是`Eligible`或`Active`。</span><span class="sxs-lookup"><span data-stu-id="e8ffc-147">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="e8ffc-148">为决策的`AdminApproved`，需要。</span><span class="sxs-lookup"><span data-stu-id="e8ffc-148">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="e8ffc-149">响应</span><span class="sxs-lookup"><span data-stu-id="e8ffc-149">Response</span></span>
<span data-ttu-id="e8ffc-150">此方法可以仅适用于请求的状态中的`PendingAdminDecision`。</span><span class="sxs-lookup"><span data-stu-id="e8ffc-150">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="e8ffc-p106">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e8ffc-p106">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="e8ffc-153">示例</span><span class="sxs-lookup"><span data-stu-id="e8ffc-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8ffc-154">请求</span><span class="sxs-lookup"><span data-stu-id="e8ffc-154">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
##### <a name="request-body"></a><span data-ttu-id="e8ffc-155">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8ffc-155">Request body</span></span>
```json
{
  "reason":"approve the request to extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-02-20T07:31:13.451Z",
    "stopDateTime":"2018-05-21T07:31:13.451Z",
    },
  "decision":"AdminApproved",
  "assignmentState": "Eligible"
}
```

##### <a name="response"></a><span data-ttu-id="e8ffc-156">响应</span><span class="sxs-lookup"><span data-stu-id="e8ffc-156">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UpdateRequest governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
