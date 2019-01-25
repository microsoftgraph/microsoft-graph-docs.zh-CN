---
title: 创建 governanceRoleAssignmentRequest
description: 创建角色分配请求以表示该操作所需角色分配。 下表列出的操作。
localization_priority: Normal
ms.openlocfilehash: c936a6cd0ba061fc1dd3758533781d7270673939
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523237"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="71fb0-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="71fb0-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71fb0-105">创建角色分配请求以表示该操作所需角色分配。</span><span class="sxs-lookup"><span data-stu-id="71fb0-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="71fb0-106">下表列出的操作。</span><span class="sxs-lookup"><span data-stu-id="71fb0-106">The following table lists the operations.</span></span>

| <span data-ttu-id="71fb0-107">Operation</span><span class="sxs-lookup"><span data-stu-id="71fb0-107">Operation</span></span>       | <span data-ttu-id="71fb0-108">类型</span><span class="sxs-lookup"><span data-stu-id="71fb0-108">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="71fb0-109">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="71fb0-109">Assign a role assignment</span></span>| <span data-ttu-id="71fb0-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="71fb0-110">AdminAdd</span></span> |
| <span data-ttu-id="71fb0-111">激活合格的角色分配</span><span class="sxs-lookup"><span data-stu-id="71fb0-111">Activate an eligible role assignment</span></span>| <span data-ttu-id="71fb0-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="71fb0-112">UserAdd</span></span> | 
| <span data-ttu-id="71fb0-113">停用已激活的角色分配</span><span class="sxs-lookup"><span data-stu-id="71fb0-113">Deactivate an activated role assignment</span></span>| <span data-ttu-id="71fb0-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="71fb0-114">UserRemove</span></span> | 
| <span data-ttu-id="71fb0-115">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="71fb0-115">Remove a role assignment</span></span>| <span data-ttu-id="71fb0-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="71fb0-116">AdminRemove</span></span> |
| <span data-ttu-id="71fb0-117">更新一个角色分配</span><span class="sxs-lookup"><span data-stu-id="71fb0-117">Update a role assignment</span></span>| <span data-ttu-id="71fb0-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="71fb0-118">AdminUpdate</span></span> |
| <span data-ttu-id="71fb0-119">请求扩展我角色分配</span><span class="sxs-lookup"><span data-stu-id="71fb0-119">Request to extend my role assignment</span></span>| <span data-ttu-id="71fb0-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="71fb0-120">UserExtend</span></span> | 
| <span data-ttu-id="71fb0-121">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="71fb0-121">Extend a role assignment</span></span>| <span data-ttu-id="71fb0-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="71fb0-122">AdminExtend</span></span> | 
| <span data-ttu-id="71fb0-123">请求续订我过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="71fb0-123">Request to renew my expired role assignment</span></span>| <span data-ttu-id="71fb0-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="71fb0-124">UserRenew</span></span> | 
| <span data-ttu-id="71fb0-125">续订已过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="71fb0-125">Renew an expired role assignment</span></span>| <span data-ttu-id="71fb0-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="71fb0-126">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="71fb0-127">权限</span><span class="sxs-lookup"><span data-stu-id="71fb0-127">Permissions</span></span>
<span data-ttu-id="71fb0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71fb0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71fb0-130">权限类型</span><span class="sxs-lookup"><span data-stu-id="71fb0-130">Permission type</span></span>      | <span data-ttu-id="71fb0-131">权限</span><span class="sxs-lookup"><span data-stu-id="71fb0-131">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71fb0-132">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71fb0-132">Delegated (work or school account)</span></span> | <span data-ttu-id="71fb0-133">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="71fb0-133">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="71fb0-134">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71fb0-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71fb0-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="71fb0-135">Not supported.</span></span>    |
|<span data-ttu-id="71fb0-136">应用程序</span><span class="sxs-lookup"><span data-stu-id="71fb0-136">Application</span></span> | <span data-ttu-id="71fb0-137">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="71fb0-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="71fb0-138">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71fb0-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="71fb0-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="71fb0-139">Request headers</span></span>
| <span data-ttu-id="71fb0-140">名称</span><span class="sxs-lookup"><span data-stu-id="71fb0-140">Name</span></span>       | <span data-ttu-id="71fb0-141">说明</span><span class="sxs-lookup"><span data-stu-id="71fb0-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="71fb0-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="71fb0-142">Authorization</span></span>  | <span data-ttu-id="71fb0-143">持有者 {code}</span><span class="sxs-lookup"><span data-stu-id="71fb0-143">Bearer {code}</span></span>|
| <span data-ttu-id="71fb0-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="71fb0-144">Content-type</span></span>  | <span data-ttu-id="71fb0-145">application/json</span><span class="sxs-lookup"><span data-stu-id="71fb0-145">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71fb0-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="71fb0-146">Request body</span></span>
<span data-ttu-id="71fb0-147">在请求正文中，提供[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71fb0-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="71fb0-148">属性</span><span class="sxs-lookup"><span data-stu-id="71fb0-148">Property</span></span>     | <span data-ttu-id="71fb0-149">类型</span><span class="sxs-lookup"><span data-stu-id="71fb0-149">Type</span></span>    |<span data-ttu-id="71fb0-150">必需</span><span class="sxs-lookup"><span data-stu-id="71fb0-150">Required</span></span>|  <span data-ttu-id="71fb0-151">说明</span><span class="sxs-lookup"><span data-stu-id="71fb0-151">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="71fb0-152">resourceId</span><span class="sxs-lookup"><span data-stu-id="71fb0-152">resourceId</span></span>|<span data-ttu-id="71fb0-153">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-153">String</span></span>|<span data-ttu-id="71fb0-154">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-154">Yes</span></span>|<span data-ttu-id="71fb0-155">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="71fb0-155">The ID of the resource.</span></span>|
|<span data-ttu-id="71fb0-156">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="71fb0-156">roleDefinitionId</span></span>|<span data-ttu-id="71fb0-157">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-157">String</span></span>|<span data-ttu-id="71fb0-158">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-158">Yes</span></span>|<span data-ttu-id="71fb0-159">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="71fb0-159">The ID of the role definition.</span></span>|
|<span data-ttu-id="71fb0-160">subjectId</span><span class="sxs-lookup"><span data-stu-id="71fb0-160">subjectId</span></span>|<span data-ttu-id="71fb0-161">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-161">String</span></span>|<span data-ttu-id="71fb0-162">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-162">Yes</span></span>|<span data-ttu-id="71fb0-163">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="71fb0-163">The ID of the subject.</span></span>|
|<span data-ttu-id="71fb0-164">assignmentState</span><span class="sxs-lookup"><span data-stu-id="71fb0-164">assignmentState</span></span>|<span data-ttu-id="71fb0-165">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-165">String</span></span>|<span data-ttu-id="71fb0-166">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-166">Yes</span></span>|<span data-ttu-id="71fb0-167">工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="71fb0-167">The state of assignment.</span></span> <span data-ttu-id="71fb0-168">值可以是``Eligible``和``Active``。</span><span class="sxs-lookup"><span data-stu-id="71fb0-168">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="71fb0-169">type</span><span class="sxs-lookup"><span data-stu-id="71fb0-169">type</span></span>|<span data-ttu-id="71fb0-170">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-170">String</span></span>|<span data-ttu-id="71fb0-171">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-171">Yes</span></span>|<span data-ttu-id="71fb0-172">请求类型。</span><span class="sxs-lookup"><span data-stu-id="71fb0-172">The request type.</span></span> <span data-ttu-id="71fb0-173">值可以是`AdminAdd`， `UserAdd`， `AdminUpdate`， `AdminRemove`， `UserRemove`， `UserExtend`， `UserRenew`，`AdminRenew`和`AdminExtend`。</span><span class="sxs-lookup"><span data-stu-id="71fb0-173">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="71fb0-174">Reason</span><span class="sxs-lookup"><span data-stu-id="71fb0-174">reason</span></span>|<span data-ttu-id="71fb0-175">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-175">String</span></span>| |<span data-ttu-id="71fb0-176">原因需要提供角色分配请求的审核和查看用途。</span><span class="sxs-lookup"><span data-stu-id="71fb0-176">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="71fb0-177">Schedule</span><span class="sxs-lookup"><span data-stu-id="71fb0-177">schedule</span></span>|[<span data-ttu-id="71fb0-178">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="71fb0-178">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="71fb0-179">角色分配请求的时间表。</span><span class="sxs-lookup"><span data-stu-id="71fb0-179">The schedule of the role assignment request.</span></span> <span data-ttu-id="71fb0-180">请求类型的`UserAdd`， `AdminAdd`， `AdminUpdate`，和`AdminExtend`，需要。</span><span class="sxs-lookup"><span data-stu-id="71fb0-180">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

## <a name="response"></a><span data-ttu-id="71fb0-181">响应</span><span class="sxs-lookup"><span data-stu-id="71fb0-181">Response</span></span>
<span data-ttu-id="71fb0-182">如果成功，此方法返回`201 Created`响应代码和响应正文中的[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="71fb0-182">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="71fb0-183">错误代码</span><span class="sxs-lookup"><span data-stu-id="71fb0-183">Error codes</span></span>
<span data-ttu-id="71fb0-184">此 API 返回的标准 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="71fb0-184">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="71fb0-185">此外，它也会返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="71fb0-185">In addition, it also returns the error codes listed in the following table.</span></span>

|<span data-ttu-id="71fb0-186">错误代码</span><span class="sxs-lookup"><span data-stu-id="71fb0-186">Error code</span></span>     | <span data-ttu-id="71fb0-187">错误消息</span><span class="sxs-lookup"><span data-stu-id="71fb0-187">Error message</span></span>              | <span data-ttu-id="71fb0-188">详细信息</span><span class="sxs-lookup"><span data-stu-id="71fb0-188">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="71fb0-189">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="71fb0-189">400 BadRequest</span></span> | <span data-ttu-id="71fb0-190">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="71fb0-190">RoleNotFound</span></span>    | <span data-ttu-id="71fb0-191">`roleDefinitionId`提供在请求正文找不到。</span><span class="sxs-lookup"><span data-stu-id="71fb0-191">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="71fb0-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="71fb0-192">400 BadRequest</span></span> | <span data-ttu-id="71fb0-193">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="71fb0-193">ResourceIsLocked</span></span>    | <span data-ttu-id="71fb0-194">在请求正文中提供的资源处于状态的`Locked`和无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="71fb0-194">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="71fb0-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="71fb0-195">400 BadRequest</span></span> | <span data-ttu-id="71fb0-196">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="71fb0-196">SubjectNotFound</span></span>    | <span data-ttu-id="71fb0-197">`subjectId`提供在请求正文找不到。</span><span class="sxs-lookup"><span data-stu-id="71fb0-197">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="71fb0-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="71fb0-198">400 BadRequest</span></span> | <span data-ttu-id="71fb0-199">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="71fb0-199">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="71fb0-200">已存在挂起[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)系统中。</span><span class="sxs-lookup"><span data-stu-id="71fb0-200">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="71fb0-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="71fb0-201">400 BadRequest</span></span> | <span data-ttu-id="71fb0-202">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="71fb0-202">RoleAssignmentExists</span></span>    | <span data-ttu-id="71fb0-203">系统中存在[governanceRoleAssignment](../resources/governanceroleassignment.md)请求已创建。</span><span class="sxs-lookup"><span data-stu-id="71fb0-203">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="71fb0-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="71fb0-204">400 BadRequest</span></span> | <span data-ttu-id="71fb0-205">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="71fb0-205">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="71fb0-206">系统中不存在[governanceRoleAssignment](../resources/governanceroleassignment.md)请求来更新/扩展。</span><span class="sxs-lookup"><span data-stu-id="71fb0-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="71fb0-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="71fb0-207">400 BadRequest</span></span> | <span data-ttu-id="71fb0-208">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="71fb0-208">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="71fb0-209">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部的策略，且无法创建。</span><span class="sxs-lookup"><span data-stu-id="71fb0-209">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="examples"></a><span data-ttu-id="71fb0-210">示例</span><span class="sxs-lookup"><span data-stu-id="71fb0-210">Examples</span></span>
<span data-ttu-id="71fb0-211">下面的示例演示如何使用此 API。</span><span class="sxs-lookup"><span data-stu-id="71fb0-211">The following examples show how to use this API.</span></span>

### <a name="example-1"></a><span data-ttu-id="71fb0-212">示例 1</span><span class="sxs-lookup"><span data-stu-id="71fb0-212">Example 1</span></span>
<span data-ttu-id="71fb0-213">本示例中，管理员为帐单读者角色分配用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="71fb0-213">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="71fb0-214">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="71fb0-214">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="71fb0-215">属性</span><span class="sxs-lookup"><span data-stu-id="71fb0-215">Property</span></span>     | <span data-ttu-id="71fb0-216">类型</span><span class="sxs-lookup"><span data-stu-id="71fb0-216">Type</span></span>    |<span data-ttu-id="71fb0-217">是否必需</span><span class="sxs-lookup"><span data-stu-id="71fb0-217">Required</span></span>|  <span data-ttu-id="71fb0-218">值</span><span class="sxs-lookup"><span data-stu-id="71fb0-218">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="71fb0-219">resourceId</span><span class="sxs-lookup"><span data-stu-id="71fb0-219">resourceId</span></span>|<span data-ttu-id="71fb0-220">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-220">String</span></span>|<span data-ttu-id="71fb0-221">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-221">Yes</span></span>|<span data-ttu-id="71fb0-222">\<</span><span class="sxs-lookup"><span data-stu-id="71fb0-222">\<resourceId\></span></span>|
|<span data-ttu-id="71fb0-223">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="71fb0-223">roleDefinitionId</span></span>|<span data-ttu-id="71fb0-224">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-224">String</span></span>|<span data-ttu-id="71fb0-225">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-225">Yes</span></span>|<span data-ttu-id="71fb0-226">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="71fb0-226">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="71fb0-227">subjectId</span><span class="sxs-lookup"><span data-stu-id="71fb0-227">subjectId</span></span>|<span data-ttu-id="71fb0-228">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-228">String</span></span>|<span data-ttu-id="71fb0-229">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-229">Yes</span></span>|<span data-ttu-id="71fb0-230">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="71fb0-230">\<subjectId\></span></span>|
|<span data-ttu-id="71fb0-231">assignmentState</span><span class="sxs-lookup"><span data-stu-id="71fb0-231">assignmentState</span></span>|<span data-ttu-id="71fb0-232">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-232">String</span></span>|<span data-ttu-id="71fb0-233">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-233">Yes</span></span>| <span data-ttu-id="71fb0-234">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="71fb0-234">Eligible / Active</span></span>|
|<span data-ttu-id="71fb0-235">type</span><span class="sxs-lookup"><span data-stu-id="71fb0-235">type</span></span>|<span data-ttu-id="71fb0-236">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-236">String</span></span>|<span data-ttu-id="71fb0-237">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-237">Yes</span></span>| <span data-ttu-id="71fb0-238">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="71fb0-238">AdminAdd</span></span>|
|<span data-ttu-id="71fb0-239">Reason</span><span class="sxs-lookup"><span data-stu-id="71fb0-239">reason</span></span>|<span data-ttu-id="71fb0-240">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-240">String</span></span>| <span data-ttu-id="71fb0-241">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="71fb0-241">depends on role Settings</span></span>||
|<span data-ttu-id="71fb0-242">Schedule</span><span class="sxs-lookup"><span data-stu-id="71fb0-242">schedule</span></span>|[<span data-ttu-id="71fb0-243">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="71fb0-243">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="71fb0-244">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-244">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="71fb0-245">请求</span><span class="sxs-lookup"><span data-stu-id="71fb0-245">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="71fb0-246">响应</span><span class="sxs-lookup"><span data-stu-id="71fb0-246">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="71fb0-247">示例 2</span><span class="sxs-lookup"><span data-stu-id="71fb0-247">Example 2</span></span>
<span data-ttu-id="71fb0-248">本示例中，用户 nawu@fimdev.net 激活合格的帐单读取器角色。</span><span class="sxs-lookup"><span data-stu-id="71fb0-248">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="71fb0-249">属性</span><span class="sxs-lookup"><span data-stu-id="71fb0-249">Property</span></span>     | <span data-ttu-id="71fb0-250">类型</span><span class="sxs-lookup"><span data-stu-id="71fb0-250">Type</span></span>    |<span data-ttu-id="71fb0-251">是否必需</span><span class="sxs-lookup"><span data-stu-id="71fb0-251">Required</span></span>|  <span data-ttu-id="71fb0-252">值</span><span class="sxs-lookup"><span data-stu-id="71fb0-252">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="71fb0-253">resourceId</span><span class="sxs-lookup"><span data-stu-id="71fb0-253">resourceId</span></span>|<span data-ttu-id="71fb0-254">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-254">String</span></span>|<span data-ttu-id="71fb0-255">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-255">Yes</span></span>|<span data-ttu-id="71fb0-256">\<</span><span class="sxs-lookup"><span data-stu-id="71fb0-256">\<resourceId\></span></span>|
|<span data-ttu-id="71fb0-257">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="71fb0-257">roleDefinitionId</span></span>|<span data-ttu-id="71fb0-258">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-258">String</span></span>|<span data-ttu-id="71fb0-259">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-259">Yes</span></span>|<span data-ttu-id="71fb0-260">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="71fb0-260">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="71fb0-261">subjectId</span><span class="sxs-lookup"><span data-stu-id="71fb0-261">subjectId</span></span>|<span data-ttu-id="71fb0-262">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-262">String</span></span>|<span data-ttu-id="71fb0-263">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-263">Yes</span></span>|<span data-ttu-id="71fb0-264">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="71fb0-264">\<subjectId\></span></span>|
|<span data-ttu-id="71fb0-265">assignmentState</span><span class="sxs-lookup"><span data-stu-id="71fb0-265">assignmentState</span></span>|<span data-ttu-id="71fb0-266">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-266">String</span></span>|<span data-ttu-id="71fb0-267">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-267">Yes</span></span>| <span data-ttu-id="71fb0-268">活动</span><span class="sxs-lookup"><span data-stu-id="71fb0-268">Active</span></span>|
|<span data-ttu-id="71fb0-269">type</span><span class="sxs-lookup"><span data-stu-id="71fb0-269">type</span></span>|<span data-ttu-id="71fb0-270">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-270">String</span></span>|<span data-ttu-id="71fb0-271">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-271">Yes</span></span>| <span data-ttu-id="71fb0-272">UserAdd</span><span class="sxs-lookup"><span data-stu-id="71fb0-272">UserAdd</span></span>|
|<span data-ttu-id="71fb0-273">Reason</span><span class="sxs-lookup"><span data-stu-id="71fb0-273">reason</span></span>|<span data-ttu-id="71fb0-274">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-274">String</span></span>| <span data-ttu-id="71fb0-275">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="71fb0-275">depends on role Settings</span></span>||
|<span data-ttu-id="71fb0-276">Schedule</span><span class="sxs-lookup"><span data-stu-id="71fb0-276">schedule</span></span>|[<span data-ttu-id="71fb0-277">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="71fb0-277">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="71fb0-278">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-278">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="71fb0-279">请求</span><span class="sxs-lookup"><span data-stu-id="71fb0-279">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="71fb0-280">响应</span><span class="sxs-lookup"><span data-stu-id="71fb0-280">Response</span></span>
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

### <a name="example-3"></a><span data-ttu-id="71fb0-281">示例 3</span><span class="sxs-lookup"><span data-stu-id="71fb0-281">Example 3</span></span>
<span data-ttu-id="71fb0-282">本示例中，用户 nawu@fimdev.net 停用活动的帐单读取器角色。</span><span class="sxs-lookup"><span data-stu-id="71fb0-282">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="71fb0-283">属性</span><span class="sxs-lookup"><span data-stu-id="71fb0-283">Property</span></span>     | <span data-ttu-id="71fb0-284">类型</span><span class="sxs-lookup"><span data-stu-id="71fb0-284">Type</span></span>    |<span data-ttu-id="71fb0-285">是否必需</span><span class="sxs-lookup"><span data-stu-id="71fb0-285">Required</span></span>|  <span data-ttu-id="71fb0-286">值</span><span class="sxs-lookup"><span data-stu-id="71fb0-286">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="71fb0-287">resourceId</span><span class="sxs-lookup"><span data-stu-id="71fb0-287">resourceId</span></span>|<span data-ttu-id="71fb0-288">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-288">String</span></span>|<span data-ttu-id="71fb0-289">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-289">Yes</span></span>|<span data-ttu-id="71fb0-290">\<</span><span class="sxs-lookup"><span data-stu-id="71fb0-290">\<resourceId\></span></span>|
|<span data-ttu-id="71fb0-291">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="71fb0-291">roleDefinitionId</span></span>|<span data-ttu-id="71fb0-292">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-292">String</span></span>|<span data-ttu-id="71fb0-293">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-293">Yes</span></span>|<span data-ttu-id="71fb0-294">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="71fb0-294">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="71fb0-295">subjectId</span><span class="sxs-lookup"><span data-stu-id="71fb0-295">subjectId</span></span>|<span data-ttu-id="71fb0-296">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-296">String</span></span>|<span data-ttu-id="71fb0-297">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-297">Yes</span></span>|<span data-ttu-id="71fb0-298">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="71fb0-298">\<subjectId\></span></span>|
|<span data-ttu-id="71fb0-299">assignmentState</span><span class="sxs-lookup"><span data-stu-id="71fb0-299">assignmentState</span></span>|<span data-ttu-id="71fb0-300">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-300">String</span></span>|<span data-ttu-id="71fb0-301">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-301">Yes</span></span>| <span data-ttu-id="71fb0-302">活动</span><span class="sxs-lookup"><span data-stu-id="71fb0-302">Active</span></span>|
|<span data-ttu-id="71fb0-303">type</span><span class="sxs-lookup"><span data-stu-id="71fb0-303">type</span></span>|<span data-ttu-id="71fb0-304">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-304">String</span></span>|<span data-ttu-id="71fb0-305">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-305">Yes</span></span>| <span data-ttu-id="71fb0-306">UserRemove</span><span class="sxs-lookup"><span data-stu-id="71fb0-306">UserRemove</span></span>|
|<span data-ttu-id="71fb0-307">Reason</span><span class="sxs-lookup"><span data-stu-id="71fb0-307">reason</span></span>|<span data-ttu-id="71fb0-308">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-308">String</span></span>| <span data-ttu-id="71fb0-309">否</span><span class="sxs-lookup"><span data-stu-id="71fb0-309">No</span></span>||
|<span data-ttu-id="71fb0-310">Schedule</span><span class="sxs-lookup"><span data-stu-id="71fb0-310">schedule</span></span>|[<span data-ttu-id="71fb0-311">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="71fb0-311">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="71fb0-312">否</span><span class="sxs-lookup"><span data-stu-id="71fb0-312">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="71fb0-313">请求</span><span class="sxs-lookup"><span data-stu-id="71fb0-313">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="71fb0-314">响应</span><span class="sxs-lookup"><span data-stu-id="71fb0-314">Response</span></span>
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

### <a name="example-4"></a><span data-ttu-id="71fb0-315">示例 4</span><span class="sxs-lookup"><span data-stu-id="71fb0-315">Example 4</span></span>
<span data-ttu-id="71fb0-316">本示例中，管理员从帐单读者角色中移除用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="71fb0-316">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="71fb0-317">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="71fb0-317">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="71fb0-318">属性</span><span class="sxs-lookup"><span data-stu-id="71fb0-318">Property</span></span>     | <span data-ttu-id="71fb0-319">类型</span><span class="sxs-lookup"><span data-stu-id="71fb0-319">Type</span></span>    |<span data-ttu-id="71fb0-320">是否必需</span><span class="sxs-lookup"><span data-stu-id="71fb0-320">Required</span></span>|  <span data-ttu-id="71fb0-321">值</span><span class="sxs-lookup"><span data-stu-id="71fb0-321">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="71fb0-322">resourceId</span><span class="sxs-lookup"><span data-stu-id="71fb0-322">resourceId</span></span>|<span data-ttu-id="71fb0-323">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-323">String</span></span>|<span data-ttu-id="71fb0-324">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-324">Yes</span></span>|<span data-ttu-id="71fb0-325">\<</span><span class="sxs-lookup"><span data-stu-id="71fb0-325">\<resourceId\></span></span>|
|<span data-ttu-id="71fb0-326">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="71fb0-326">roleDefinitionId</span></span>|<span data-ttu-id="71fb0-327">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-327">String</span></span>|<span data-ttu-id="71fb0-328">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-328">Yes</span></span>|<span data-ttu-id="71fb0-329">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="71fb0-329">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="71fb0-330">subjectId</span><span class="sxs-lookup"><span data-stu-id="71fb0-330">subjectId</span></span>|<span data-ttu-id="71fb0-331">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-331">String</span></span>|<span data-ttu-id="71fb0-332">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-332">Yes</span></span>|<span data-ttu-id="71fb0-333">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="71fb0-333">\<subjectId\></span></span>|
|<span data-ttu-id="71fb0-334">assignmentState</span><span class="sxs-lookup"><span data-stu-id="71fb0-334">assignmentState</span></span>|<span data-ttu-id="71fb0-335">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-335">String</span></span>|<span data-ttu-id="71fb0-336">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-336">Yes</span></span>| <span data-ttu-id="71fb0-337">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="71fb0-337">Eligible / Active</span></span>|
|<span data-ttu-id="71fb0-338">type</span><span class="sxs-lookup"><span data-stu-id="71fb0-338">type</span></span>|<span data-ttu-id="71fb0-339">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-339">String</span></span>|<span data-ttu-id="71fb0-340">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-340">Yes</span></span>| <span data-ttu-id="71fb0-341">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="71fb0-341">AdminRemove</span></span>|
|<span data-ttu-id="71fb0-342">Reason</span><span class="sxs-lookup"><span data-stu-id="71fb0-342">reason</span></span>|<span data-ttu-id="71fb0-343">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-343">String</span></span>| <span data-ttu-id="71fb0-344">否</span><span class="sxs-lookup"><span data-stu-id="71fb0-344">No</span></span>||
|<span data-ttu-id="71fb0-345">Schedule</span><span class="sxs-lookup"><span data-stu-id="71fb0-345">schedule</span></span>|[<span data-ttu-id="71fb0-346">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="71fb0-346">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="71fb0-347">否</span><span class="sxs-lookup"><span data-stu-id="71fb0-347">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="71fb0-348">请求</span><span class="sxs-lookup"><span data-stu-id="71fb0-348">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="71fb0-349">响应</span><span class="sxs-lookup"><span data-stu-id="71fb0-349">Response</span></span>
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

### <a name="example-5"></a><span data-ttu-id="71fb0-350">示例 5</span><span class="sxs-lookup"><span data-stu-id="71fb0-350">Example 5</span></span>
<span data-ttu-id="71fb0-351">本示例中，管理员向所有者更新用户 nawu@fimdev.net 的角色分配。</span><span class="sxs-lookup"><span data-stu-id="71fb0-351">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="71fb0-352">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="71fb0-352">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="71fb0-353">属性</span><span class="sxs-lookup"><span data-stu-id="71fb0-353">Property</span></span>     | <span data-ttu-id="71fb0-354">类型</span><span class="sxs-lookup"><span data-stu-id="71fb0-354">Type</span></span>    |<span data-ttu-id="71fb0-355">是否必需</span><span class="sxs-lookup"><span data-stu-id="71fb0-355">Required</span></span>|  <span data-ttu-id="71fb0-356">值</span><span class="sxs-lookup"><span data-stu-id="71fb0-356">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="71fb0-357">resourceId</span><span class="sxs-lookup"><span data-stu-id="71fb0-357">resourceId</span></span>|<span data-ttu-id="71fb0-358">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-358">String</span></span>|<span data-ttu-id="71fb0-359">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-359">Yes</span></span>|<span data-ttu-id="71fb0-360">\<</span><span class="sxs-lookup"><span data-stu-id="71fb0-360">\<resourceId\></span></span>|
|<span data-ttu-id="71fb0-361">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="71fb0-361">roleDefinitionId</span></span>|<span data-ttu-id="71fb0-362">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-362">String</span></span>|<span data-ttu-id="71fb0-363">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-363">Yes</span></span>|<span data-ttu-id="71fb0-364">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="71fb0-364">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="71fb0-365">subjectId</span><span class="sxs-lookup"><span data-stu-id="71fb0-365">subjectId</span></span>|<span data-ttu-id="71fb0-366">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-366">String</span></span>|<span data-ttu-id="71fb0-367">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-367">Yes</span></span>|<span data-ttu-id="71fb0-368">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="71fb0-368">\<subjectId\></span></span>|
|<span data-ttu-id="71fb0-369">assignmentState</span><span class="sxs-lookup"><span data-stu-id="71fb0-369">assignmentState</span></span>|<span data-ttu-id="71fb0-370">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-370">String</span></span>|<span data-ttu-id="71fb0-371">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-371">Yes</span></span>| <span data-ttu-id="71fb0-372">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="71fb0-372">Eligible / Active</span></span>|
|<span data-ttu-id="71fb0-373">type</span><span class="sxs-lookup"><span data-stu-id="71fb0-373">type</span></span>|<span data-ttu-id="71fb0-374">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-374">String</span></span>|<span data-ttu-id="71fb0-375">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-375">Yes</span></span>| <span data-ttu-id="71fb0-376">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="71fb0-376">AdminUpdate</span></span>|
|<span data-ttu-id="71fb0-377">Reason</span><span class="sxs-lookup"><span data-stu-id="71fb0-377">reason</span></span>|<span data-ttu-id="71fb0-378">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-378">String</span></span>| <span data-ttu-id="71fb0-379">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="71fb0-379">depends on roleSettings</span></span>||
|<span data-ttu-id="71fb0-380">Schedule</span><span class="sxs-lookup"><span data-stu-id="71fb0-380">schedule</span></span>|[<span data-ttu-id="71fb0-381">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="71fb0-381">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="71fb0-382">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-382">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="71fb0-383">请求</span><span class="sxs-lookup"><span data-stu-id="71fb0-383">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="71fb0-384">响应</span><span class="sxs-lookup"><span data-stu-id="71fb0-384">Response</span></span>
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

### <a name="example-6"></a><span data-ttu-id="71fb0-385">示例 6</span><span class="sxs-lookup"><span data-stu-id="71fb0-385">Example 6</span></span>
<span data-ttu-id="71fb0-386">本示例将用户 ANUJCUSER 即将过期的角色分配给 API 管理服务参与者。</span><span class="sxs-lookup"><span data-stu-id="71fb0-386">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="71fb0-387">**注意：** 另外还包括的权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="71fb0-387">**Note:** In additon to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="71fb0-388">属性</span><span class="sxs-lookup"><span data-stu-id="71fb0-388">Property</span></span>     | <span data-ttu-id="71fb0-389">类型</span><span class="sxs-lookup"><span data-stu-id="71fb0-389">Type</span></span>    |<span data-ttu-id="71fb0-390">是否必需</span><span class="sxs-lookup"><span data-stu-id="71fb0-390">Required</span></span>|  <span data-ttu-id="71fb0-391">值</span><span class="sxs-lookup"><span data-stu-id="71fb0-391">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="71fb0-392">resourceId</span><span class="sxs-lookup"><span data-stu-id="71fb0-392">resourceId</span></span>|<span data-ttu-id="71fb0-393">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-393">String</span></span>|<span data-ttu-id="71fb0-394">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-394">Yes</span></span>|<span data-ttu-id="71fb0-395">\<</span><span class="sxs-lookup"><span data-stu-id="71fb0-395">\<resourceId\></span></span>|
|<span data-ttu-id="71fb0-396">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="71fb0-396">roleDefinitionId</span></span>|<span data-ttu-id="71fb0-397">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-397">String</span></span>|<span data-ttu-id="71fb0-398">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-398">Yes</span></span>|<span data-ttu-id="71fb0-399">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="71fb0-399">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="71fb0-400">subjectId</span><span class="sxs-lookup"><span data-stu-id="71fb0-400">subjectId</span></span>|<span data-ttu-id="71fb0-401">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-401">String</span></span>|<span data-ttu-id="71fb0-402">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-402">Yes</span></span>|<span data-ttu-id="71fb0-403">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="71fb0-403">\<subjectId\></span></span>|
|<span data-ttu-id="71fb0-404">assignmentState</span><span class="sxs-lookup"><span data-stu-id="71fb0-404">assignmentState</span></span>|<span data-ttu-id="71fb0-405">字符串</span><span class="sxs-lookup"><span data-stu-id="71fb0-405">String</span></span>|<span data-ttu-id="71fb0-406">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-406">Yes</span></span>| <span data-ttu-id="71fb0-407">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="71fb0-407">Eligible / Active</span></span> |
|<span data-ttu-id="71fb0-408">type</span><span class="sxs-lookup"><span data-stu-id="71fb0-408">type</span></span>|<span data-ttu-id="71fb0-409">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-409">String</span></span>|<span data-ttu-id="71fb0-410">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-410">Yes</span></span>| <span data-ttu-id="71fb0-411">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="71fb0-411">AdminExtend</span></span>|
|<span data-ttu-id="71fb0-412">Reason</span><span class="sxs-lookup"><span data-stu-id="71fb0-412">reason</span></span>|<span data-ttu-id="71fb0-413">String</span><span class="sxs-lookup"><span data-stu-id="71fb0-413">String</span></span>| <span data-ttu-id="71fb0-414">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="71fb0-414">depends on roleSettings</span></span>||
|<span data-ttu-id="71fb0-415">Schedule</span><span class="sxs-lookup"><span data-stu-id="71fb0-415">schedule</span></span>|[<span data-ttu-id="71fb0-416">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="71fb0-416">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="71fb0-417">是</span><span class="sxs-lookup"><span data-stu-id="71fb0-417">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="71fb0-418">请求</span><span class="sxs-lookup"><span data-stu-id="71fb0-418">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="71fb0-419">响应</span><span class="sxs-lookup"><span data-stu-id="71fb0-419">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
