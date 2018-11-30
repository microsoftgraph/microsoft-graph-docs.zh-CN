---
title: 创建 governanceRoleAssignmentRequest
description: 创建角色分配请求以表示该操作所需角色分配。 下表列出的操作。
ms.openlocfilehash: b0d9edab1182d4a6fa620cfb953df1cb8af20c66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044348"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="cc11f-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="cc11f-104">Create governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="cc11f-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cc11f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc11f-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cc11f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cc11f-107">创建角色分配请求以表示该操作所需角色分配。</span><span class="sxs-lookup"><span data-stu-id="cc11f-107">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="cc11f-108">下表列出的操作。</span><span class="sxs-lookup"><span data-stu-id="cc11f-108">The following table lists the operations.</span></span>

| <span data-ttu-id="cc11f-109">操作</span><span class="sxs-lookup"><span data-stu-id="cc11f-109">Operation</span></span>       | <span data-ttu-id="cc11f-110">类型</span><span class="sxs-lookup"><span data-stu-id="cc11f-110">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="cc11f-111">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="cc11f-111">Assign a role assignment</span></span>| <span data-ttu-id="cc11f-112">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="cc11f-112">AdminAdd</span></span> |
| <span data-ttu-id="cc11f-113">激活合格的角色分配</span><span class="sxs-lookup"><span data-stu-id="cc11f-113">Activate an eligible role assignment</span></span>| <span data-ttu-id="cc11f-114">UserAdd</span><span class="sxs-lookup"><span data-stu-id="cc11f-114">UserAdd</span></span> | 
| <span data-ttu-id="cc11f-115">停用已激活的角色分配</span><span class="sxs-lookup"><span data-stu-id="cc11f-115">Deactivate an activated role assignment</span></span>| <span data-ttu-id="cc11f-116">UserRemove</span><span class="sxs-lookup"><span data-stu-id="cc11f-116">UserRemove</span></span> | 
| <span data-ttu-id="cc11f-117">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="cc11f-117">Remove a role assignment</span></span>| <span data-ttu-id="cc11f-118">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="cc11f-118">AdminRemove</span></span> |
| <span data-ttu-id="cc11f-119">更新一个角色分配</span><span class="sxs-lookup"><span data-stu-id="cc11f-119">Update a role assignment</span></span>| <span data-ttu-id="cc11f-120">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="cc11f-120">AdminUpdate</span></span> |
| <span data-ttu-id="cc11f-121">请求扩展我角色分配</span><span class="sxs-lookup"><span data-stu-id="cc11f-121">Request to extend my role assignment</span></span>| <span data-ttu-id="cc11f-122">UserExtend</span><span class="sxs-lookup"><span data-stu-id="cc11f-122">UserExtend</span></span> | 
| <span data-ttu-id="cc11f-123">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="cc11f-123">Extend a role assignment</span></span>| <span data-ttu-id="cc11f-124">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="cc11f-124">AdminExtend</span></span> | 
| <span data-ttu-id="cc11f-125">请求续订我过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="cc11f-125">Request to renew my expired role assignment</span></span>| <span data-ttu-id="cc11f-126">UserRenew</span><span class="sxs-lookup"><span data-stu-id="cc11f-126">UserRenew</span></span> | 
| <span data-ttu-id="cc11f-127">续订已过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="cc11f-127">Renew an expired role assignment</span></span>| <span data-ttu-id="cc11f-128">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="cc11f-128">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="cc11f-129">权限</span><span class="sxs-lookup"><span data-stu-id="cc11f-129">Permissions</span></span>
<span data-ttu-id="cc11f-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc11f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc11f-132">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc11f-132">Permission type</span></span>      | <span data-ttu-id="cc11f-133">Permissions</span><span class="sxs-lookup"><span data-stu-id="cc11f-133">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc11f-134">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc11f-134">Delegated (work or school account)</span></span> | <span data-ttu-id="cc11f-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="cc11f-135">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="cc11f-136">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc11f-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc11f-137">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc11f-137">Not supported.</span></span>    |
|<span data-ttu-id="cc11f-138">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc11f-138">Application</span></span> | <span data-ttu-id="cc11f-139">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="cc11f-139">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc11f-140">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc11f-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc11f-141">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cc11f-141">Optional query parameters</span></span>
<span data-ttu-id="cc11f-142">此方法执行**不**支持[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="cc11f-142">This method does **not** support [OData query parameters](/graph/query-parameters).</span></span>

### <a name="request-headers"></a><span data-ttu-id="cc11f-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc11f-143">Request headers</span></span>
| <span data-ttu-id="cc11f-144">名称</span><span class="sxs-lookup"><span data-stu-id="cc11f-144">Name</span></span>       | <span data-ttu-id="cc11f-145">说明</span><span class="sxs-lookup"><span data-stu-id="cc11f-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cc11f-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc11f-146">Authorization</span></span>  | <span data-ttu-id="cc11f-147">持有者 {code}</span><span class="sxs-lookup"><span data-stu-id="cc11f-147">Bearer {code}</span></span>|
| <span data-ttu-id="cc11f-148">Content-type</span><span class="sxs-lookup"><span data-stu-id="cc11f-148">Content-type</span></span>  | <span data-ttu-id="cc11f-149">application/json</span><span class="sxs-lookup"><span data-stu-id="cc11f-149">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="cc11f-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc11f-150">Request body</span></span>
<span data-ttu-id="cc11f-151">在请求正文中，提供[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc11f-151">In the request body, supply a JSON representation of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="cc11f-152">属性</span><span class="sxs-lookup"><span data-stu-id="cc11f-152">Property</span></span>     | <span data-ttu-id="cc11f-153">类型</span><span class="sxs-lookup"><span data-stu-id="cc11f-153">Type</span></span>    |<span data-ttu-id="cc11f-154">必需</span><span class="sxs-lookup"><span data-stu-id="cc11f-154">Required</span></span>|  <span data-ttu-id="cc11f-155">说明</span><span class="sxs-lookup"><span data-stu-id="cc11f-155">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="cc11f-156">resourceId</span><span class="sxs-lookup"><span data-stu-id="cc11f-156">resourceId</span></span>|<span data-ttu-id="cc11f-157">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-157">String</span></span>|<span data-ttu-id="cc11f-158">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-158">Yes</span></span>|<span data-ttu-id="cc11f-159">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="cc11f-159">The ID of the resource.</span></span>|
|<span data-ttu-id="cc11f-160">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="cc11f-160">roleDefinitionId</span></span>|<span data-ttu-id="cc11f-161">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-161">String</span></span>|<span data-ttu-id="cc11f-162">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-162">Yes</span></span>|<span data-ttu-id="cc11f-163">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="cc11f-163">The ID of the role definition.</span></span>|
|<span data-ttu-id="cc11f-164">subjectId</span><span class="sxs-lookup"><span data-stu-id="cc11f-164">subjectId</span></span>|<span data-ttu-id="cc11f-165">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-165">String</span></span>|<span data-ttu-id="cc11f-166">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-166">Yes</span></span>|<span data-ttu-id="cc11f-167">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="cc11f-167">The ID of the subject.</span></span>|
|<span data-ttu-id="cc11f-168">assignmentState</span><span class="sxs-lookup"><span data-stu-id="cc11f-168">assignmentState</span></span>|<span data-ttu-id="cc11f-169">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-169">String</span></span>|<span data-ttu-id="cc11f-170">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-170">Yes</span></span>|<span data-ttu-id="cc11f-171">工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="cc11f-171">The state of assignment.</span></span> <span data-ttu-id="cc11f-172">值可以是``Eligible``和``Active``。</span><span class="sxs-lookup"><span data-stu-id="cc11f-172">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="cc11f-173">type</span><span class="sxs-lookup"><span data-stu-id="cc11f-173">type</span></span>|<span data-ttu-id="cc11f-174">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-174">String</span></span>|<span data-ttu-id="cc11f-175">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-175">Yes</span></span>|<span data-ttu-id="cc11f-176">请求类型。</span><span class="sxs-lookup"><span data-stu-id="cc11f-176">The request type.</span></span> <span data-ttu-id="cc11f-177">值可以是`AdminAdd`， `UserAdd`， `AdminUpdate`， `AdminRemove`， `UserRemove`， `UserExtend`， `UserRenew`，`AdminRenew`和`AdminExtend`。</span><span class="sxs-lookup"><span data-stu-id="cc11f-177">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="cc11f-178">原因</span><span class="sxs-lookup"><span data-stu-id="cc11f-178">reason</span></span>|<span data-ttu-id="cc11f-179">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-179">String</span></span>| |<span data-ttu-id="cc11f-180">原因需要提供角色分配请求的审核和查看用途。</span><span class="sxs-lookup"><span data-stu-id="cc11f-180">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="cc11f-181">计划</span><span class="sxs-lookup"><span data-stu-id="cc11f-181">schedule</span></span>|[<span data-ttu-id="cc11f-182">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="cc11f-182">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="cc11f-183">角色分配请求的时间表。</span><span class="sxs-lookup"><span data-stu-id="cc11f-183">The schedule of the role assignment request.</span></span> <span data-ttu-id="cc11f-184">请求类型的`UserAdd`， `AdminAdd`， `AdminUpdate`，和`AdminExtend`，需要。</span><span class="sxs-lookup"><span data-stu-id="cc11f-184">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

### <a name="response"></a><span data-ttu-id="cc11f-185">响应</span><span class="sxs-lookup"><span data-stu-id="cc11f-185">Response</span></span>
<span data-ttu-id="cc11f-186">如果成功，此方法返回`201, Created`响应代码和响应正文中的[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cc11f-186">If successful, this method returns a `201, Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="error-codes"></a><span data-ttu-id="cc11f-187">错误代码</span><span class="sxs-lookup"><span data-stu-id="cc11f-187">Error codes</span></span>
<span data-ttu-id="cc11f-188">此 API 遵循标准的 HTTP 代码，除了下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="cc11f-188">This API follows the standard of HTTP codes, in addition to the error codes listed in the following table.</span></span>

|<span data-ttu-id="cc11f-189">错误代码</span><span class="sxs-lookup"><span data-stu-id="cc11f-189">Error code</span></span>     | <span data-ttu-id="cc11f-190">错误消息</span><span class="sxs-lookup"><span data-stu-id="cc11f-190">Error message</span></span>              | <span data-ttu-id="cc11f-191">详细信息</span><span class="sxs-lookup"><span data-stu-id="cc11f-191">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="cc11f-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="cc11f-192">400 BadRequest</span></span> | <span data-ttu-id="cc11f-193">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="cc11f-193">RoleNotFound</span></span>    | <span data-ttu-id="cc11f-194">`roleDefinitionId`提供在请求正文找不到。</span><span class="sxs-lookup"><span data-stu-id="cc11f-194">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="cc11f-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="cc11f-195">400 BadRequest</span></span> | <span data-ttu-id="cc11f-196">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="cc11f-196">ResourceIsLocked</span></span>    | <span data-ttu-id="cc11f-197">在请求正文中提供的资源处于状态的`Locked`和无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="cc11f-197">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="cc11f-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="cc11f-198">400 BadRequest</span></span> | <span data-ttu-id="cc11f-199">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="cc11f-199">SubjectNotFound</span></span>    | <span data-ttu-id="cc11f-200">`subjectId`提供在请求正文找不到。</span><span class="sxs-lookup"><span data-stu-id="cc11f-200">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="cc11f-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="cc11f-201">400 BadRequest</span></span> | <span data-ttu-id="cc11f-202">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="cc11f-202">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="cc11f-203">已存在挂起[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)系统中。</span><span class="sxs-lookup"><span data-stu-id="cc11f-203">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="cc11f-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="cc11f-204">400 BadRequest</span></span> | <span data-ttu-id="cc11f-205">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="cc11f-205">RoleAssignmentExists</span></span>    | <span data-ttu-id="cc11f-206">系统中存在[governanceRoleAssignment](../resources/governanceroleassignment.md)请求已创建。</span><span class="sxs-lookup"><span data-stu-id="cc11f-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="cc11f-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="cc11f-207">400 BadRequest</span></span> | <span data-ttu-id="cc11f-208">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="cc11f-208">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="cc11f-209">系统中不存在[governanceRoleAssignment](../resources/governanceroleassignment.md)请求来更新/扩展。</span><span class="sxs-lookup"><span data-stu-id="cc11f-209">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="cc11f-210">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="cc11f-210">400 BadRequest</span></span> | <span data-ttu-id="cc11f-211">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="cc11f-211">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="cc11f-212">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部的策略，且无法创建。</span><span class="sxs-lookup"><span data-stu-id="cc11f-212">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="example-1"></a><span data-ttu-id="cc11f-213">示例 1</span><span class="sxs-lookup"><span data-stu-id="cc11f-213">Example 1</span></span>
<span data-ttu-id="cc11f-214">本示例中，管理员为帐单读者角色分配用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="cc11f-214">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="cc11f-215">**注意：** 除了权限，此示例要求至少有一个请求程序`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="cc11f-215">**Note:** Besides the permission, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="cc11f-216">属性</span><span class="sxs-lookup"><span data-stu-id="cc11f-216">Property</span></span>     | <span data-ttu-id="cc11f-217">类型</span><span class="sxs-lookup"><span data-stu-id="cc11f-217">Type</span></span>    |<span data-ttu-id="cc11f-218">是否必需</span><span class="sxs-lookup"><span data-stu-id="cc11f-218">Required</span></span>|  <span data-ttu-id="cc11f-219">值</span><span class="sxs-lookup"><span data-stu-id="cc11f-219">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="cc11f-220">resourceId</span><span class="sxs-lookup"><span data-stu-id="cc11f-220">resourceId</span></span>|<span data-ttu-id="cc11f-221">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-221">String</span></span>|<span data-ttu-id="cc11f-222">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-222">Yes</span></span>|<span data-ttu-id="cc11f-223">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="cc11f-223">\<resourceId\></span></span>|
|<span data-ttu-id="cc11f-224">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="cc11f-224">roleDefinitionId</span></span>|<span data-ttu-id="cc11f-225">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-225">String</span></span>|<span data-ttu-id="cc11f-226">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-226">Yes</span></span>|<span data-ttu-id="cc11f-227">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="cc11f-227">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="cc11f-228">subjectId</span><span class="sxs-lookup"><span data-stu-id="cc11f-228">subjectId</span></span>|<span data-ttu-id="cc11f-229">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-229">String</span></span>|<span data-ttu-id="cc11f-230">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-230">Yes</span></span>|<span data-ttu-id="cc11f-231">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="cc11f-231">\<subjectId\></span></span>|
|<span data-ttu-id="cc11f-232">assignmentState</span><span class="sxs-lookup"><span data-stu-id="cc11f-232">assignmentState</span></span>|<span data-ttu-id="cc11f-233">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-233">String</span></span>|<span data-ttu-id="cc11f-234">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-234">Yes</span></span>| <span data-ttu-id="cc11f-235">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="cc11f-235">Eligible / Active</span></span>|
|<span data-ttu-id="cc11f-236">type</span><span class="sxs-lookup"><span data-stu-id="cc11f-236">type</span></span>|<span data-ttu-id="cc11f-237">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-237">String</span></span>|<span data-ttu-id="cc11f-238">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-238">Yes</span></span>| <span data-ttu-id="cc11f-239">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="cc11f-239">AdminAdd</span></span>|
|<span data-ttu-id="cc11f-240">原因</span><span class="sxs-lookup"><span data-stu-id="cc11f-240">reason</span></span>|<span data-ttu-id="cc11f-241">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-241">String</span></span>| <span data-ttu-id="cc11f-242">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="cc11f-242">depends on role Settings</span></span>||
|<span data-ttu-id="cc11f-243">计划</span><span class="sxs-lookup"><span data-stu-id="cc11f-243">schedule</span></span>|[<span data-ttu-id="cc11f-244">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="cc11f-244">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="cc11f-245">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-245">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="cc11f-246">请求</span><span class="sxs-lookup"><span data-stu-id="cc11f-246">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
"resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Eligible",
"type":"AdminAdd",
"reason":"Assign an eligible role",
"schedule":{
  "startDateTime":"2018-05-12T23:37:43.356Z",
  "endDateTime":"2018-11-08T23:37:43.356Z",
  "type":"Once"
  }
}
```
##### <a name="response"></a><span data-ttu-id="cc11f-247">响应</span><span class="sxs-lookup"><span data-stu-id="cc11f-247">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "1232e4ea-741a-4be5-8044-5edabdd61672",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "",
    "type": "AdminAdd",
    "assignmentState": "Eligible",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "roleAssignmentStartDateTime": "2018-05-12T23:38:34.6007266Z",
    "roleAssignmentEndDateTime": "2018-11-08T23:37:43.356Z",
    "reason": "Evaluate Only",
    "status": {
        "status": "InProgress",
        "subStatus": "Granted",
        "statusDetails": [
            {
                "key": "AdminRequestRule",
                "value": "Grant"
            },
            {
                "key": "ExpirationRule",
                "value": "Grant"
            },
            {
                "key": "MfaRule",
                "value": "Grant"
            }
        ]
    },
    "schedule": {
        "type": "Once",
        "startDateTime": "2018-05-12T23:37:43.356Z",
        "endDateTime": "2018-11-08T23:37:43.356Z",
        "duration": "PT0S"
    }
}
```

## <a name="example-2"></a><span data-ttu-id="cc11f-248">示例 2</span><span class="sxs-lookup"><span data-stu-id="cc11f-248">Example 2</span></span>
<span data-ttu-id="cc11f-249">本示例中，用户 nawu@fimdev.net 激活合格的帐单读取器角色。</span><span class="sxs-lookup"><span data-stu-id="cc11f-249">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="cc11f-250">属性</span><span class="sxs-lookup"><span data-stu-id="cc11f-250">Property</span></span>     | <span data-ttu-id="cc11f-251">类型</span><span class="sxs-lookup"><span data-stu-id="cc11f-251">Type</span></span>    |<span data-ttu-id="cc11f-252">是否必需</span><span class="sxs-lookup"><span data-stu-id="cc11f-252">Required</span></span>|  <span data-ttu-id="cc11f-253">值</span><span class="sxs-lookup"><span data-stu-id="cc11f-253">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="cc11f-254">resourceId</span><span class="sxs-lookup"><span data-stu-id="cc11f-254">resourceId</span></span>|<span data-ttu-id="cc11f-255">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-255">String</span></span>|<span data-ttu-id="cc11f-256">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-256">Yes</span></span>|<span data-ttu-id="cc11f-257">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="cc11f-257">\<resourceId\></span></span>|
|<span data-ttu-id="cc11f-258">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="cc11f-258">roleDefinitionId</span></span>|<span data-ttu-id="cc11f-259">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-259">String</span></span>|<span data-ttu-id="cc11f-260">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-260">Yes</span></span>|<span data-ttu-id="cc11f-261">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="cc11f-261">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="cc11f-262">subjectId</span><span class="sxs-lookup"><span data-stu-id="cc11f-262">subjectId</span></span>|<span data-ttu-id="cc11f-263">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-263">String</span></span>|<span data-ttu-id="cc11f-264">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-264">Yes</span></span>|<span data-ttu-id="cc11f-265">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="cc11f-265">\<subjectId\></span></span>|
|<span data-ttu-id="cc11f-266">assignmentState</span><span class="sxs-lookup"><span data-stu-id="cc11f-266">assignmentState</span></span>|<span data-ttu-id="cc11f-267">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-267">String</span></span>|<span data-ttu-id="cc11f-268">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-268">Yes</span></span>| <span data-ttu-id="cc11f-269">活跃</span><span class="sxs-lookup"><span data-stu-id="cc11f-269">Active</span></span>|
|<span data-ttu-id="cc11f-270">type</span><span class="sxs-lookup"><span data-stu-id="cc11f-270">type</span></span>|<span data-ttu-id="cc11f-271">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-271">String</span></span>|<span data-ttu-id="cc11f-272">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-272">Yes</span></span>| <span data-ttu-id="cc11f-273">UserAdd</span><span class="sxs-lookup"><span data-stu-id="cc11f-273">UserAdd</span></span>|
|<span data-ttu-id="cc11f-274">原因</span><span class="sxs-lookup"><span data-stu-id="cc11f-274">reason</span></span>|<span data-ttu-id="cc11f-275">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-275">String</span></span>| <span data-ttu-id="cc11f-276">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="cc11f-276">depends on role Settings</span></span>||
|<span data-ttu-id="cc11f-277">计划</span><span class="sxs-lookup"><span data-stu-id="cc11f-277">schedule</span></span>|[<span data-ttu-id="cc11f-278">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="cc11f-278">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="cc11f-279">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-279">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="cc11f-280">请求</span><span class="sxs-lookup"><span data-stu-id="cc11f-280">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"8b4d1d51-08e9-4254-b0a6-b16177aae376",
"resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Active",
"type":"UserAdd",
"reason": "Activate the owner role",
"schedule":{
  "type":"Once",
  "startDateTime":"2018-05-12T23:28:43.537Z",
  "duration":"PT9H"
  },
"linkedEligibleRoleAssignmentId":"e327f4be-42a0-47a2-8579-0a39b025b394"
}
```
##### <a name="response"></a><span data-ttu-id="cc11f-281">响应</span><span class="sxs-lookup"><span data-stu-id="cc11f-281">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "3ad49a7c-918e-4d86-9f84-fab28f8658c0",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394",
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "roleAssignmentStartDateTime": "2018-05-12T23:29:29.5123911Z",
    "roleAssignmentEndDateTime": "2018-05-13T08:28:43.537Z",
    "reason": "Activate the owner role",
    "status": {
        "status": "InProgress",
        "subStatus": "Granted",
        "statusDetails": [
            {
                "key": "EligibilityRule",
                "value": "Grant"
            },
            {
                "key": "ExpirationRule",
                "value": "Grant"
            },
            {
                "key": "MfaRule",
                "value": "Grant"
            },
            {
                "key": "JustificationRule",
                "value": "Grant"
            },
            {
                "key": "ActivationDayRule",
                "value": "Grant"
            },
            {
                "key": "ApprovalRule",
                "value": "Grant"
            }
        ]
    },
    "schedule": {
        "type": "Once",
        "startDateTime": "2018-05-12T23:28:43.537Z",
        "endDateTime": "0001-01-01T00:00:00Z",
        "duration": "PT9H"
    }
}
```

## <a name="example-3"></a><span data-ttu-id="cc11f-282">示例 3</span><span class="sxs-lookup"><span data-stu-id="cc11f-282">Example 3</span></span>
<span data-ttu-id="cc11f-283">本示例中，用户 nawu@fimdev.net 停用活动的帐单读取器角色。</span><span class="sxs-lookup"><span data-stu-id="cc11f-283">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="cc11f-284">属性</span><span class="sxs-lookup"><span data-stu-id="cc11f-284">Property</span></span>     | <span data-ttu-id="cc11f-285">类型</span><span class="sxs-lookup"><span data-stu-id="cc11f-285">Type</span></span>    |<span data-ttu-id="cc11f-286">是否必需</span><span class="sxs-lookup"><span data-stu-id="cc11f-286">Required</span></span>|  <span data-ttu-id="cc11f-287">值</span><span class="sxs-lookup"><span data-stu-id="cc11f-287">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="cc11f-288">resourceId</span><span class="sxs-lookup"><span data-stu-id="cc11f-288">resourceId</span></span>|<span data-ttu-id="cc11f-289">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-289">String</span></span>|<span data-ttu-id="cc11f-290">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-290">Yes</span></span>|<span data-ttu-id="cc11f-291">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="cc11f-291">\<resourceId\></span></span>|
|<span data-ttu-id="cc11f-292">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="cc11f-292">roleDefinitionId</span></span>|<span data-ttu-id="cc11f-293">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-293">String</span></span>|<span data-ttu-id="cc11f-294">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-294">Yes</span></span>|<span data-ttu-id="cc11f-295">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="cc11f-295">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="cc11f-296">subjectId</span><span class="sxs-lookup"><span data-stu-id="cc11f-296">subjectId</span></span>|<span data-ttu-id="cc11f-297">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-297">String</span></span>|<span data-ttu-id="cc11f-298">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-298">Yes</span></span>|<span data-ttu-id="cc11f-299">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="cc11f-299">\<subjectId\></span></span>|
|<span data-ttu-id="cc11f-300">assignmentState</span><span class="sxs-lookup"><span data-stu-id="cc11f-300">assignmentState</span></span>|<span data-ttu-id="cc11f-301">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-301">String</span></span>|<span data-ttu-id="cc11f-302">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-302">Yes</span></span>| <span data-ttu-id="cc11f-303">活跃</span><span class="sxs-lookup"><span data-stu-id="cc11f-303">Active</span></span>|
|<span data-ttu-id="cc11f-304">type</span><span class="sxs-lookup"><span data-stu-id="cc11f-304">type</span></span>|<span data-ttu-id="cc11f-305">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-305">String</span></span>|<span data-ttu-id="cc11f-306">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-306">Yes</span></span>| <span data-ttu-id="cc11f-307">UserRemove</span><span class="sxs-lookup"><span data-stu-id="cc11f-307">UserRemove</span></span>|
|<span data-ttu-id="cc11f-308">原因</span><span class="sxs-lookup"><span data-stu-id="cc11f-308">reason</span></span>|<span data-ttu-id="cc11f-309">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-309">String</span></span>| <span data-ttu-id="cc11f-310">否</span><span class="sxs-lookup"><span data-stu-id="cc11f-310">No</span></span>||
|<span data-ttu-id="cc11f-311">计划</span><span class="sxs-lookup"><span data-stu-id="cc11f-311">schedule</span></span>|[<span data-ttu-id="cc11f-312">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="cc11f-312">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="cc11f-313">否</span><span class="sxs-lookup"><span data-stu-id="cc11f-313">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="cc11f-314">请求</span><span class="sxs-lookup"><span data-stu-id="cc11f-314">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"bc75b4e6-7403-4243-bf2f-d1f6990be122",
"resourceId":"fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Active",
"type":"UserRemove",
"reason":"Deactivate the role",
"linkedEligibleRoleAssignmentId":"cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```
##### <a name="response"></a><span data-ttu-id="cc11f-315">响应</span><span class="sxs-lookup"><span data-stu-id="cc11f-315">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
    "id": "abfcdb57-8e5d-42a0-ae67-7598b96fddb1",
    "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
    "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
    "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
    "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec",
    "type": "UserRemove",
    "assignmentState": "Active",
    "requestedDateTime": "0001-01-01T00:00:00Z",
    "roleAssignmentStartDateTime": null,
    "roleAssignmentEndDateTime": null,
    "reason": "Evaluate only",
    "schedule": null,
    "status": {
        "status": "Closed",
        "subStatus": "Revoked",
        "statusDetails": []
    }
}
```

### <a name="example-4"></a><span data-ttu-id="cc11f-316">示例 4</span><span class="sxs-lookup"><span data-stu-id="cc11f-316">Example 4</span></span>
<span data-ttu-id="cc11f-317">本示例中，管理员从帐单读者角色中移除用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="cc11f-317">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="cc11f-318">**注意：** 除了权限范围，此示例要求至少有一个请求程序`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="cc11f-318">**Note:** Besides the permission scope, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="cc11f-319">属性</span><span class="sxs-lookup"><span data-stu-id="cc11f-319">Property</span></span>     | <span data-ttu-id="cc11f-320">类型</span><span class="sxs-lookup"><span data-stu-id="cc11f-320">Type</span></span>    |<span data-ttu-id="cc11f-321">是否必需</span><span class="sxs-lookup"><span data-stu-id="cc11f-321">Required</span></span>|  <span data-ttu-id="cc11f-322">值</span><span class="sxs-lookup"><span data-stu-id="cc11f-322">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="cc11f-323">resourceId</span><span class="sxs-lookup"><span data-stu-id="cc11f-323">resourceId</span></span>|<span data-ttu-id="cc11f-324">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-324">String</span></span>|<span data-ttu-id="cc11f-325">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-325">Yes</span></span>|<span data-ttu-id="cc11f-326">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="cc11f-326">\<resourceId\></span></span>|
|<span data-ttu-id="cc11f-327">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="cc11f-327">roleDefinitionId</span></span>|<span data-ttu-id="cc11f-328">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-328">String</span></span>|<span data-ttu-id="cc11f-329">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-329">Yes</span></span>|<span data-ttu-id="cc11f-330">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="cc11f-330">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="cc11f-331">subjectId</span><span class="sxs-lookup"><span data-stu-id="cc11f-331">subjectId</span></span>|<span data-ttu-id="cc11f-332">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-332">String</span></span>|<span data-ttu-id="cc11f-333">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-333">Yes</span></span>|<span data-ttu-id="cc11f-334">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="cc11f-334">\<subjectId\></span></span>|
|<span data-ttu-id="cc11f-335">assignmentState</span><span class="sxs-lookup"><span data-stu-id="cc11f-335">assignmentState</span></span>|<span data-ttu-id="cc11f-336">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-336">String</span></span>|<span data-ttu-id="cc11f-337">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-337">Yes</span></span>| <span data-ttu-id="cc11f-338">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="cc11f-338">Eligible / Active</span></span>|
|<span data-ttu-id="cc11f-339">type</span><span class="sxs-lookup"><span data-stu-id="cc11f-339">type</span></span>|<span data-ttu-id="cc11f-340">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-340">String</span></span>|<span data-ttu-id="cc11f-341">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-341">Yes</span></span>| <span data-ttu-id="cc11f-342">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="cc11f-342">AdminRemove</span></span>|
|<span data-ttu-id="cc11f-343">原因</span><span class="sxs-lookup"><span data-stu-id="cc11f-343">reason</span></span>|<span data-ttu-id="cc11f-344">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-344">String</span></span>| <span data-ttu-id="cc11f-345">否</span><span class="sxs-lookup"><span data-stu-id="cc11f-345">No</span></span>||
|<span data-ttu-id="cc11f-346">计划</span><span class="sxs-lookup"><span data-stu-id="cc11f-346">schedule</span></span>|[<span data-ttu-id="cc11f-347">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="cc11f-347">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="cc11f-348">否</span><span class="sxs-lookup"><span data-stu-id="cc11f-348">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="cc11f-349">请求</span><span class="sxs-lookup"><span data-stu-id="cc11f-349">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState":"Eligible",
  "type":"AdminRemove"
}
```
##### <a name="response"></a><span data-ttu-id="cc11f-350">响应</span><span class="sxs-lookup"><span data-stu-id="cc11f-350">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminRemove",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "roleAssignmentStartDateTime":null,
  "roleAssignmentEndDateTime":null,
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```

