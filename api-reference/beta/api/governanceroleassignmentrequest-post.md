---
title: 创建 governanceRoleAssignmentRequest
description: 创建角色分配请求以表示该操作所需角色分配。 下表列出的操作。
localization_priority: Normal
ms.openlocfilehash: 0fc8d96585daf63f53bc6b33985a289e8f810d6b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572365"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="018f6-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="018f6-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="018f6-105">创建角色分配请求以表示该操作所需角色分配。</span><span class="sxs-lookup"><span data-stu-id="018f6-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="018f6-106">下表列出的操作。</span><span class="sxs-lookup"><span data-stu-id="018f6-106">The following table lists the operations.</span></span>

| <span data-ttu-id="018f6-107">操作</span><span class="sxs-lookup"><span data-stu-id="018f6-107">Operation</span></span>       | <span data-ttu-id="018f6-108">类型</span><span class="sxs-lookup"><span data-stu-id="018f6-108">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="018f6-109">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="018f6-109">Assign a role assignment</span></span>| <span data-ttu-id="018f6-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="018f6-110">AdminAdd</span></span> |
| <span data-ttu-id="018f6-111">激活合格的角色分配</span><span class="sxs-lookup"><span data-stu-id="018f6-111">Activate an eligible role assignment</span></span>| <span data-ttu-id="018f6-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="018f6-112">UserAdd</span></span> | 
| <span data-ttu-id="018f6-113">停用已激活的角色分配</span><span class="sxs-lookup"><span data-stu-id="018f6-113">Deactivate an activated role assignment</span></span>| <span data-ttu-id="018f6-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="018f6-114">UserRemove</span></span> | 
| <span data-ttu-id="018f6-115">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="018f6-115">Remove a role assignment</span></span>| <span data-ttu-id="018f6-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="018f6-116">AdminRemove</span></span> |
| <span data-ttu-id="018f6-117">更新一个角色分配</span><span class="sxs-lookup"><span data-stu-id="018f6-117">Update a role assignment</span></span>| <span data-ttu-id="018f6-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="018f6-118">AdminUpdate</span></span> |
| <span data-ttu-id="018f6-119">请求扩展我角色分配</span><span class="sxs-lookup"><span data-stu-id="018f6-119">Request to extend my role assignment</span></span>| <span data-ttu-id="018f6-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="018f6-120">UserExtend</span></span> | 
| <span data-ttu-id="018f6-121">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="018f6-121">Extend a role assignment</span></span>| <span data-ttu-id="018f6-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="018f6-122">AdminExtend</span></span> | 
| <span data-ttu-id="018f6-123">请求续订我过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="018f6-123">Request to renew my expired role assignment</span></span>| <span data-ttu-id="018f6-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="018f6-124">UserRenew</span></span> | 
| <span data-ttu-id="018f6-125">续订已过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="018f6-125">Renew an expired role assignment</span></span>| <span data-ttu-id="018f6-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="018f6-126">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="018f6-127">权限</span><span class="sxs-lookup"><span data-stu-id="018f6-127">Permissions</span></span>
<span data-ttu-id="018f6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="018f6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="018f6-130">权限类型</span><span class="sxs-lookup"><span data-stu-id="018f6-130">Permission type</span></span>      | <span data-ttu-id="018f6-131">权限</span><span class="sxs-lookup"><span data-stu-id="018f6-131">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="018f6-132">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="018f6-132">Delegated (work or school account)</span></span> | <span data-ttu-id="018f6-133">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="018f6-133">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="018f6-134">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="018f6-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="018f6-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="018f6-135">Not supported.</span></span>    |
|<span data-ttu-id="018f6-136">应用程序</span><span class="sxs-lookup"><span data-stu-id="018f6-136">Application</span></span> | <span data-ttu-id="018f6-137">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="018f6-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="018f6-138">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="018f6-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="018f6-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="018f6-139">Request headers</span></span>
| <span data-ttu-id="018f6-140">名称</span><span class="sxs-lookup"><span data-stu-id="018f6-140">Name</span></span>       | <span data-ttu-id="018f6-141">说明</span><span class="sxs-lookup"><span data-stu-id="018f6-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="018f6-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="018f6-142">Authorization</span></span>  | <span data-ttu-id="018f6-143">持有者 {code}</span><span class="sxs-lookup"><span data-stu-id="018f6-143">Bearer {code}</span></span>|
| <span data-ttu-id="018f6-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="018f6-144">Content-type</span></span>  | <span data-ttu-id="018f6-145">application/json</span><span class="sxs-lookup"><span data-stu-id="018f6-145">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="018f6-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="018f6-146">Request body</span></span>
<span data-ttu-id="018f6-147">在请求正文中，提供[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="018f6-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="018f6-148">属性</span><span class="sxs-lookup"><span data-stu-id="018f6-148">Property</span></span>     | <span data-ttu-id="018f6-149">类型</span><span class="sxs-lookup"><span data-stu-id="018f6-149">Type</span></span>    |<span data-ttu-id="018f6-150">必需</span><span class="sxs-lookup"><span data-stu-id="018f6-150">Required</span></span>|  <span data-ttu-id="018f6-151">说明</span><span class="sxs-lookup"><span data-stu-id="018f6-151">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="018f6-152">resourceId</span><span class="sxs-lookup"><span data-stu-id="018f6-152">resourceId</span></span>|<span data-ttu-id="018f6-153">String</span><span class="sxs-lookup"><span data-stu-id="018f6-153">String</span></span>|<span data-ttu-id="018f6-154">是</span><span class="sxs-lookup"><span data-stu-id="018f6-154">Yes</span></span>|<span data-ttu-id="018f6-155">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="018f6-155">The ID of the resource.</span></span>|
|<span data-ttu-id="018f6-156">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="018f6-156">roleDefinitionId</span></span>|<span data-ttu-id="018f6-157">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-157">String</span></span>|<span data-ttu-id="018f6-158">是</span><span class="sxs-lookup"><span data-stu-id="018f6-158">Yes</span></span>|<span data-ttu-id="018f6-159">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="018f6-159">The ID of the role definition.</span></span>|
|<span data-ttu-id="018f6-160">subjectId</span><span class="sxs-lookup"><span data-stu-id="018f6-160">subjectId</span></span>|<span data-ttu-id="018f6-161">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-161">String</span></span>|<span data-ttu-id="018f6-162">是</span><span class="sxs-lookup"><span data-stu-id="018f6-162">Yes</span></span>|<span data-ttu-id="018f6-163">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="018f6-163">The ID of the subject.</span></span>|
|<span data-ttu-id="018f6-164">assignmentState</span><span class="sxs-lookup"><span data-stu-id="018f6-164">assignmentState</span></span>|<span data-ttu-id="018f6-165">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-165">String</span></span>|<span data-ttu-id="018f6-166">是</span><span class="sxs-lookup"><span data-stu-id="018f6-166">Yes</span></span>|<span data-ttu-id="018f6-167">工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="018f6-167">The state of assignment.</span></span> <span data-ttu-id="018f6-168">值可以是``Eligible``和``Active``。</span><span class="sxs-lookup"><span data-stu-id="018f6-168">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="018f6-169">type</span><span class="sxs-lookup"><span data-stu-id="018f6-169">type</span></span>|<span data-ttu-id="018f6-170">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-170">String</span></span>|<span data-ttu-id="018f6-171">是</span><span class="sxs-lookup"><span data-stu-id="018f6-171">Yes</span></span>|<span data-ttu-id="018f6-172">请求类型。</span><span class="sxs-lookup"><span data-stu-id="018f6-172">The request type.</span></span> <span data-ttu-id="018f6-173">值可以是`AdminAdd`， `UserAdd`， `AdminUpdate`， `AdminRemove`， `UserRemove`， `UserExtend`， `UserRenew`，`AdminRenew`和`AdminExtend`。</span><span class="sxs-lookup"><span data-stu-id="018f6-173">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="018f6-174">原因</span><span class="sxs-lookup"><span data-stu-id="018f6-174">reason</span></span>|<span data-ttu-id="018f6-175">String</span><span class="sxs-lookup"><span data-stu-id="018f6-175">String</span></span>| |<span data-ttu-id="018f6-176">原因需要提供角色分配请求的审核和查看用途。</span><span class="sxs-lookup"><span data-stu-id="018f6-176">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="018f6-177">计划</span><span class="sxs-lookup"><span data-stu-id="018f6-177">schedule</span></span>|[<span data-ttu-id="018f6-178">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="018f6-178">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="018f6-179">角色分配请求的时间表。</span><span class="sxs-lookup"><span data-stu-id="018f6-179">The schedule of the role assignment request.</span></span> <span data-ttu-id="018f6-180">请求类型的`UserAdd`， `AdminAdd`， `AdminUpdate`，和`AdminExtend`，需要。</span><span class="sxs-lookup"><span data-stu-id="018f6-180">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

## <a name="response"></a><span data-ttu-id="018f6-181">响应</span><span class="sxs-lookup"><span data-stu-id="018f6-181">Response</span></span>
<span data-ttu-id="018f6-182">如果成功，此方法返回`201 Created`响应代码和响应正文中的[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="018f6-182">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="018f6-183">错误代码</span><span class="sxs-lookup"><span data-stu-id="018f6-183">Error codes</span></span>
<span data-ttu-id="018f6-184">此 API 返回的标准 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="018f6-184">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="018f6-185">此外，它也会返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="018f6-185">In addition, it also returns the error codes listed in the following table.</span></span>

|<span data-ttu-id="018f6-186">错误代码</span><span class="sxs-lookup"><span data-stu-id="018f6-186">Error code</span></span>     | <span data-ttu-id="018f6-187">错误消息</span><span class="sxs-lookup"><span data-stu-id="018f6-187">Error message</span></span>              | <span data-ttu-id="018f6-188">详细信息</span><span class="sxs-lookup"><span data-stu-id="018f6-188">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="018f6-189">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="018f6-189">400 BadRequest</span></span> | <span data-ttu-id="018f6-190">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="018f6-190">RoleNotFound</span></span>    | <span data-ttu-id="018f6-191">`roleDefinitionId`提供在请求正文找不到。</span><span class="sxs-lookup"><span data-stu-id="018f6-191">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="018f6-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="018f6-192">400 BadRequest</span></span> | <span data-ttu-id="018f6-193">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="018f6-193">ResourceIsLocked</span></span>    | <span data-ttu-id="018f6-194">在请求正文中提供的资源处于状态的`Locked`和无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="018f6-194">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="018f6-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="018f6-195">400 BadRequest</span></span> | <span data-ttu-id="018f6-196">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="018f6-196">SubjectNotFound</span></span>    | <span data-ttu-id="018f6-197">`subjectId`提供在请求正文找不到。</span><span class="sxs-lookup"><span data-stu-id="018f6-197">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="018f6-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="018f6-198">400 BadRequest</span></span> | <span data-ttu-id="018f6-199">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="018f6-199">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="018f6-200">已存在挂起[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)系统中。</span><span class="sxs-lookup"><span data-stu-id="018f6-200">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="018f6-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="018f6-201">400 BadRequest</span></span> | <span data-ttu-id="018f6-202">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="018f6-202">RoleAssignmentExists</span></span>    | <span data-ttu-id="018f6-203">系统中存在[governanceRoleAssignment](../resources/governanceroleassignment.md)请求已创建。</span><span class="sxs-lookup"><span data-stu-id="018f6-203">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="018f6-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="018f6-204">400 BadRequest</span></span> | <span data-ttu-id="018f6-205">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="018f6-205">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="018f6-206">系统中不存在[governanceRoleAssignment](../resources/governanceroleassignment.md)请求来更新/扩展。</span><span class="sxs-lookup"><span data-stu-id="018f6-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="018f6-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="018f6-207">400 BadRequest</span></span> | <span data-ttu-id="018f6-208">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="018f6-208">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="018f6-209">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部的策略，且无法创建。</span><span class="sxs-lookup"><span data-stu-id="018f6-209">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="examples"></a><span data-ttu-id="018f6-210">示例</span><span class="sxs-lookup"><span data-stu-id="018f6-210">Examples</span></span>
<span data-ttu-id="018f6-211">下面的示例演示如何使用此 API。</span><span class="sxs-lookup"><span data-stu-id="018f6-211">The following examples show how to use this API.</span></span>

### <a name="example-1"></a><span data-ttu-id="018f6-212">示例 1</span><span class="sxs-lookup"><span data-stu-id="018f6-212">Example 1</span></span>
<span data-ttu-id="018f6-213">本示例中，管理员为帐单读者角色分配用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="018f6-213">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="018f6-214">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="018f6-214">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="018f6-215">属性</span><span class="sxs-lookup"><span data-stu-id="018f6-215">Property</span></span>     | <span data-ttu-id="018f6-216">类型</span><span class="sxs-lookup"><span data-stu-id="018f6-216">Type</span></span>    |<span data-ttu-id="018f6-217">是否必需</span><span class="sxs-lookup"><span data-stu-id="018f6-217">Required</span></span>|  <span data-ttu-id="018f6-218">值</span><span class="sxs-lookup"><span data-stu-id="018f6-218">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="018f6-219">resourceId</span><span class="sxs-lookup"><span data-stu-id="018f6-219">resourceId</span></span>|<span data-ttu-id="018f6-220">String</span><span class="sxs-lookup"><span data-stu-id="018f6-220">String</span></span>|<span data-ttu-id="018f6-221">是</span><span class="sxs-lookup"><span data-stu-id="018f6-221">Yes</span></span>|<span data-ttu-id="018f6-222">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="018f6-222">\<resourceId\></span></span>|
|<span data-ttu-id="018f6-223">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="018f6-223">roleDefinitionId</span></span>|<span data-ttu-id="018f6-224">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-224">String</span></span>|<span data-ttu-id="018f6-225">是</span><span class="sxs-lookup"><span data-stu-id="018f6-225">Yes</span></span>|<span data-ttu-id="018f6-226">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="018f6-226">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="018f6-227">subjectId</span><span class="sxs-lookup"><span data-stu-id="018f6-227">subjectId</span></span>|<span data-ttu-id="018f6-228">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-228">String</span></span>|<span data-ttu-id="018f6-229">是</span><span class="sxs-lookup"><span data-stu-id="018f6-229">Yes</span></span>|<span data-ttu-id="018f6-230">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="018f6-230">\<subjectId\></span></span>|
|<span data-ttu-id="018f6-231">assignmentState</span><span class="sxs-lookup"><span data-stu-id="018f6-231">assignmentState</span></span>|<span data-ttu-id="018f6-232">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-232">String</span></span>|<span data-ttu-id="018f6-233">是</span><span class="sxs-lookup"><span data-stu-id="018f6-233">Yes</span></span>| <span data-ttu-id="018f6-234">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="018f6-234">Eligible / Active</span></span>|
|<span data-ttu-id="018f6-235">type</span><span class="sxs-lookup"><span data-stu-id="018f6-235">type</span></span>|<span data-ttu-id="018f6-236">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-236">String</span></span>|<span data-ttu-id="018f6-237">是</span><span class="sxs-lookup"><span data-stu-id="018f6-237">Yes</span></span>| <span data-ttu-id="018f6-238">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="018f6-238">AdminAdd</span></span>|
|<span data-ttu-id="018f6-239">原因</span><span class="sxs-lookup"><span data-stu-id="018f6-239">reason</span></span>|<span data-ttu-id="018f6-240">String</span><span class="sxs-lookup"><span data-stu-id="018f6-240">String</span></span>| <span data-ttu-id="018f6-241">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="018f6-241">depends on role Settings</span></span>||
|<span data-ttu-id="018f6-242">计划</span><span class="sxs-lookup"><span data-stu-id="018f6-242">schedule</span></span>|[<span data-ttu-id="018f6-243">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="018f6-243">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="018f6-244">是</span><span class="sxs-lookup"><span data-stu-id="018f6-244">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="018f6-245">请求</span><span class="sxs-lookup"><span data-stu-id="018f6-245">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="018f6-246">响应</span><span class="sxs-lookup"><span data-stu-id="018f6-246">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="018f6-247">示例 2</span><span class="sxs-lookup"><span data-stu-id="018f6-247">Example 2</span></span>
<span data-ttu-id="018f6-248">本示例中，用户 nawu@fimdev.net 激活合格的帐单读取器角色。</span><span class="sxs-lookup"><span data-stu-id="018f6-248">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="018f6-249">属性</span><span class="sxs-lookup"><span data-stu-id="018f6-249">Property</span></span>     | <span data-ttu-id="018f6-250">类型</span><span class="sxs-lookup"><span data-stu-id="018f6-250">Type</span></span>    |<span data-ttu-id="018f6-251">是否必需</span><span class="sxs-lookup"><span data-stu-id="018f6-251">Required</span></span>|  <span data-ttu-id="018f6-252">值</span><span class="sxs-lookup"><span data-stu-id="018f6-252">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="018f6-253">resourceId</span><span class="sxs-lookup"><span data-stu-id="018f6-253">resourceId</span></span>|<span data-ttu-id="018f6-254">String</span><span class="sxs-lookup"><span data-stu-id="018f6-254">String</span></span>|<span data-ttu-id="018f6-255">是</span><span class="sxs-lookup"><span data-stu-id="018f6-255">Yes</span></span>|<span data-ttu-id="018f6-256">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="018f6-256">\<resourceId\></span></span>|
|<span data-ttu-id="018f6-257">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="018f6-257">roleDefinitionId</span></span>|<span data-ttu-id="018f6-258">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-258">String</span></span>|<span data-ttu-id="018f6-259">是</span><span class="sxs-lookup"><span data-stu-id="018f6-259">Yes</span></span>|<span data-ttu-id="018f6-260">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="018f6-260">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="018f6-261">subjectId</span><span class="sxs-lookup"><span data-stu-id="018f6-261">subjectId</span></span>|<span data-ttu-id="018f6-262">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-262">String</span></span>|<span data-ttu-id="018f6-263">是</span><span class="sxs-lookup"><span data-stu-id="018f6-263">Yes</span></span>|<span data-ttu-id="018f6-264">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="018f6-264">\<subjectId\></span></span>|
|<span data-ttu-id="018f6-265">assignmentState</span><span class="sxs-lookup"><span data-stu-id="018f6-265">assignmentState</span></span>|<span data-ttu-id="018f6-266">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-266">String</span></span>|<span data-ttu-id="018f6-267">是</span><span class="sxs-lookup"><span data-stu-id="018f6-267">Yes</span></span>| <span data-ttu-id="018f6-268">活动</span><span class="sxs-lookup"><span data-stu-id="018f6-268">Active</span></span>|
|<span data-ttu-id="018f6-269">type</span><span class="sxs-lookup"><span data-stu-id="018f6-269">type</span></span>|<span data-ttu-id="018f6-270">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-270">String</span></span>|<span data-ttu-id="018f6-271">是</span><span class="sxs-lookup"><span data-stu-id="018f6-271">Yes</span></span>| <span data-ttu-id="018f6-272">UserAdd</span><span class="sxs-lookup"><span data-stu-id="018f6-272">UserAdd</span></span>|
|<span data-ttu-id="018f6-273">原因</span><span class="sxs-lookup"><span data-stu-id="018f6-273">reason</span></span>|<span data-ttu-id="018f6-274">String</span><span class="sxs-lookup"><span data-stu-id="018f6-274">String</span></span>| <span data-ttu-id="018f6-275">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="018f6-275">depends on role Settings</span></span>||
|<span data-ttu-id="018f6-276">计划</span><span class="sxs-lookup"><span data-stu-id="018f6-276">schedule</span></span>|[<span data-ttu-id="018f6-277">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="018f6-277">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="018f6-278">是</span><span class="sxs-lookup"><span data-stu-id="018f6-278">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="018f6-279">请求</span><span class="sxs-lookup"><span data-stu-id="018f6-279">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="018f6-280">响应</span><span class="sxs-lookup"><span data-stu-id="018f6-280">Response</span></span>
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

### <a name="example-3"></a><span data-ttu-id="018f6-281">示例 3</span><span class="sxs-lookup"><span data-stu-id="018f6-281">Example 3</span></span>
<span data-ttu-id="018f6-282">本示例中，用户 nawu@fimdev.net 停用活动的帐单读取器角色。</span><span class="sxs-lookup"><span data-stu-id="018f6-282">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="018f6-283">属性</span><span class="sxs-lookup"><span data-stu-id="018f6-283">Property</span></span>     | <span data-ttu-id="018f6-284">类型</span><span class="sxs-lookup"><span data-stu-id="018f6-284">Type</span></span>    |<span data-ttu-id="018f6-285">是否必需</span><span class="sxs-lookup"><span data-stu-id="018f6-285">Required</span></span>|  <span data-ttu-id="018f6-286">值</span><span class="sxs-lookup"><span data-stu-id="018f6-286">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="018f6-287">resourceId</span><span class="sxs-lookup"><span data-stu-id="018f6-287">resourceId</span></span>|<span data-ttu-id="018f6-288">String</span><span class="sxs-lookup"><span data-stu-id="018f6-288">String</span></span>|<span data-ttu-id="018f6-289">是</span><span class="sxs-lookup"><span data-stu-id="018f6-289">Yes</span></span>|<span data-ttu-id="018f6-290">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="018f6-290">\<resourceId\></span></span>|
|<span data-ttu-id="018f6-291">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="018f6-291">roleDefinitionId</span></span>|<span data-ttu-id="018f6-292">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-292">String</span></span>|<span data-ttu-id="018f6-293">是</span><span class="sxs-lookup"><span data-stu-id="018f6-293">Yes</span></span>|<span data-ttu-id="018f6-294">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="018f6-294">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="018f6-295">subjectId</span><span class="sxs-lookup"><span data-stu-id="018f6-295">subjectId</span></span>|<span data-ttu-id="018f6-296">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-296">String</span></span>|<span data-ttu-id="018f6-297">是</span><span class="sxs-lookup"><span data-stu-id="018f6-297">Yes</span></span>|<span data-ttu-id="018f6-298">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="018f6-298">\<subjectId\></span></span>|
|<span data-ttu-id="018f6-299">assignmentState</span><span class="sxs-lookup"><span data-stu-id="018f6-299">assignmentState</span></span>|<span data-ttu-id="018f6-300">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-300">String</span></span>|<span data-ttu-id="018f6-301">是</span><span class="sxs-lookup"><span data-stu-id="018f6-301">Yes</span></span>| <span data-ttu-id="018f6-302">活动</span><span class="sxs-lookup"><span data-stu-id="018f6-302">Active</span></span>|
|<span data-ttu-id="018f6-303">type</span><span class="sxs-lookup"><span data-stu-id="018f6-303">type</span></span>|<span data-ttu-id="018f6-304">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-304">String</span></span>|<span data-ttu-id="018f6-305">是</span><span class="sxs-lookup"><span data-stu-id="018f6-305">Yes</span></span>| <span data-ttu-id="018f6-306">UserRemove</span><span class="sxs-lookup"><span data-stu-id="018f6-306">UserRemove</span></span>|
|<span data-ttu-id="018f6-307">原因</span><span class="sxs-lookup"><span data-stu-id="018f6-307">reason</span></span>|<span data-ttu-id="018f6-308">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-308">String</span></span>| <span data-ttu-id="018f6-309">否</span><span class="sxs-lookup"><span data-stu-id="018f6-309">No</span></span>||
|<span data-ttu-id="018f6-310">计划</span><span class="sxs-lookup"><span data-stu-id="018f6-310">schedule</span></span>|[<span data-ttu-id="018f6-311">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="018f6-311">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="018f6-312">否</span><span class="sxs-lookup"><span data-stu-id="018f6-312">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="018f6-313">请求</span><span class="sxs-lookup"><span data-stu-id="018f6-313">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="018f6-314">响应</span><span class="sxs-lookup"><span data-stu-id="018f6-314">Response</span></span>
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

### <a name="example-4"></a><span data-ttu-id="018f6-315">示例 4</span><span class="sxs-lookup"><span data-stu-id="018f6-315">Example 4</span></span>
<span data-ttu-id="018f6-316">本示例中，管理员从帐单读者角色中移除用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="018f6-316">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="018f6-317">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="018f6-317">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="018f6-318">属性</span><span class="sxs-lookup"><span data-stu-id="018f6-318">Property</span></span>     | <span data-ttu-id="018f6-319">类型</span><span class="sxs-lookup"><span data-stu-id="018f6-319">Type</span></span>    |<span data-ttu-id="018f6-320">是否必需</span><span class="sxs-lookup"><span data-stu-id="018f6-320">Required</span></span>|  <span data-ttu-id="018f6-321">值</span><span class="sxs-lookup"><span data-stu-id="018f6-321">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="018f6-322">resourceId</span><span class="sxs-lookup"><span data-stu-id="018f6-322">resourceId</span></span>|<span data-ttu-id="018f6-323">String</span><span class="sxs-lookup"><span data-stu-id="018f6-323">String</span></span>|<span data-ttu-id="018f6-324">是</span><span class="sxs-lookup"><span data-stu-id="018f6-324">Yes</span></span>|<span data-ttu-id="018f6-325">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="018f6-325">\<resourceId\></span></span>|
|<span data-ttu-id="018f6-326">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="018f6-326">roleDefinitionId</span></span>|<span data-ttu-id="018f6-327">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-327">String</span></span>|<span data-ttu-id="018f6-328">是</span><span class="sxs-lookup"><span data-stu-id="018f6-328">Yes</span></span>|<span data-ttu-id="018f6-329">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="018f6-329">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="018f6-330">subjectId</span><span class="sxs-lookup"><span data-stu-id="018f6-330">subjectId</span></span>|<span data-ttu-id="018f6-331">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-331">String</span></span>|<span data-ttu-id="018f6-332">是</span><span class="sxs-lookup"><span data-stu-id="018f6-332">Yes</span></span>|<span data-ttu-id="018f6-333">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="018f6-333">\<subjectId\></span></span>|
|<span data-ttu-id="018f6-334">assignmentState</span><span class="sxs-lookup"><span data-stu-id="018f6-334">assignmentState</span></span>|<span data-ttu-id="018f6-335">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-335">String</span></span>|<span data-ttu-id="018f6-336">是</span><span class="sxs-lookup"><span data-stu-id="018f6-336">Yes</span></span>| <span data-ttu-id="018f6-337">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="018f6-337">Eligible / Active</span></span>|
|<span data-ttu-id="018f6-338">type</span><span class="sxs-lookup"><span data-stu-id="018f6-338">type</span></span>|<span data-ttu-id="018f6-339">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-339">String</span></span>|<span data-ttu-id="018f6-340">是</span><span class="sxs-lookup"><span data-stu-id="018f6-340">Yes</span></span>| <span data-ttu-id="018f6-341">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="018f6-341">AdminRemove</span></span>|
|<span data-ttu-id="018f6-342">原因</span><span class="sxs-lookup"><span data-stu-id="018f6-342">reason</span></span>|<span data-ttu-id="018f6-343">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-343">String</span></span>| <span data-ttu-id="018f6-344">否</span><span class="sxs-lookup"><span data-stu-id="018f6-344">No</span></span>||
|<span data-ttu-id="018f6-345">计划</span><span class="sxs-lookup"><span data-stu-id="018f6-345">schedule</span></span>|[<span data-ttu-id="018f6-346">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="018f6-346">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="018f6-347">否</span><span class="sxs-lookup"><span data-stu-id="018f6-347">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="018f6-348">请求</span><span class="sxs-lookup"><span data-stu-id="018f6-348">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="018f6-349">响应</span><span class="sxs-lookup"><span data-stu-id="018f6-349">Response</span></span>
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

### <a name="example-5"></a><span data-ttu-id="018f6-350">示例 5</span><span class="sxs-lookup"><span data-stu-id="018f6-350">Example 5</span></span>
<span data-ttu-id="018f6-351">本示例中，管理员向所有者更新用户 nawu@fimdev.net 的角色分配。</span><span class="sxs-lookup"><span data-stu-id="018f6-351">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="018f6-352">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="018f6-352">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="018f6-353">属性</span><span class="sxs-lookup"><span data-stu-id="018f6-353">Property</span></span>     | <span data-ttu-id="018f6-354">类型</span><span class="sxs-lookup"><span data-stu-id="018f6-354">Type</span></span>    |<span data-ttu-id="018f6-355">是否必需</span><span class="sxs-lookup"><span data-stu-id="018f6-355">Required</span></span>|  <span data-ttu-id="018f6-356">值</span><span class="sxs-lookup"><span data-stu-id="018f6-356">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="018f6-357">resourceId</span><span class="sxs-lookup"><span data-stu-id="018f6-357">resourceId</span></span>|<span data-ttu-id="018f6-358">String</span><span class="sxs-lookup"><span data-stu-id="018f6-358">String</span></span>|<span data-ttu-id="018f6-359">是</span><span class="sxs-lookup"><span data-stu-id="018f6-359">Yes</span></span>|<span data-ttu-id="018f6-360">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="018f6-360">\<resourceId\></span></span>|
|<span data-ttu-id="018f6-361">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="018f6-361">roleDefinitionId</span></span>|<span data-ttu-id="018f6-362">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-362">String</span></span>|<span data-ttu-id="018f6-363">是</span><span class="sxs-lookup"><span data-stu-id="018f6-363">Yes</span></span>|<span data-ttu-id="018f6-364">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="018f6-364">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="018f6-365">subjectId</span><span class="sxs-lookup"><span data-stu-id="018f6-365">subjectId</span></span>|<span data-ttu-id="018f6-366">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-366">String</span></span>|<span data-ttu-id="018f6-367">是</span><span class="sxs-lookup"><span data-stu-id="018f6-367">Yes</span></span>|<span data-ttu-id="018f6-368">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="018f6-368">\<subjectId\></span></span>|
|<span data-ttu-id="018f6-369">assignmentState</span><span class="sxs-lookup"><span data-stu-id="018f6-369">assignmentState</span></span>|<span data-ttu-id="018f6-370">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-370">String</span></span>|<span data-ttu-id="018f6-371">是</span><span class="sxs-lookup"><span data-stu-id="018f6-371">Yes</span></span>| <span data-ttu-id="018f6-372">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="018f6-372">Eligible / Active</span></span>|
|<span data-ttu-id="018f6-373">type</span><span class="sxs-lookup"><span data-stu-id="018f6-373">type</span></span>|<span data-ttu-id="018f6-374">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-374">String</span></span>|<span data-ttu-id="018f6-375">是</span><span class="sxs-lookup"><span data-stu-id="018f6-375">Yes</span></span>| <span data-ttu-id="018f6-376">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="018f6-376">AdminUpdate</span></span>|
|<span data-ttu-id="018f6-377">原因</span><span class="sxs-lookup"><span data-stu-id="018f6-377">reason</span></span>|<span data-ttu-id="018f6-378">String</span><span class="sxs-lookup"><span data-stu-id="018f6-378">String</span></span>| <span data-ttu-id="018f6-379">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="018f6-379">depends on roleSettings</span></span>||
|<span data-ttu-id="018f6-380">计划</span><span class="sxs-lookup"><span data-stu-id="018f6-380">schedule</span></span>|[<span data-ttu-id="018f6-381">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="018f6-381">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="018f6-382">是</span><span class="sxs-lookup"><span data-stu-id="018f6-382">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="018f6-383">请求</span><span class="sxs-lookup"><span data-stu-id="018f6-383">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="018f6-384">响应</span><span class="sxs-lookup"><span data-stu-id="018f6-384">Response</span></span>
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

### <a name="example-6"></a><span data-ttu-id="018f6-385">示例 6</span><span class="sxs-lookup"><span data-stu-id="018f6-385">Example 6</span></span>
<span data-ttu-id="018f6-386">本示例将用户 ANUJCUSER 即将过期的角色分配给 API 管理服务参与者。</span><span class="sxs-lookup"><span data-stu-id="018f6-386">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="018f6-387">**注意：** 另外还包括的权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="018f6-387">**Note:** In additon to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="018f6-388">属性</span><span class="sxs-lookup"><span data-stu-id="018f6-388">Property</span></span>     | <span data-ttu-id="018f6-389">类型</span><span class="sxs-lookup"><span data-stu-id="018f6-389">Type</span></span>    |<span data-ttu-id="018f6-390">是否必需</span><span class="sxs-lookup"><span data-stu-id="018f6-390">Required</span></span>|  <span data-ttu-id="018f6-391">值</span><span class="sxs-lookup"><span data-stu-id="018f6-391">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="018f6-392">resourceId</span><span class="sxs-lookup"><span data-stu-id="018f6-392">resourceId</span></span>|<span data-ttu-id="018f6-393">String</span><span class="sxs-lookup"><span data-stu-id="018f6-393">String</span></span>|<span data-ttu-id="018f6-394">是</span><span class="sxs-lookup"><span data-stu-id="018f6-394">Yes</span></span>|<span data-ttu-id="018f6-395">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="018f6-395">\<resourceId\></span></span>|
|<span data-ttu-id="018f6-396">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="018f6-396">roleDefinitionId</span></span>|<span data-ttu-id="018f6-397">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-397">String</span></span>|<span data-ttu-id="018f6-398">是</span><span class="sxs-lookup"><span data-stu-id="018f6-398">Yes</span></span>|<span data-ttu-id="018f6-399">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="018f6-399">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="018f6-400">subjectId</span><span class="sxs-lookup"><span data-stu-id="018f6-400">subjectId</span></span>|<span data-ttu-id="018f6-401">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-401">String</span></span>|<span data-ttu-id="018f6-402">是</span><span class="sxs-lookup"><span data-stu-id="018f6-402">Yes</span></span>|<span data-ttu-id="018f6-403">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="018f6-403">\<subjectId\></span></span>|
|<span data-ttu-id="018f6-404">assignmentState</span><span class="sxs-lookup"><span data-stu-id="018f6-404">assignmentState</span></span>|<span data-ttu-id="018f6-405">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-405">String</span></span>|<span data-ttu-id="018f6-406">是</span><span class="sxs-lookup"><span data-stu-id="018f6-406">Yes</span></span>| <span data-ttu-id="018f6-407">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="018f6-407">Eligible / Active</span></span> |
|<span data-ttu-id="018f6-408">type</span><span class="sxs-lookup"><span data-stu-id="018f6-408">type</span></span>|<span data-ttu-id="018f6-409">字符串</span><span class="sxs-lookup"><span data-stu-id="018f6-409">String</span></span>|<span data-ttu-id="018f6-410">是</span><span class="sxs-lookup"><span data-stu-id="018f6-410">Yes</span></span>| <span data-ttu-id="018f6-411">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="018f6-411">AdminExtend</span></span>|
|<span data-ttu-id="018f6-412">原因</span><span class="sxs-lookup"><span data-stu-id="018f6-412">reason</span></span>|<span data-ttu-id="018f6-413">String</span><span class="sxs-lookup"><span data-stu-id="018f6-413">String</span></span>| <span data-ttu-id="018f6-414">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="018f6-414">depends on roleSettings</span></span>||
|<span data-ttu-id="018f6-415">计划</span><span class="sxs-lookup"><span data-stu-id="018f6-415">schedule</span></span>|[<span data-ttu-id="018f6-416">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="018f6-416">microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="018f6-417">是</span><span class="sxs-lookup"><span data-stu-id="018f6-417">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="018f6-418">请求</span><span class="sxs-lookup"><span data-stu-id="018f6-418">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="018f6-419">响应</span><span class="sxs-lookup"><span data-stu-id="018f6-419">Response</span></span>
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
