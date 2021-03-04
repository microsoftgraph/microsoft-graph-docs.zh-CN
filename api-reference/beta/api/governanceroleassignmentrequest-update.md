---
title: 更新 governanceRoleAssignmentRequests
description: 使管理员能够更新其 (`AdminApproved` 或) `AdminDenied` 状态为 governanceRoleAssignmentRequests 的决策 `PendingAdminDecision` 。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 59080cf19cf96d82f029d3ba9513cd16a042157a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435852"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="4f46b-103">更新 governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="4f46b-103">Update governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="4f46b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f46b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f46b-105">使管理员能够更新其 (`AdminApproved` 或) `AdminDenied` 状态为 [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) 的决策 `PendingAdminDecision` 。</span><span class="sxs-lookup"><span data-stu-id="4f46b-105">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f46b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4f46b-106">Permissions</span></span>
<span data-ttu-id="4f46b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="4f46b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="4f46b-109">**注意：** 此 API 还要求请求者至少具有一个管理员角色分配 (或) `Active` `owner` `user access administrator` [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 所属的资源分配权限。</span><span class="sxs-lookup"><span data-stu-id="4f46b-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

### <a name="azure-resources"></a><span data-ttu-id="4f46b-110">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="4f46b-110">Azure resources</span></span>

| <span data-ttu-id="4f46b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f46b-111">Permission type</span></span> | <span data-ttu-id="4f46b-112">权限</span><span class="sxs-lookup"><span data-stu-id="4f46b-112">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="4f46b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f46b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4f46b-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="4f46b-114">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="4f46b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f46b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f46b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f46b-116">Not supported.</span></span> |
| <span data-ttu-id="4f46b-117">Application</span><span class="sxs-lookup"><span data-stu-id="4f46b-117">Application</span></span> | <span data-ttu-id="4f46b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f46b-118">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="4f46b-119">Azure AD</span><span class="sxs-lookup"><span data-stu-id="4f46b-119">Azure AD</span></span>

| <span data-ttu-id="4f46b-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f46b-120">Permission type</span></span> | <span data-ttu-id="4f46b-121">权限</span><span class="sxs-lookup"><span data-stu-id="4f46b-121">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="4f46b-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f46b-122">Delegated (work or school account)</span></span> | <span data-ttu-id="4f46b-123">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="4f46b-123">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="4f46b-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f46b-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f46b-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f46b-125">Not supported.</span></span> |
| <span data-ttu-id="4f46b-126">Application</span><span class="sxs-lookup"><span data-stu-id="4f46b-126">Application</span></span> | <span data-ttu-id="4f46b-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f46b-127">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="4f46b-128">组</span><span class="sxs-lookup"><span data-stu-id="4f46b-128">Groups</span></span>

|<span data-ttu-id="4f46b-129">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f46b-129">Permission type</span></span> | <span data-ttu-id="4f46b-130">权限</span><span class="sxs-lookup"><span data-stu-id="4f46b-130">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="4f46b-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f46b-131">Delegated (work or school account)</span></span> | <span data-ttu-id="4f46b-132">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="4f46b-132">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="4f46b-133">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f46b-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f46b-134">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f46b-134">Not supported.</span></span> |
| <span data-ttu-id="4f46b-135">Application</span><span class="sxs-lookup"><span data-stu-id="4f46b-135">Application</span></span> | <span data-ttu-id="4f46b-136">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f46b-136">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f46b-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f46b-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="4f46b-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f46b-138">Request headers</span></span>
| <span data-ttu-id="4f46b-139">名称</span><span class="sxs-lookup"><span data-stu-id="4f46b-139">Name</span></span>           | <span data-ttu-id="4f46b-140">说明</span><span class="sxs-lookup"><span data-stu-id="4f46b-140">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4f46b-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f46b-141">Authorization</span></span>  | <span data-ttu-id="4f46b-142">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4f46b-142">Bearer {code}</span></span>|
| <span data-ttu-id="4f46b-143">Content-type</span><span class="sxs-lookup"><span data-stu-id="4f46b-143">Content-type</span></span>  | <span data-ttu-id="4f46b-144">application/json</span><span class="sxs-lookup"><span data-stu-id="4f46b-144">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f46b-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f46b-145">Request body</span></span>

|<span data-ttu-id="4f46b-146">参数</span><span class="sxs-lookup"><span data-stu-id="4f46b-146">Parameters</span></span>      |<span data-ttu-id="4f46b-147">类型</span><span class="sxs-lookup"><span data-stu-id="4f46b-147">Type</span></span>                   |<span data-ttu-id="4f46b-148">必需</span><span class="sxs-lookup"><span data-stu-id="4f46b-148">Required</span></span> |<span data-ttu-id="4f46b-149">说明</span><span class="sxs-lookup"><span data-stu-id="4f46b-149">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="4f46b-150">reason</span><span class="sxs-lookup"><span data-stu-id="4f46b-150">reason</span></span>        |<span data-ttu-id="4f46b-151">String</span><span class="sxs-lookup"><span data-stu-id="4f46b-151">String</span></span>                 |<span data-ttu-id="4f46b-152">✓</span><span class="sxs-lookup"><span data-stu-id="4f46b-152">✓</span></span>        |<span data-ttu-id="4f46b-153">管理员提供其决策的原因。</span><span class="sxs-lookup"><span data-stu-id="4f46b-153">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="4f46b-154">决策</span><span class="sxs-lookup"><span data-stu-id="4f46b-154">decision</span></span>        |<span data-ttu-id="4f46b-155">String</span><span class="sxs-lookup"><span data-stu-id="4f46b-155">String</span></span>                 |<span data-ttu-id="4f46b-156">✓</span><span class="sxs-lookup"><span data-stu-id="4f46b-156">✓</span></span>        |<span data-ttu-id="4f46b-157">请求的管理员角色分配决定。</span><span class="sxs-lookup"><span data-stu-id="4f46b-157">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="4f46b-158">值应更新为 `AdminApproved` 或 `AdminDenied` 。</span><span class="sxs-lookup"><span data-stu-id="4f46b-158">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="4f46b-159">schedule</span><span class="sxs-lookup"><span data-stu-id="4f46b-159">schedule</span></span>      |[<span data-ttu-id="4f46b-160">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4f46b-160">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="4f46b-161">请求角色分配计划。</span><span class="sxs-lookup"><span data-stu-id="4f46b-161">The schedule of the role assignment request.</span></span> <span data-ttu-id="4f46b-162">对于状态 `AdminApproved` ，此为必需项。</span><span class="sxs-lookup"><span data-stu-id="4f46b-162">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="4f46b-163">assignmentState</span><span class="sxs-lookup"><span data-stu-id="4f46b-163">assignmentState</span></span>      |<span data-ttu-id="4f46b-164">String</span><span class="sxs-lookup"><span data-stu-id="4f46b-164">String</span></span>|         | <span data-ttu-id="4f46b-165">工作分配的状态，值可以是 `Eligible` 或 `Active` 。</span><span class="sxs-lookup"><span data-stu-id="4f46b-165">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="4f46b-166">要做出 `AdminApproved` 决策，必须执行。</span><span class="sxs-lookup"><span data-stu-id="4f46b-166">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="4f46b-167">响应</span><span class="sxs-lookup"><span data-stu-id="4f46b-167">Response</span></span>
<span data-ttu-id="4f46b-168">此方法只能应用于状态为 `PendingAdminDecision` .</span><span class="sxs-lookup"><span data-stu-id="4f46b-168">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="4f46b-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4f46b-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f46b-171">示例</span><span class="sxs-lookup"><span data-stu-id="4f46b-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f46b-172">请求</span><span class="sxs-lookup"><span data-stu-id="4f46b-172">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4f46b-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f46b-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="c"></a>[<span data-ttu-id="4f46b-174">C#</span><span class="sxs-lookup"><span data-stu-id="4f46b-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f46b-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f46b-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f46b-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f46b-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f46b-177">Java</span><span class="sxs-lookup"><span data-stu-id="4f46b-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updaterequest-governanceroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a><span data-ttu-id="4f46b-178">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f46b-178">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="4f46b-179">响应</span><span class="sxs-lookup"><span data-stu-id="4f46b-179">Response</span></span>
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


