---
title: 创建 governanceRoleAssignmentRequest
description: 创建角色分配请求以表示该操作所需角色分配。 下表列出的操作。
ms.openlocfilehash: 775cc8e22e7d273bfe387e5be2cc183d3d919a38
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191170"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="4ce8a-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="4ce8a-104">Create governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="4ce8a-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ce8a-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ce8a-107">创建角色分配请求以表示该操作所需角色分配。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-107">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="4ce8a-108">下表列出的操作。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-108">The following table lists the operations.</span></span>

| <span data-ttu-id="4ce8a-109">操作</span><span class="sxs-lookup"><span data-stu-id="4ce8a-109">Operation</span></span>       | <span data-ttu-id="4ce8a-110">类型</span><span class="sxs-lookup"><span data-stu-id="4ce8a-110">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="4ce8a-111">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="4ce8a-111">Assign a role assignment</span></span>| <span data-ttu-id="4ce8a-112">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="4ce8a-112">AdminAdd</span></span> |
| <span data-ttu-id="4ce8a-113">激活合格的角色分配</span><span class="sxs-lookup"><span data-stu-id="4ce8a-113">Activate an eligible role assignment</span></span>| <span data-ttu-id="4ce8a-114">UserAdd</span><span class="sxs-lookup"><span data-stu-id="4ce8a-114">UserAdd</span></span> | 
| <span data-ttu-id="4ce8a-115">停用已激活的角色分配</span><span class="sxs-lookup"><span data-stu-id="4ce8a-115">Deactivate an activated role assignment</span></span>| <span data-ttu-id="4ce8a-116">UserRemove</span><span class="sxs-lookup"><span data-stu-id="4ce8a-116">UserRemove</span></span> | 
| <span data-ttu-id="4ce8a-117">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="4ce8a-117">Remove a role assignment</span></span>| <span data-ttu-id="4ce8a-118">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="4ce8a-118">AdminRemove</span></span> |
| <span data-ttu-id="4ce8a-119">更新一个角色分配</span><span class="sxs-lookup"><span data-stu-id="4ce8a-119">Update a role assignment</span></span>| <span data-ttu-id="4ce8a-120">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="4ce8a-120">AdminUpdate</span></span> |
| <span data-ttu-id="4ce8a-121">请求扩展我角色分配</span><span class="sxs-lookup"><span data-stu-id="4ce8a-121">Request to extend my role assignment</span></span>| <span data-ttu-id="4ce8a-122">UserExtend</span><span class="sxs-lookup"><span data-stu-id="4ce8a-122">UserExtend</span></span> | 
| <span data-ttu-id="4ce8a-123">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="4ce8a-123">Extend a role assignment</span></span>| <span data-ttu-id="4ce8a-124">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="4ce8a-124">AdminExtend</span></span> | 
| <span data-ttu-id="4ce8a-125">请求续订我过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="4ce8a-125">Request to renew my expired role assignment</span></span>| <span data-ttu-id="4ce8a-126">UserRenew</span><span class="sxs-lookup"><span data-stu-id="4ce8a-126">UserRenew</span></span> | 
| <span data-ttu-id="4ce8a-127">续订已过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="4ce8a-127">Renew an expired role assignment</span></span>| <span data-ttu-id="4ce8a-128">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="4ce8a-128">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="4ce8a-129">权限</span><span class="sxs-lookup"><span data-stu-id="4ce8a-129">Permissions</span></span>
<span data-ttu-id="4ce8a-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ce8a-132">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ce8a-132">Permission type</span></span>      | <span data-ttu-id="4ce8a-133">Permissions</span><span class="sxs-lookup"><span data-stu-id="4ce8a-133">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ce8a-134">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ce8a-134">Delegated (work or school account)</span></span> | <span data-ttu-id="4ce8a-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="4ce8a-135">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="4ce8a-136">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ce8a-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ce8a-137">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-137">Not supported.</span></span>    |
|<span data-ttu-id="4ce8a-138">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ce8a-138">Application</span></span> | <span data-ttu-id="4ce8a-139">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="4ce8a-139">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ce8a-140">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ce8a-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="4ce8a-141">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ce8a-141">Request headers</span></span>
| <span data-ttu-id="4ce8a-142">名称</span><span class="sxs-lookup"><span data-stu-id="4ce8a-142">Name</span></span>       | <span data-ttu-id="4ce8a-143">说明</span><span class="sxs-lookup"><span data-stu-id="4ce8a-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4ce8a-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ce8a-144">Authorization</span></span>  | <span data-ttu-id="4ce8a-145">持有者 {code}</span><span class="sxs-lookup"><span data-stu-id="4ce8a-145">Bearer {code}</span></span>|
| <span data-ttu-id="4ce8a-146">Content-type</span><span class="sxs-lookup"><span data-stu-id="4ce8a-146">Content-type</span></span>  | <span data-ttu-id="4ce8a-147">application/json</span><span class="sxs-lookup"><span data-stu-id="4ce8a-147">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ce8a-148">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ce8a-148">Request body</span></span>
<span data-ttu-id="4ce8a-149">在请求正文中，提供[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-149">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="4ce8a-150">属性</span><span class="sxs-lookup"><span data-stu-id="4ce8a-150">Property</span></span>     | <span data-ttu-id="4ce8a-151">类型</span><span class="sxs-lookup"><span data-stu-id="4ce8a-151">Type</span></span>    |<span data-ttu-id="4ce8a-152">必需</span><span class="sxs-lookup"><span data-stu-id="4ce8a-152">Required</span></span>|  <span data-ttu-id="4ce8a-153">说明</span><span class="sxs-lookup"><span data-stu-id="4ce8a-153">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="4ce8a-154">resourceId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-154">resourceId</span></span>|<span data-ttu-id="4ce8a-155">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-155">String</span></span>|<span data-ttu-id="4ce8a-156">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-156">Yes</span></span>|<span data-ttu-id="4ce8a-157">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-157">The ID of the resource.</span></span>|
|<span data-ttu-id="4ce8a-158">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-158">roleDefinitionId</span></span>|<span data-ttu-id="4ce8a-159">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-159">String</span></span>|<span data-ttu-id="4ce8a-160">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-160">Yes</span></span>|<span data-ttu-id="4ce8a-161">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-161">The ID of the role definition.</span></span>|
|<span data-ttu-id="4ce8a-162">subjectId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-162">subjectId</span></span>|<span data-ttu-id="4ce8a-163">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-163">String</span></span>|<span data-ttu-id="4ce8a-164">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-164">Yes</span></span>|<span data-ttu-id="4ce8a-165">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-165">The ID of the subject.</span></span>|
|<span data-ttu-id="4ce8a-166">assignmentState</span><span class="sxs-lookup"><span data-stu-id="4ce8a-166">assignmentState</span></span>|<span data-ttu-id="4ce8a-167">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-167">String</span></span>|<span data-ttu-id="4ce8a-168">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-168">Yes</span></span>|<span data-ttu-id="4ce8a-169">工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-169">The state of assignment.</span></span> <span data-ttu-id="4ce8a-170">值可以是``Eligible``和``Active``。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-170">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="4ce8a-171">type</span><span class="sxs-lookup"><span data-stu-id="4ce8a-171">type</span></span>|<span data-ttu-id="4ce8a-172">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-172">String</span></span>|<span data-ttu-id="4ce8a-173">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-173">Yes</span></span>|<span data-ttu-id="4ce8a-174">请求类型。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-174">The request type.</span></span> <span data-ttu-id="4ce8a-175">值可以是`AdminAdd`， `UserAdd`， `AdminUpdate`， `AdminRemove`， `UserRemove`， `UserExtend`， `UserRenew`，`AdminRenew`和`AdminExtend`。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-175">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="4ce8a-176">原因</span><span class="sxs-lookup"><span data-stu-id="4ce8a-176">reason</span></span>|<span data-ttu-id="4ce8a-177">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-177">String</span></span>| |<span data-ttu-id="4ce8a-178">原因需要提供角色分配请求的审核和查看用途。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-178">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="4ce8a-179">计划</span><span class="sxs-lookup"><span data-stu-id="4ce8a-179">schedule</span></span>|[<span data-ttu-id="4ce8a-180">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4ce8a-180">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="4ce8a-181">角色分配请求的时间表。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-181">The schedule of the role assignment request.</span></span> <span data-ttu-id="4ce8a-182">请求类型的`UserAdd`， `AdminAdd`， `AdminUpdate`，和`AdminExtend`，需要。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-182">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

## <a name="response"></a><span data-ttu-id="4ce8a-183">响应</span><span class="sxs-lookup"><span data-stu-id="4ce8a-183">Response</span></span>
<span data-ttu-id="4ce8a-184">如果成功，此方法返回`201 Created`响应代码和响应正文中的[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-184">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="4ce8a-185">错误代码</span><span class="sxs-lookup"><span data-stu-id="4ce8a-185">Error codes</span></span>
<span data-ttu-id="4ce8a-186">此 API 返回的标准 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-186">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="4ce8a-187">此外，它也会返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-187">In addition, it also returns the error codes listed in the following table.</span></span>

|<span data-ttu-id="4ce8a-188">错误代码</span><span class="sxs-lookup"><span data-stu-id="4ce8a-188">Error code</span></span>     | <span data-ttu-id="4ce8a-189">错误消息</span><span class="sxs-lookup"><span data-stu-id="4ce8a-189">Error message</span></span>              | <span data-ttu-id="4ce8a-190">详细信息</span><span class="sxs-lookup"><span data-stu-id="4ce8a-190">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="4ce8a-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4ce8a-191">400 BadRequest</span></span> | <span data-ttu-id="4ce8a-192">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="4ce8a-192">RoleNotFound</span></span>    | <span data-ttu-id="4ce8a-193">`roleDefinitionId`提供在请求正文找不到。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-193">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="4ce8a-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4ce8a-194">400 BadRequest</span></span> | <span data-ttu-id="4ce8a-195">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="4ce8a-195">ResourceIsLocked</span></span>    | <span data-ttu-id="4ce8a-196">在请求正文中提供的资源处于状态的`Locked`和无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-196">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="4ce8a-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4ce8a-197">400 BadRequest</span></span> | <span data-ttu-id="4ce8a-198">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="4ce8a-198">SubjectNotFound</span></span>    | <span data-ttu-id="4ce8a-199">`subjectId`提供在请求正文找不到。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-199">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="4ce8a-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4ce8a-200">400 BadRequest</span></span> | <span data-ttu-id="4ce8a-201">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="4ce8a-201">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="4ce8a-202">已存在挂起[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)系统中。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-202">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="4ce8a-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4ce8a-203">400 BadRequest</span></span> | <span data-ttu-id="4ce8a-204">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="4ce8a-204">RoleAssignmentExists</span></span>    | <span data-ttu-id="4ce8a-205">系统中存在[governanceRoleAssignment](../resources/governanceroleassignment.md)请求已创建。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="4ce8a-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4ce8a-206">400 BadRequest</span></span> | <span data-ttu-id="4ce8a-207">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="4ce8a-207">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="4ce8a-208">系统中不存在[governanceRoleAssignment](../resources/governanceroleassignment.md)请求来更新/扩展。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-208">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="4ce8a-209">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4ce8a-209">400 BadRequest</span></span> | <span data-ttu-id="4ce8a-210">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="4ce8a-210">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="4ce8a-211">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部的策略，且无法创建。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-211">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="examples"></a><span data-ttu-id="4ce8a-212">示例</span><span class="sxs-lookup"><span data-stu-id="4ce8a-212">Examples</span></span>
<span data-ttu-id="4ce8a-213">下面的示例演示如何使用此 API。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-213">The following examples show how to use this API.</span></span>

### <a name="example-1"></a><span data-ttu-id="4ce8a-214">示例 1</span><span class="sxs-lookup"><span data-stu-id="4ce8a-214">Example 1</span></span>
<span data-ttu-id="4ce8a-215">本示例中，管理员为帐单读者角色分配用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-215">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="4ce8a-216">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-216">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="4ce8a-217">属性</span><span class="sxs-lookup"><span data-stu-id="4ce8a-217">Property</span></span>     | <span data-ttu-id="4ce8a-218">类型</span><span class="sxs-lookup"><span data-stu-id="4ce8a-218">Type</span></span>    |<span data-ttu-id="4ce8a-219">是否必需</span><span class="sxs-lookup"><span data-stu-id="4ce8a-219">Required</span></span>|  <span data-ttu-id="4ce8a-220">值</span><span class="sxs-lookup"><span data-stu-id="4ce8a-220">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="4ce8a-221">resourceId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-221">resourceId</span></span>|<span data-ttu-id="4ce8a-222">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-222">String</span></span>|<span data-ttu-id="4ce8a-223">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-223">Yes</span></span>|<span data-ttu-id="4ce8a-224">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="4ce8a-224">\<resourceId\></span></span>|
|<span data-ttu-id="4ce8a-225">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-225">roleDefinitionId</span></span>|<span data-ttu-id="4ce8a-226">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-226">String</span></span>|<span data-ttu-id="4ce8a-227">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-227">Yes</span></span>|<span data-ttu-id="4ce8a-228">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="4ce8a-228">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="4ce8a-229">subjectId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-229">subjectId</span></span>|<span data-ttu-id="4ce8a-230">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-230">String</span></span>|<span data-ttu-id="4ce8a-231">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-231">Yes</span></span>|<span data-ttu-id="4ce8a-232">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="4ce8a-232">\<subjectId\></span></span>|
|<span data-ttu-id="4ce8a-233">assignmentState</span><span class="sxs-lookup"><span data-stu-id="4ce8a-233">assignmentState</span></span>|<span data-ttu-id="4ce8a-234">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-234">String</span></span>|<span data-ttu-id="4ce8a-235">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-235">Yes</span></span>| <span data-ttu-id="4ce8a-236">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="4ce8a-236">Eligible / Active</span></span>|
|<span data-ttu-id="4ce8a-237">type</span><span class="sxs-lookup"><span data-stu-id="4ce8a-237">type</span></span>|<span data-ttu-id="4ce8a-238">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-238">String</span></span>|<span data-ttu-id="4ce8a-239">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-239">Yes</span></span>| <span data-ttu-id="4ce8a-240">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="4ce8a-240">AdminAdd</span></span>|
|<span data-ttu-id="4ce8a-241">原因</span><span class="sxs-lookup"><span data-stu-id="4ce8a-241">reason</span></span>|<span data-ttu-id="4ce8a-242">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-242">String</span></span>| <span data-ttu-id="4ce8a-243">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="4ce8a-243">depends on role Settings</span></span>||
|<span data-ttu-id="4ce8a-244">计划</span><span class="sxs-lookup"><span data-stu-id="4ce8a-244">schedule</span></span>|[<span data-ttu-id="4ce8a-245">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4ce8a-245">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="4ce8a-246">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-246">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="4ce8a-247">请求</span><span class="sxs-lookup"><span data-stu-id="4ce8a-247">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="4ce8a-248">响应</span><span class="sxs-lookup"><span data-stu-id="4ce8a-248">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="4ce8a-249">示例 2</span><span class="sxs-lookup"><span data-stu-id="4ce8a-249">Example 2</span></span>
<span data-ttu-id="4ce8a-250">本示例中，用户 nawu@fimdev.net 激活合格的帐单读取器角色。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-250">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="4ce8a-251">属性</span><span class="sxs-lookup"><span data-stu-id="4ce8a-251">Property</span></span>     | <span data-ttu-id="4ce8a-252">类型</span><span class="sxs-lookup"><span data-stu-id="4ce8a-252">Type</span></span>    |<span data-ttu-id="4ce8a-253">是否必需</span><span class="sxs-lookup"><span data-stu-id="4ce8a-253">Required</span></span>|  <span data-ttu-id="4ce8a-254">值</span><span class="sxs-lookup"><span data-stu-id="4ce8a-254">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="4ce8a-255">resourceId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-255">resourceId</span></span>|<span data-ttu-id="4ce8a-256">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-256">String</span></span>|<span data-ttu-id="4ce8a-257">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-257">Yes</span></span>|<span data-ttu-id="4ce8a-258">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="4ce8a-258">\<resourceId\></span></span>|
|<span data-ttu-id="4ce8a-259">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-259">roleDefinitionId</span></span>|<span data-ttu-id="4ce8a-260">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-260">String</span></span>|<span data-ttu-id="4ce8a-261">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-261">Yes</span></span>|<span data-ttu-id="4ce8a-262">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="4ce8a-262">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="4ce8a-263">subjectId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-263">subjectId</span></span>|<span data-ttu-id="4ce8a-264">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-264">String</span></span>|<span data-ttu-id="4ce8a-265">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-265">Yes</span></span>|<span data-ttu-id="4ce8a-266">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="4ce8a-266">\<subjectId\></span></span>|
|<span data-ttu-id="4ce8a-267">assignmentState</span><span class="sxs-lookup"><span data-stu-id="4ce8a-267">assignmentState</span></span>|<span data-ttu-id="4ce8a-268">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-268">String</span></span>|<span data-ttu-id="4ce8a-269">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-269">Yes</span></span>| <span data-ttu-id="4ce8a-270">活跃</span><span class="sxs-lookup"><span data-stu-id="4ce8a-270">Active</span></span>|
|<span data-ttu-id="4ce8a-271">type</span><span class="sxs-lookup"><span data-stu-id="4ce8a-271">type</span></span>|<span data-ttu-id="4ce8a-272">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-272">String</span></span>|<span data-ttu-id="4ce8a-273">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-273">Yes</span></span>| <span data-ttu-id="4ce8a-274">UserAdd</span><span class="sxs-lookup"><span data-stu-id="4ce8a-274">UserAdd</span></span>|
|<span data-ttu-id="4ce8a-275">原因</span><span class="sxs-lookup"><span data-stu-id="4ce8a-275">reason</span></span>|<span data-ttu-id="4ce8a-276">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-276">String</span></span>| <span data-ttu-id="4ce8a-277">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="4ce8a-277">depends on role Settings</span></span>||
|<span data-ttu-id="4ce8a-278">计划</span><span class="sxs-lookup"><span data-stu-id="4ce8a-278">schedule</span></span>|[<span data-ttu-id="4ce8a-279">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4ce8a-279">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="4ce8a-280">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-280">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="4ce8a-281">请求</span><span class="sxs-lookup"><span data-stu-id="4ce8a-281">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="4ce8a-282">响应</span><span class="sxs-lookup"><span data-stu-id="4ce8a-282">Response</span></span>
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

### <a name="example-3"></a><span data-ttu-id="4ce8a-283">示例 3</span><span class="sxs-lookup"><span data-stu-id="4ce8a-283">Example 3</span></span>
<span data-ttu-id="4ce8a-284">本示例中，用户 nawu@fimdev.net 停用活动的帐单读取器角色。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-284">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="4ce8a-285">属性</span><span class="sxs-lookup"><span data-stu-id="4ce8a-285">Property</span></span>     | <span data-ttu-id="4ce8a-286">类型</span><span class="sxs-lookup"><span data-stu-id="4ce8a-286">Type</span></span>    |<span data-ttu-id="4ce8a-287">是否必需</span><span class="sxs-lookup"><span data-stu-id="4ce8a-287">Required</span></span>|  <span data-ttu-id="4ce8a-288">值</span><span class="sxs-lookup"><span data-stu-id="4ce8a-288">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="4ce8a-289">resourceId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-289">resourceId</span></span>|<span data-ttu-id="4ce8a-290">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-290">String</span></span>|<span data-ttu-id="4ce8a-291">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-291">Yes</span></span>|<span data-ttu-id="4ce8a-292">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="4ce8a-292">\<resourceId\></span></span>|
|<span data-ttu-id="4ce8a-293">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-293">roleDefinitionId</span></span>|<span data-ttu-id="4ce8a-294">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-294">String</span></span>|<span data-ttu-id="4ce8a-295">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-295">Yes</span></span>|<span data-ttu-id="4ce8a-296">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="4ce8a-296">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="4ce8a-297">subjectId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-297">subjectId</span></span>|<span data-ttu-id="4ce8a-298">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-298">String</span></span>|<span data-ttu-id="4ce8a-299">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-299">Yes</span></span>|<span data-ttu-id="4ce8a-300">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="4ce8a-300">\<subjectId\></span></span>|
|<span data-ttu-id="4ce8a-301">assignmentState</span><span class="sxs-lookup"><span data-stu-id="4ce8a-301">assignmentState</span></span>|<span data-ttu-id="4ce8a-302">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-302">String</span></span>|<span data-ttu-id="4ce8a-303">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-303">Yes</span></span>| <span data-ttu-id="4ce8a-304">活跃</span><span class="sxs-lookup"><span data-stu-id="4ce8a-304">Active</span></span>|
|<span data-ttu-id="4ce8a-305">type</span><span class="sxs-lookup"><span data-stu-id="4ce8a-305">type</span></span>|<span data-ttu-id="4ce8a-306">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-306">String</span></span>|<span data-ttu-id="4ce8a-307">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-307">Yes</span></span>| <span data-ttu-id="4ce8a-308">UserRemove</span><span class="sxs-lookup"><span data-stu-id="4ce8a-308">UserRemove</span></span>|
|<span data-ttu-id="4ce8a-309">原因</span><span class="sxs-lookup"><span data-stu-id="4ce8a-309">reason</span></span>|<span data-ttu-id="4ce8a-310">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-310">String</span></span>| <span data-ttu-id="4ce8a-311">否</span><span class="sxs-lookup"><span data-stu-id="4ce8a-311">No</span></span>||
|<span data-ttu-id="4ce8a-312">计划</span><span class="sxs-lookup"><span data-stu-id="4ce8a-312">schedule</span></span>|[<span data-ttu-id="4ce8a-313">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4ce8a-313">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="4ce8a-314">否</span><span class="sxs-lookup"><span data-stu-id="4ce8a-314">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="4ce8a-315">请求</span><span class="sxs-lookup"><span data-stu-id="4ce8a-315">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="4ce8a-316">响应</span><span class="sxs-lookup"><span data-stu-id="4ce8a-316">Response</span></span>
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
    "reason": "Evaluate only",
    "schedule": null,
    "status": {
        "status": "Closed",
        "subStatus": "Revoked",
        "statusDetails": []
    }
}
```

### <a name="example-4"></a><span data-ttu-id="4ce8a-317">示例 4</span><span class="sxs-lookup"><span data-stu-id="4ce8a-317">Example 4</span></span>
<span data-ttu-id="4ce8a-318">本示例中，管理员从帐单读者角色中移除用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-318">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="4ce8a-319">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-319">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="4ce8a-320">属性</span><span class="sxs-lookup"><span data-stu-id="4ce8a-320">Property</span></span>     | <span data-ttu-id="4ce8a-321">类型</span><span class="sxs-lookup"><span data-stu-id="4ce8a-321">Type</span></span>    |<span data-ttu-id="4ce8a-322">是否必需</span><span class="sxs-lookup"><span data-stu-id="4ce8a-322">Required</span></span>|  <span data-ttu-id="4ce8a-323">值</span><span class="sxs-lookup"><span data-stu-id="4ce8a-323">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="4ce8a-324">resourceId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-324">resourceId</span></span>|<span data-ttu-id="4ce8a-325">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-325">String</span></span>|<span data-ttu-id="4ce8a-326">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-326">Yes</span></span>|<span data-ttu-id="4ce8a-327">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="4ce8a-327">\<resourceId\></span></span>|
|<span data-ttu-id="4ce8a-328">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-328">roleDefinitionId</span></span>|<span data-ttu-id="4ce8a-329">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-329">String</span></span>|<span data-ttu-id="4ce8a-330">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-330">Yes</span></span>|<span data-ttu-id="4ce8a-331">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="4ce8a-331">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="4ce8a-332">subjectId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-332">subjectId</span></span>|<span data-ttu-id="4ce8a-333">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-333">String</span></span>|<span data-ttu-id="4ce8a-334">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-334">Yes</span></span>|<span data-ttu-id="4ce8a-335">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="4ce8a-335">\<subjectId\></span></span>|
|<span data-ttu-id="4ce8a-336">assignmentState</span><span class="sxs-lookup"><span data-stu-id="4ce8a-336">assignmentState</span></span>|<span data-ttu-id="4ce8a-337">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-337">String</span></span>|<span data-ttu-id="4ce8a-338">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-338">Yes</span></span>| <span data-ttu-id="4ce8a-339">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="4ce8a-339">Eligible / Active</span></span>|
|<span data-ttu-id="4ce8a-340">type</span><span class="sxs-lookup"><span data-stu-id="4ce8a-340">type</span></span>|<span data-ttu-id="4ce8a-341">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-341">String</span></span>|<span data-ttu-id="4ce8a-342">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-342">Yes</span></span>| <span data-ttu-id="4ce8a-343">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="4ce8a-343">AdminRemove</span></span>|
|<span data-ttu-id="4ce8a-344">原因</span><span class="sxs-lookup"><span data-stu-id="4ce8a-344">reason</span></span>|<span data-ttu-id="4ce8a-345">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-345">String</span></span>| <span data-ttu-id="4ce8a-346">否</span><span class="sxs-lookup"><span data-stu-id="4ce8a-346">No</span></span>||
|<span data-ttu-id="4ce8a-347">计划</span><span class="sxs-lookup"><span data-stu-id="4ce8a-347">schedule</span></span>|[<span data-ttu-id="4ce8a-348">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4ce8a-348">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="4ce8a-349">否</span><span class="sxs-lookup"><span data-stu-id="4ce8a-349">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="4ce8a-350">请求</span><span class="sxs-lookup"><span data-stu-id="4ce8a-350">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="4ce8a-351">响应</span><span class="sxs-lookup"><span data-stu-id="4ce8a-351">Response</span></span>
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
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```

### <a name="example-5"></a><span data-ttu-id="4ce8a-352">示例 5</span><span class="sxs-lookup"><span data-stu-id="4ce8a-352">Example 5</span></span>
<span data-ttu-id="4ce8a-353">本示例中，管理员向所有者更新用户 nawu@fimdev.net 的角色分配。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-353">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="4ce8a-354">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-354">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="4ce8a-355">属性</span><span class="sxs-lookup"><span data-stu-id="4ce8a-355">Property</span></span>     | <span data-ttu-id="4ce8a-356">类型</span><span class="sxs-lookup"><span data-stu-id="4ce8a-356">Type</span></span>    |<span data-ttu-id="4ce8a-357">是否必需</span><span class="sxs-lookup"><span data-stu-id="4ce8a-357">Required</span></span>|  <span data-ttu-id="4ce8a-358">值</span><span class="sxs-lookup"><span data-stu-id="4ce8a-358">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="4ce8a-359">resourceId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-359">resourceId</span></span>|<span data-ttu-id="4ce8a-360">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-360">String</span></span>|<span data-ttu-id="4ce8a-361">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-361">Yes</span></span>|<span data-ttu-id="4ce8a-362">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="4ce8a-362">\<resourceId\></span></span>|
|<span data-ttu-id="4ce8a-363">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-363">roleDefinitionId</span></span>|<span data-ttu-id="4ce8a-364">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-364">String</span></span>|<span data-ttu-id="4ce8a-365">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-365">Yes</span></span>|<span data-ttu-id="4ce8a-366">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="4ce8a-366">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="4ce8a-367">subjectId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-367">subjectId</span></span>|<span data-ttu-id="4ce8a-368">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-368">String</span></span>|<span data-ttu-id="4ce8a-369">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-369">Yes</span></span>|<span data-ttu-id="4ce8a-370">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="4ce8a-370">\<subjectId\></span></span>|
|<span data-ttu-id="4ce8a-371">assignmentState</span><span class="sxs-lookup"><span data-stu-id="4ce8a-371">assignmentState</span></span>|<span data-ttu-id="4ce8a-372">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-372">String</span></span>|<span data-ttu-id="4ce8a-373">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-373">Yes</span></span>| <span data-ttu-id="4ce8a-374">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="4ce8a-374">Eligible / Active</span></span>|
|<span data-ttu-id="4ce8a-375">type</span><span class="sxs-lookup"><span data-stu-id="4ce8a-375">type</span></span>|<span data-ttu-id="4ce8a-376">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-376">String</span></span>|<span data-ttu-id="4ce8a-377">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-377">Yes</span></span>| <span data-ttu-id="4ce8a-378">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="4ce8a-378">AdminUpdate</span></span>|
|<span data-ttu-id="4ce8a-379">原因</span><span class="sxs-lookup"><span data-stu-id="4ce8a-379">reason</span></span>|<span data-ttu-id="4ce8a-380">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-380">String</span></span>| <span data-ttu-id="4ce8a-381">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="4ce8a-381">depends on roleSettings</span></span>||
|<span data-ttu-id="4ce8a-382">计划</span><span class="sxs-lookup"><span data-stu-id="4ce8a-382">schedule</span></span>|[<span data-ttu-id="4ce8a-383">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4ce8a-383">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="4ce8a-384">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-384">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="4ce8a-385">请求</span><span class="sxs-lookup"><span data-stu-id="4ce8a-385">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="4ce8a-386">响应</span><span class="sxs-lookup"><span data-stu-id="4ce8a-386">Response</span></span>
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

### <a name="example-6"></a><span data-ttu-id="4ce8a-387">示例 6</span><span class="sxs-lookup"><span data-stu-id="4ce8a-387">Example 6</span></span>
<span data-ttu-id="4ce8a-388">本示例将用户 ANUJCUSER 即将过期的角色分配给 API 管理服务参与者。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-388">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="4ce8a-389">**注意：** 另外还包括的权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="4ce8a-389">**Note:** In additon to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="4ce8a-390">属性</span><span class="sxs-lookup"><span data-stu-id="4ce8a-390">Property</span></span>     | <span data-ttu-id="4ce8a-391">类型</span><span class="sxs-lookup"><span data-stu-id="4ce8a-391">Type</span></span>    |<span data-ttu-id="4ce8a-392">是否必需</span><span class="sxs-lookup"><span data-stu-id="4ce8a-392">Required</span></span>|  <span data-ttu-id="4ce8a-393">值</span><span class="sxs-lookup"><span data-stu-id="4ce8a-393">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="4ce8a-394">resourceId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-394">resourceId</span></span>|<span data-ttu-id="4ce8a-395">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-395">String</span></span>|<span data-ttu-id="4ce8a-396">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-396">Yes</span></span>|<span data-ttu-id="4ce8a-397">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="4ce8a-397">\<resourceId\></span></span>|
|<span data-ttu-id="4ce8a-398">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-398">roleDefinitionId</span></span>|<span data-ttu-id="4ce8a-399">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-399">String</span></span>|<span data-ttu-id="4ce8a-400">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-400">Yes</span></span>|<span data-ttu-id="4ce8a-401">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="4ce8a-401">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="4ce8a-402">subjectId</span><span class="sxs-lookup"><span data-stu-id="4ce8a-402">subjectId</span></span>|<span data-ttu-id="4ce8a-403">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-403">String</span></span>|<span data-ttu-id="4ce8a-404">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-404">Yes</span></span>|<span data-ttu-id="4ce8a-405">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="4ce8a-405">\<subjectId\></span></span>|
|<span data-ttu-id="4ce8a-406">assignmentState</span><span class="sxs-lookup"><span data-stu-id="4ce8a-406">assignmentState</span></span>|<span data-ttu-id="4ce8a-407">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-407">String</span></span>|<span data-ttu-id="4ce8a-408">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-408">Yes</span></span>| <span data-ttu-id="4ce8a-409">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="4ce8a-409">Eligible / Active</span></span> |
|<span data-ttu-id="4ce8a-410">type</span><span class="sxs-lookup"><span data-stu-id="4ce8a-410">type</span></span>|<span data-ttu-id="4ce8a-411">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-411">String</span></span>|<span data-ttu-id="4ce8a-412">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-412">Yes</span></span>| <span data-ttu-id="4ce8a-413">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="4ce8a-413">AdminExtend</span></span>|
|<span data-ttu-id="4ce8a-414">原因</span><span class="sxs-lookup"><span data-stu-id="4ce8a-414">reason</span></span>|<span data-ttu-id="4ce8a-415">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce8a-415">String</span></span>| <span data-ttu-id="4ce8a-416">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="4ce8a-416">depends on roleSettings</span></span>||
|<span data-ttu-id="4ce8a-417">计划</span><span class="sxs-lookup"><span data-stu-id="4ce8a-417">schedule</span></span>|[<span data-ttu-id="4ce8a-418">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4ce8a-418">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="4ce8a-419">是</span><span class="sxs-lookup"><span data-stu-id="4ce8a-419">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="4ce8a-420">请求</span><span class="sxs-lookup"><span data-stu-id="4ce8a-420">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="4ce8a-421">响应</span><span class="sxs-lookup"><span data-stu-id="4ce8a-421">Response</span></span>
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
