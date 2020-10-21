---
title: 更新 governanceRoleAssignmentRequests
description: 使管理员能够更新 `AdminApproved` 状态为的 governanceRoleAssignmentRequests 上的决策 (或 `AdminDenied`) `PendingAdminDecision` 。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 95ff7dbf174a5dc6287be0fc7476c21596e651ba
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634860"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="46d4c-103">更新 governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="46d4c-103">Update governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="46d4c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46d4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46d4c-105">使管理员能够更新 `AdminApproved` `AdminDenied` 状态为的 [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) 上的决策 (或) `PendingAdminDecision` 。</span><span class="sxs-lookup"><span data-stu-id="46d4c-105">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="46d4c-106">权限</span><span class="sxs-lookup"><span data-stu-id="46d4c-106">Permissions</span></span>
<span data-ttu-id="46d4c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="46d4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="46d4c-109">**注意：** 此 API 还要求请求者在 `Active` `owner` `user access administrator` [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 所属的资源上至少有一个管理员角色分配 (或) 。</span><span class="sxs-lookup"><span data-stu-id="46d4c-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

### <a name="azure-resources"></a><span data-ttu-id="46d4c-110">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="46d4c-110">Azure resources</span></span>

| <span data-ttu-id="46d4c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="46d4c-111">Permission type</span></span> | <span data-ttu-id="46d4c-112">权限</span><span class="sxs-lookup"><span data-stu-id="46d4c-112">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="46d4c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46d4c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="46d4c-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="46d4c-114">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="46d4c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46d4c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46d4c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="46d4c-116">Not supported.</span></span> |
| <span data-ttu-id="46d4c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="46d4c-117">Application</span></span> | <span data-ttu-id="46d4c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="46d4c-118">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="46d4c-119">Azure AD</span><span class="sxs-lookup"><span data-stu-id="46d4c-119">Azure AD</span></span>

| <span data-ttu-id="46d4c-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="46d4c-120">Permission type</span></span> | <span data-ttu-id="46d4c-121">权限</span><span class="sxs-lookup"><span data-stu-id="46d4c-121">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="46d4c-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46d4c-122">Delegated (work or school account)</span></span> | <span data-ttu-id="46d4c-123">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="46d4c-123">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="46d4c-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46d4c-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46d4c-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="46d4c-125">Not supported.</span></span> |
| <span data-ttu-id="46d4c-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="46d4c-126">Application</span></span> | <span data-ttu-id="46d4c-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="46d4c-127">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="46d4c-128">组</span><span class="sxs-lookup"><span data-stu-id="46d4c-128">Groups</span></span>

|<span data-ttu-id="46d4c-129">权限类型</span><span class="sxs-lookup"><span data-stu-id="46d4c-129">Permission type</span></span> | <span data-ttu-id="46d4c-130">权限</span><span class="sxs-lookup"><span data-stu-id="46d4c-130">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="46d4c-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46d4c-131">Delegated (work or school account)</span></span> | <span data-ttu-id="46d4c-132">PrivilegedAccess AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="46d4c-132">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="46d4c-133">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46d4c-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46d4c-134">不支持。</span><span class="sxs-lookup"><span data-stu-id="46d4c-134">Not supported.</span></span> |
| <span data-ttu-id="46d4c-135">应用程序</span><span class="sxs-lookup"><span data-stu-id="46d4c-135">Application</span></span> | <span data-ttu-id="46d4c-136">不支持。</span><span class="sxs-lookup"><span data-stu-id="46d4c-136">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46d4c-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46d4c-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="46d4c-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="46d4c-138">Request headers</span></span>
| <span data-ttu-id="46d4c-139">名称</span><span class="sxs-lookup"><span data-stu-id="46d4c-139">Name</span></span>           | <span data-ttu-id="46d4c-140">说明</span><span class="sxs-lookup"><span data-stu-id="46d4c-140">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="46d4c-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="46d4c-141">Authorization</span></span>  | <span data-ttu-id="46d4c-142">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="46d4c-142">Bearer {code}</span></span>|
| <span data-ttu-id="46d4c-143">Content-type</span><span class="sxs-lookup"><span data-stu-id="46d4c-143">Content-type</span></span>  | <span data-ttu-id="46d4c-144">application/json</span><span class="sxs-lookup"><span data-stu-id="46d4c-144">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46d4c-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="46d4c-145">Request body</span></span>

|<span data-ttu-id="46d4c-146">参数</span><span class="sxs-lookup"><span data-stu-id="46d4c-146">Parameters</span></span>      |<span data-ttu-id="46d4c-147">类型</span><span class="sxs-lookup"><span data-stu-id="46d4c-147">Type</span></span>                   |<span data-ttu-id="46d4c-148">必需</span><span class="sxs-lookup"><span data-stu-id="46d4c-148">Required</span></span> |<span data-ttu-id="46d4c-149">说明</span><span class="sxs-lookup"><span data-stu-id="46d4c-149">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="46d4c-150">reason</span><span class="sxs-lookup"><span data-stu-id="46d4c-150">reason</span></span>        |<span data-ttu-id="46d4c-151">String</span><span class="sxs-lookup"><span data-stu-id="46d4c-151">String</span></span>                 |<span data-ttu-id="46d4c-152">✓</span><span class="sxs-lookup"><span data-stu-id="46d4c-152">✓</span></span>        |<span data-ttu-id="46d4c-153">管理员为自己的决定提供的原因。</span><span class="sxs-lookup"><span data-stu-id="46d4c-153">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="46d4c-154">权</span><span class="sxs-lookup"><span data-stu-id="46d4c-154">decision</span></span>        |<span data-ttu-id="46d4c-155">String</span><span class="sxs-lookup"><span data-stu-id="46d4c-155">String</span></span>                 |<span data-ttu-id="46d4c-156">✓</span><span class="sxs-lookup"><span data-stu-id="46d4c-156">✓</span></span>        |<span data-ttu-id="46d4c-157">角色分配请求的管理员决定。</span><span class="sxs-lookup"><span data-stu-id="46d4c-157">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="46d4c-158">应将值更新为 `AdminApproved` 或 `AdminDenied` 。</span><span class="sxs-lookup"><span data-stu-id="46d4c-158">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="46d4c-159">schedule</span><span class="sxs-lookup"><span data-stu-id="46d4c-159">schedule</span></span>      |[<span data-ttu-id="46d4c-160">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="46d4c-160">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="46d4c-161">角色分配请求的日程安排。</span><span class="sxs-lookup"><span data-stu-id="46d4c-161">The schedule of the role assignment request.</span></span> <span data-ttu-id="46d4c-162">对于的状态 `AdminApproved` ，是必需的。</span><span class="sxs-lookup"><span data-stu-id="46d4c-162">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="46d4c-163">assignmentState</span><span class="sxs-lookup"><span data-stu-id="46d4c-163">assignmentState</span></span>      |<span data-ttu-id="46d4c-164">String</span><span class="sxs-lookup"><span data-stu-id="46d4c-164">String</span></span>|         | <span data-ttu-id="46d4c-165">工作分配的状态，值可以是 `Eligible` 或 `Active` 。</span><span class="sxs-lookup"><span data-stu-id="46d4c-165">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="46d4c-166">有关的决策 `AdminApproved` ，则是必需的。</span><span class="sxs-lookup"><span data-stu-id="46d4c-166">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="46d4c-167">响应</span><span class="sxs-lookup"><span data-stu-id="46d4c-167">Response</span></span>
<span data-ttu-id="46d4c-168">此方法仅适用于状态为的请求 `PendingAdminDecision` 。</span><span class="sxs-lookup"><span data-stu-id="46d4c-168">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="46d4c-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="46d4c-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46d4c-171">示例</span><span class="sxs-lookup"><span data-stu-id="46d4c-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46d4c-172">请求</span><span class="sxs-lookup"><span data-stu-id="46d4c-172">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="46d4c-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="46d4c-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="c"></a>[<span data-ttu-id="46d4c-174">C#</span><span class="sxs-lookup"><span data-stu-id="46d4c-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46d4c-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46d4c-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46d4c-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46d4c-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a><span data-ttu-id="46d4c-177">请求正文</span><span class="sxs-lookup"><span data-stu-id="46d4c-177">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="46d4c-178">响应</span><span class="sxs-lookup"><span data-stu-id="46d4c-178">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "UpdateRequest governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