### <a name="example-5"></a><span data-ttu-id="cc11f-351">示例 5</span><span class="sxs-lookup"><span data-stu-id="cc11f-351">Example 5</span></span>
<span data-ttu-id="cc11f-352">本示例中，管理员向所有者更新用户 nawu@fimdev.net 的角色分配。</span><span class="sxs-lookup"><span data-stu-id="cc11f-352">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="cc11f-353">**注意：** 除了权限范围，此示例要求至少有一个请求程序`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="cc11f-353">**Note:** Besides the permission scope, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 
| <span data-ttu-id="cc11f-354">属性</span><span class="sxs-lookup"><span data-stu-id="cc11f-354">Property</span></span>     | <span data-ttu-id="cc11f-355">类型</span><span class="sxs-lookup"><span data-stu-id="cc11f-355">Type</span></span>    |<span data-ttu-id="cc11f-356">是否必需</span><span class="sxs-lookup"><span data-stu-id="cc11f-356">Required</span></span>|  <span data-ttu-id="cc11f-357">值</span><span class="sxs-lookup"><span data-stu-id="cc11f-357">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="cc11f-358">resourceId</span><span class="sxs-lookup"><span data-stu-id="cc11f-358">resourceId</span></span>|<span data-ttu-id="cc11f-359">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-359">String</span></span>|<span data-ttu-id="cc11f-360">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-360">Yes</span></span>|<span data-ttu-id="cc11f-361">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="cc11f-361">\<resourceId\></span></span>|
|<span data-ttu-id="cc11f-362">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="cc11f-362">roleDefinitionId</span></span>|<span data-ttu-id="cc11f-363">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-363">String</span></span>|<span data-ttu-id="cc11f-364">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-364">Yes</span></span>|<span data-ttu-id="cc11f-365">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="cc11f-365">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="cc11f-366">subjectId</span><span class="sxs-lookup"><span data-stu-id="cc11f-366">subjectId</span></span>|<span data-ttu-id="cc11f-367">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-367">String</span></span>|<span data-ttu-id="cc11f-368">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-368">Yes</span></span>|<span data-ttu-id="cc11f-369">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="cc11f-369">\<subjectId\></span></span>|
|<span data-ttu-id="cc11f-370">assignmentState</span><span class="sxs-lookup"><span data-stu-id="cc11f-370">assignmentState</span></span>|<span data-ttu-id="cc11f-371">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-371">String</span></span>|<span data-ttu-id="cc11f-372">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-372">Yes</span></span>| <span data-ttu-id="cc11f-373">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="cc11f-373">Eligible / Active</span></span>|
|<span data-ttu-id="cc11f-374">type</span><span class="sxs-lookup"><span data-stu-id="cc11f-374">type</span></span>|<span data-ttu-id="cc11f-375">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-375">String</span></span>|<span data-ttu-id="cc11f-376">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-376">Yes</span></span>| <span data-ttu-id="cc11f-377">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="cc11f-377">AdminUpdate</span></span>|
|<span data-ttu-id="cc11f-378">原因</span><span class="sxs-lookup"><span data-stu-id="cc11f-378">reason</span></span>|<span data-ttu-id="cc11f-379">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-379">String</span></span>| <span data-ttu-id="cc11f-380">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="cc11f-380">depends on roleSettings</span></span>||
|<span data-ttu-id="cc11f-381">计划</span><span class="sxs-lookup"><span data-stu-id="cc11f-381">schedule</span></span>|[<span data-ttu-id="cc11f-382">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="cc11f-382">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="cc11f-383">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-383">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="cc11f-384">请求</span><span class="sxs-lookup"><span data-stu-id="cc11f-384">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState":"Eligible",
  "type":"AdminUpdate",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-03-08T05:42:45.317Z",
    "endDateTime":"2018-06-05T05:42:31.000Z"
  }
}
```
##### <a name="response"></a><span data-ttu-id="cc11f-385">响应</span><span class="sxs-lookup"><span data-stu-id="cc11f-385">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId":"1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminUpdate",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "roleAssignmentStartDateTime":"2018-05-12T23:50:03.4755896Z",
  "roleAssignmentEndDateTime":"2018-06-05T05:42:31Z",
  "reason":null,
  "status":{
    "status":"InProgress",
    "subStatus":"Granted",
    "statusDetails":[
      {
        "key":"AdminRequestRule","value":"Grant"
      },{
        "key":"ExpirationRule","value":"Grant"
      },{
        "key":"MfaRule","value":"Grant"
      }
    ]
  },
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-03-08T05:42:45.317Z",
    "endDateTime":"2018-06-05T05:42:31Z",
    "duration":"PT0S"
  }
}
```

### <a name="example-6"></a><span data-ttu-id="cc11f-386">示例 6</span><span class="sxs-lookup"><span data-stu-id="cc11f-386">Example 6</span></span>
<span data-ttu-id="cc11f-387">本示例将用户 ANUJCUSER 即将过期的角色分配给 API 管理服务参与者。</span><span class="sxs-lookup"><span data-stu-id="cc11f-387">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="cc11f-388">**注意：** 除了权限范围，此示例要求至少有一个请求程序`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="cc11f-388">**Note:** Besides the permission scope, this example requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="cc11f-389">属性</span><span class="sxs-lookup"><span data-stu-id="cc11f-389">Property</span></span>     | <span data-ttu-id="cc11f-390">类型</span><span class="sxs-lookup"><span data-stu-id="cc11f-390">Type</span></span>    |<span data-ttu-id="cc11f-391">是否必需</span><span class="sxs-lookup"><span data-stu-id="cc11f-391">Required</span></span>|  <span data-ttu-id="cc11f-392">值</span><span class="sxs-lookup"><span data-stu-id="cc11f-392">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="cc11f-393">resourceId</span><span class="sxs-lookup"><span data-stu-id="cc11f-393">resourceId</span></span>|<span data-ttu-id="cc11f-394">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-394">String</span></span>|<span data-ttu-id="cc11f-395">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-395">Yes</span></span>|<span data-ttu-id="cc11f-396">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="cc11f-396">\<resourceId\></span></span>|
|<span data-ttu-id="cc11f-397">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="cc11f-397">roleDefinitionId</span></span>|<span data-ttu-id="cc11f-398">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-398">String</span></span>|<span data-ttu-id="cc11f-399">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-399">Yes</span></span>|<span data-ttu-id="cc11f-400">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="cc11f-400">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="cc11f-401">subjectId</span><span class="sxs-lookup"><span data-stu-id="cc11f-401">subjectId</span></span>|<span data-ttu-id="cc11f-402">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-402">String</span></span>|<span data-ttu-id="cc11f-403">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-403">Yes</span></span>|<span data-ttu-id="cc11f-404">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="cc11f-404">\<subjectId\></span></span>|
|<span data-ttu-id="cc11f-405">assignmentState</span><span class="sxs-lookup"><span data-stu-id="cc11f-405">assignmentState</span></span>|<span data-ttu-id="cc11f-406">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-406">String</span></span>|<span data-ttu-id="cc11f-407">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-407">Yes</span></span>| <span data-ttu-id="cc11f-408">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="cc11f-408">Eligible / Active</span></span> |
|<span data-ttu-id="cc11f-409">type</span><span class="sxs-lookup"><span data-stu-id="cc11f-409">type</span></span>|<span data-ttu-id="cc11f-410">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-410">String</span></span>|<span data-ttu-id="cc11f-411">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-411">Yes</span></span>| <span data-ttu-id="cc11f-412">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="cc11f-412">AdminExtend</span></span>|
|<span data-ttu-id="cc11f-413">原因</span><span class="sxs-lookup"><span data-stu-id="cc11f-413">reason</span></span>|<span data-ttu-id="cc11f-414">字符串</span><span class="sxs-lookup"><span data-stu-id="cc11f-414">String</span></span>| <span data-ttu-id="cc11f-415">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="cc11f-415">depends on roleSettings</span></span>||
|<span data-ttu-id="cc11f-416">计划</span><span class="sxs-lookup"><span data-stu-id="cc11f-416">schedule</span></span>|[<span data-ttu-id="cc11f-417">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="cc11f-417">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="cc11f-418">是</span><span class="sxs-lookup"><span data-stu-id="cc11f-418">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="cc11f-419">请求</span><span class="sxs-lookup"><span data-stu-id="cc11f-419">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState":"Eligible",
  "type":"AdminExtend",
  "reason":"extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-05-12T23:53:55.327Z",
    "endDateTime":"2018-08-10T23:53:55.327Z"
  }
}
```
##### <a name="response"></a><span data-ttu-id="cc11f-420">响应</span><span class="sxs-lookup"><span data-stu-id="cc11f-420">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminExtend",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "roleAssignmentStartDateTime":"2018-05-12T23:54:09.7221332Z",
  "roleAssignmentEndDateTime":"2018-08-10T23:53:55.327Z",
  "reason":"extend role assignment",
  "status":{
    "status":"InProgress",
    "subStatus":"Granted",
    "statusDetails":[
      {
        "key":"AdminRequestRule","value":"Grant"
      },{
        "key":"ExpirationRule","value":"Grant"
      },{
        "key":"MfaRule","value":"Grant"
      }
    ]
  },
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-05-12T23:53:55.327Z",
    "endDateTime":"2018-08-10T23:53:55.327Z",
    "duration":"PT0S"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
