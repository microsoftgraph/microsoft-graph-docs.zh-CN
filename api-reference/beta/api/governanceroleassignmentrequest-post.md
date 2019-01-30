---
title: 创建 governanceRoleAssignmentRequest
description: 创建角色分配请求以表示该操作所需角色分配。 下表列出的操作。
localization_priority: Normal
ms.openlocfilehash: c936a6cd0ba061fc1dd3758533781d7270673939
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641265"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="b7f78-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="b7f78-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7f78-105">创建角色分配请求以表示该操作所需角色分配。</span><span class="sxs-lookup"><span data-stu-id="b7f78-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="b7f78-106">下表列出的操作。</span><span class="sxs-lookup"><span data-stu-id="b7f78-106">The following table lists the operations.</span></span>

| <span data-ttu-id="b7f78-107">操作</span><span class="sxs-lookup"><span data-stu-id="b7f78-107">Operation</span></span>       | <span data-ttu-id="b7f78-108">类型</span><span class="sxs-lookup"><span data-stu-id="b7f78-108">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="b7f78-109">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="b7f78-109">Assign a role assignment</span></span>| <span data-ttu-id="b7f78-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="b7f78-110">AdminAdd</span></span> |
| <span data-ttu-id="b7f78-111">激活合格的角色分配</span><span class="sxs-lookup"><span data-stu-id="b7f78-111">Activate an eligible role assignment</span></span>| <span data-ttu-id="b7f78-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="b7f78-112">UserAdd</span></span> | 
| <span data-ttu-id="b7f78-113">停用已激活的角色分配</span><span class="sxs-lookup"><span data-stu-id="b7f78-113">Deactivate an activated role assignment</span></span>| <span data-ttu-id="b7f78-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="b7f78-114">UserRemove</span></span> | 
| <span data-ttu-id="b7f78-115">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="b7f78-115">Remove a role assignment</span></span>| <span data-ttu-id="b7f78-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="b7f78-116">AdminRemove</span></span> |
| <span data-ttu-id="b7f78-117">更新一个角色分配</span><span class="sxs-lookup"><span data-stu-id="b7f78-117">Update a role assignment</span></span>| <span data-ttu-id="b7f78-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="b7f78-118">AdminUpdate</span></span> |
| <span data-ttu-id="b7f78-119">请求扩展我角色分配</span><span class="sxs-lookup"><span data-stu-id="b7f78-119">Request to extend my role assignment</span></span>| <span data-ttu-id="b7f78-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="b7f78-120">UserExtend</span></span> | 
| <span data-ttu-id="b7f78-121">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="b7f78-121">Extend a role assignment</span></span>| <span data-ttu-id="b7f78-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="b7f78-122">AdminExtend</span></span> | 
| <span data-ttu-id="b7f78-123">请求续订我过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="b7f78-123">Request to renew my expired role assignment</span></span>| <span data-ttu-id="b7f78-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="b7f78-124">UserRenew</span></span> | 
| <span data-ttu-id="b7f78-125">续订已过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="b7f78-125">Renew an expired role assignment</span></span>| <span data-ttu-id="b7f78-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="b7f78-126">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="b7f78-127">权限</span><span class="sxs-lookup"><span data-stu-id="b7f78-127">Permissions</span></span>
<span data-ttu-id="b7f78-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7f78-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7f78-130">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7f78-130">Permission type</span></span>      | <span data-ttu-id="b7f78-131">权限</span><span class="sxs-lookup"><span data-stu-id="b7f78-131">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7f78-132">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7f78-132">Delegated (work or school account)</span></span> | <span data-ttu-id="b7f78-133">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b7f78-133">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="b7f78-134">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7f78-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7f78-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7f78-135">Not supported.</span></span>    |
|<span data-ttu-id="b7f78-136">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7f78-136">Application</span></span> | <span data-ttu-id="b7f78-137">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b7f78-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7f78-138">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7f78-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="b7f78-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7f78-139">Request headers</span></span>
| <span data-ttu-id="b7f78-140">名称</span><span class="sxs-lookup"><span data-stu-id="b7f78-140">Name</span></span>       | <span data-ttu-id="b7f78-141">说明</span><span class="sxs-lookup"><span data-stu-id="b7f78-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b7f78-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7f78-142">Authorization</span></span>  | <span data-ttu-id="b7f78-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b7f78-143">Bearer {code}</span></span>|
| <span data-ttu-id="b7f78-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="b7f78-144">Content-type</span></span>  | <span data-ttu-id="b7f78-145">application/json</span><span class="sxs-lookup"><span data-stu-id="b7f78-145">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7f78-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7f78-146">Request body</span></span>
<span data-ttu-id="b7f78-147">在请求正文中，提供[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7f78-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="b7f78-148">属性</span><span class="sxs-lookup"><span data-stu-id="b7f78-148">Property</span></span>     | <span data-ttu-id="b7f78-149">类型</span><span class="sxs-lookup"><span data-stu-id="b7f78-149">Type</span></span>    |<span data-ttu-id="b7f78-150">必需</span><span class="sxs-lookup"><span data-stu-id="b7f78-150">Required</span></span>|  <span data-ttu-id="b7f78-151">说明</span><span class="sxs-lookup"><span data-stu-id="b7f78-151">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="b7f78-152">resourceId</span><span class="sxs-lookup"><span data-stu-id="b7f78-152">resourceId</span></span>|<span data-ttu-id="b7f78-153">String</span><span class="sxs-lookup"><span data-stu-id="b7f78-153">String</span></span>|<span data-ttu-id="b7f78-154">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-154">Yes</span></span>|<span data-ttu-id="b7f78-155">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="b7f78-155">The ID of the resource.</span></span>|
|<span data-ttu-id="b7f78-156">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b7f78-156">roleDefinitionId</span></span>|<span data-ttu-id="b7f78-157">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-157">String</span></span>|<span data-ttu-id="b7f78-158">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-158">Yes</span></span>|<span data-ttu-id="b7f78-159">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="b7f78-159">The ID of the role definition.</span></span>|
|<span data-ttu-id="b7f78-160">subjectId</span><span class="sxs-lookup"><span data-stu-id="b7f78-160">subjectId</span></span>|<span data-ttu-id="b7f78-161">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-161">String</span></span>|<span data-ttu-id="b7f78-162">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-162">Yes</span></span>|<span data-ttu-id="b7f78-163">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="b7f78-163">The ID of the subject.</span></span>|
|<span data-ttu-id="b7f78-164">assignmentState</span><span class="sxs-lookup"><span data-stu-id="b7f78-164">assignmentState</span></span>|<span data-ttu-id="b7f78-165">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-165">String</span></span>|<span data-ttu-id="b7f78-166">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-166">Yes</span></span>|<span data-ttu-id="b7f78-167">工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="b7f78-167">The state of assignment.</span></span> <span data-ttu-id="b7f78-168">值可以是``Eligible``和``Active``。</span><span class="sxs-lookup"><span data-stu-id="b7f78-168">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="b7f78-169">type</span><span class="sxs-lookup"><span data-stu-id="b7f78-169">type</span></span>|<span data-ttu-id="b7f78-170">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-170">String</span></span>|<span data-ttu-id="b7f78-171">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-171">Yes</span></span>|<span data-ttu-id="b7f78-172">请求类型。</span><span class="sxs-lookup"><span data-stu-id="b7f78-172">The request type.</span></span> <span data-ttu-id="b7f78-173">值可以是`AdminAdd`， `UserAdd`， `AdminUpdate`， `AdminRemove`， `UserRemove`， `UserExtend`， `UserRenew`，`AdminRenew`和`AdminExtend`。</span><span class="sxs-lookup"><span data-stu-id="b7f78-173">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="b7f78-174">原因</span><span class="sxs-lookup"><span data-stu-id="b7f78-174">reason</span></span>|<span data-ttu-id="b7f78-175">String</span><span class="sxs-lookup"><span data-stu-id="b7f78-175">String</span></span>| |<span data-ttu-id="b7f78-176">原因需要提供角色分配请求的审核和查看用途。</span><span class="sxs-lookup"><span data-stu-id="b7f78-176">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="b7f78-177">计划</span><span class="sxs-lookup"><span data-stu-id="b7f78-177">schedule</span></span>|[<span data-ttu-id="b7f78-178">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b7f78-178">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="b7f78-179">角色分配请求的时间表。</span><span class="sxs-lookup"><span data-stu-id="b7f78-179">The schedule of the role assignment request.</span></span> <span data-ttu-id="b7f78-180">请求类型的`UserAdd`， `AdminAdd`， `AdminUpdate`，和`AdminExtend`，需要。</span><span class="sxs-lookup"><span data-stu-id="b7f78-180">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

## <a name="response"></a><span data-ttu-id="b7f78-181">响应</span><span class="sxs-lookup"><span data-stu-id="b7f78-181">Response</span></span>
<span data-ttu-id="b7f78-182">如果成功，此方法返回`201 Created`响应代码和响应正文中的[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b7f78-182">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="b7f78-183">错误代码</span><span class="sxs-lookup"><span data-stu-id="b7f78-183">Error codes</span></span>
<span data-ttu-id="b7f78-184">此 API 返回的标准 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="b7f78-184">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="b7f78-185">此外，它也会返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="b7f78-185">In addition, it also returns the error codes listed in the following table.</span></span>

|<span data-ttu-id="b7f78-186">错误代码</span><span class="sxs-lookup"><span data-stu-id="b7f78-186">Error code</span></span>     | <span data-ttu-id="b7f78-187">错误消息</span><span class="sxs-lookup"><span data-stu-id="b7f78-187">Error message</span></span>              | <span data-ttu-id="b7f78-188">详细信息</span><span class="sxs-lookup"><span data-stu-id="b7f78-188">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="b7f78-189">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="b7f78-189">400 BadRequest</span></span> | <span data-ttu-id="b7f78-190">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="b7f78-190">RoleNotFound</span></span>    | <span data-ttu-id="b7f78-191">`roleDefinitionId`提供在请求正文找不到。</span><span class="sxs-lookup"><span data-stu-id="b7f78-191">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="b7f78-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="b7f78-192">400 BadRequest</span></span> | <span data-ttu-id="b7f78-193">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="b7f78-193">ResourceIsLocked</span></span>    | <span data-ttu-id="b7f78-194">在请求正文中提供的资源处于状态的`Locked`和无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="b7f78-194">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="b7f78-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="b7f78-195">400 BadRequest</span></span> | <span data-ttu-id="b7f78-196">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="b7f78-196">SubjectNotFound</span></span>    | <span data-ttu-id="b7f78-197">`subjectId`提供在请求正文找不到。</span><span class="sxs-lookup"><span data-stu-id="b7f78-197">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="b7f78-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="b7f78-198">400 BadRequest</span></span> | <span data-ttu-id="b7f78-199">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="b7f78-199">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="b7f78-200">已存在挂起[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)系统中。</span><span class="sxs-lookup"><span data-stu-id="b7f78-200">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="b7f78-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="b7f78-201">400 BadRequest</span></span> | <span data-ttu-id="b7f78-202">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="b7f78-202">RoleAssignmentExists</span></span>    | <span data-ttu-id="b7f78-203">系统中存在[governanceRoleAssignment](../resources/governanceroleassignment.md)请求已创建。</span><span class="sxs-lookup"><span data-stu-id="b7f78-203">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="b7f78-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="b7f78-204">400 BadRequest</span></span> | <span data-ttu-id="b7f78-205">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="b7f78-205">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="b7f78-206">系统中不存在[governanceRoleAssignment](../resources/governanceroleassignment.md)请求来更新/扩展。</span><span class="sxs-lookup"><span data-stu-id="b7f78-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="b7f78-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="b7f78-207">400 BadRequest</span></span> | <span data-ttu-id="b7f78-208">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="b7f78-208">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="b7f78-209">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部的策略，且无法创建。</span><span class="sxs-lookup"><span data-stu-id="b7f78-209">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="examples"></a><span data-ttu-id="b7f78-210">示例</span><span class="sxs-lookup"><span data-stu-id="b7f78-210">Examples</span></span>
<span data-ttu-id="b7f78-211">下面的示例演示如何使用此 API。</span><span class="sxs-lookup"><span data-stu-id="b7f78-211">The following examples show how to use this API.</span></span>

### <a name="example-1"></a><span data-ttu-id="b7f78-212">示例 1</span><span class="sxs-lookup"><span data-stu-id="b7f78-212">Example 1</span></span>
<span data-ttu-id="b7f78-213">本示例中，管理员为帐单读者角色分配用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="b7f78-213">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="b7f78-214">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="b7f78-214">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="b7f78-215">属性</span><span class="sxs-lookup"><span data-stu-id="b7f78-215">Property</span></span>     | <span data-ttu-id="b7f78-216">类型</span><span class="sxs-lookup"><span data-stu-id="b7f78-216">Type</span></span>    |<span data-ttu-id="b7f78-217">是否必需</span><span class="sxs-lookup"><span data-stu-id="b7f78-217">Required</span></span>|  <span data-ttu-id="b7f78-218">值</span><span class="sxs-lookup"><span data-stu-id="b7f78-218">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="b7f78-219">resourceId</span><span class="sxs-lookup"><span data-stu-id="b7f78-219">resourceId</span></span>|<span data-ttu-id="b7f78-220">String</span><span class="sxs-lookup"><span data-stu-id="b7f78-220">String</span></span>|<span data-ttu-id="b7f78-221">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-221">Yes</span></span>|<span data-ttu-id="b7f78-222">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="b7f78-222">\<resourceId\></span></span>|
|<span data-ttu-id="b7f78-223">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b7f78-223">roleDefinitionId</span></span>|<span data-ttu-id="b7f78-224">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-224">String</span></span>|<span data-ttu-id="b7f78-225">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-225">Yes</span></span>|<span data-ttu-id="b7f78-226">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="b7f78-226">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="b7f78-227">subjectId</span><span class="sxs-lookup"><span data-stu-id="b7f78-227">subjectId</span></span>|<span data-ttu-id="b7f78-228">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-228">String</span></span>|<span data-ttu-id="b7f78-229">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-229">Yes</span></span>|<span data-ttu-id="b7f78-230">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="b7f78-230">\<subjectId\></span></span>|
|<span data-ttu-id="b7f78-231">assignmentState</span><span class="sxs-lookup"><span data-stu-id="b7f78-231">assignmentState</span></span>|<span data-ttu-id="b7f78-232">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-232">String</span></span>|<span data-ttu-id="b7f78-233">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-233">Yes</span></span>| <span data-ttu-id="b7f78-234">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="b7f78-234">Eligible / Active</span></span>|
|<span data-ttu-id="b7f78-235">type</span><span class="sxs-lookup"><span data-stu-id="b7f78-235">type</span></span>|<span data-ttu-id="b7f78-236">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-236">String</span></span>|<span data-ttu-id="b7f78-237">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-237">Yes</span></span>| <span data-ttu-id="b7f78-238">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="b7f78-238">AdminAdd</span></span>|
|<span data-ttu-id="b7f78-239">原因</span><span class="sxs-lookup"><span data-stu-id="b7f78-239">reason</span></span>|<span data-ttu-id="b7f78-240">String</span><span class="sxs-lookup"><span data-stu-id="b7f78-240">String</span></span>| <span data-ttu-id="b7f78-241">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="b7f78-241">depends on role Settings</span></span>||
|<span data-ttu-id="b7f78-242">计划</span><span class="sxs-lookup"><span data-stu-id="b7f78-242">schedule</span></span>|[<span data-ttu-id="b7f78-243">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b7f78-243">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="b7f78-244">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-244">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="b7f78-245">请求</span><span class="sxs-lookup"><span data-stu-id="b7f78-245">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="b7f78-246">响应</span><span class="sxs-lookup"><span data-stu-id="b7f78-246">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="b7f78-247">示例 2</span><span class="sxs-lookup"><span data-stu-id="b7f78-247">Example 2</span></span>
<span data-ttu-id="b7f78-248">本示例中，用户 nawu@fimdev.net 激活合格的帐单读取器角色。</span><span class="sxs-lookup"><span data-stu-id="b7f78-248">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="b7f78-249">属性</span><span class="sxs-lookup"><span data-stu-id="b7f78-249">Property</span></span>     | <span data-ttu-id="b7f78-250">类型</span><span class="sxs-lookup"><span data-stu-id="b7f78-250">Type</span></span>    |<span data-ttu-id="b7f78-251">是否必需</span><span class="sxs-lookup"><span data-stu-id="b7f78-251">Required</span></span>|  <span data-ttu-id="b7f78-252">值</span><span class="sxs-lookup"><span data-stu-id="b7f78-252">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="b7f78-253">resourceId</span><span class="sxs-lookup"><span data-stu-id="b7f78-253">resourceId</span></span>|<span data-ttu-id="b7f78-254">String</span><span class="sxs-lookup"><span data-stu-id="b7f78-254">String</span></span>|<span data-ttu-id="b7f78-255">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-255">Yes</span></span>|<span data-ttu-id="b7f78-256">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="b7f78-256">\<resourceId\></span></span>|
|<span data-ttu-id="b7f78-257">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b7f78-257">roleDefinitionId</span></span>|<span data-ttu-id="b7f78-258">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-258">String</span></span>|<span data-ttu-id="b7f78-259">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-259">Yes</span></span>|<span data-ttu-id="b7f78-260">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="b7f78-260">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="b7f78-261">subjectId</span><span class="sxs-lookup"><span data-stu-id="b7f78-261">subjectId</span></span>|<span data-ttu-id="b7f78-262">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-262">String</span></span>|<span data-ttu-id="b7f78-263">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-263">Yes</span></span>|<span data-ttu-id="b7f78-264">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="b7f78-264">\<subjectId\></span></span>|
|<span data-ttu-id="b7f78-265">assignmentState</span><span class="sxs-lookup"><span data-stu-id="b7f78-265">assignmentState</span></span>|<span data-ttu-id="b7f78-266">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-266">String</span></span>|<span data-ttu-id="b7f78-267">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-267">Yes</span></span>| <span data-ttu-id="b7f78-268">活动</span><span class="sxs-lookup"><span data-stu-id="b7f78-268">Active</span></span>|
|<span data-ttu-id="b7f78-269">type</span><span class="sxs-lookup"><span data-stu-id="b7f78-269">type</span></span>|<span data-ttu-id="b7f78-270">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-270">String</span></span>|<span data-ttu-id="b7f78-271">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-271">Yes</span></span>| <span data-ttu-id="b7f78-272">UserAdd</span><span class="sxs-lookup"><span data-stu-id="b7f78-272">UserAdd</span></span>|
|<span data-ttu-id="b7f78-273">原因</span><span class="sxs-lookup"><span data-stu-id="b7f78-273">reason</span></span>|<span data-ttu-id="b7f78-274">String</span><span class="sxs-lookup"><span data-stu-id="b7f78-274">String</span></span>| <span data-ttu-id="b7f78-275">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="b7f78-275">depends on role Settings</span></span>||
|<span data-ttu-id="b7f78-276">计划</span><span class="sxs-lookup"><span data-stu-id="b7f78-276">schedule</span></span>|[<span data-ttu-id="b7f78-277">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b7f78-277">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="b7f78-278">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-278">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="b7f78-279">请求</span><span class="sxs-lookup"><span data-stu-id="b7f78-279">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="b7f78-280">响应</span><span class="sxs-lookup"><span data-stu-id="b7f78-280">Response</span></span>
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

### <a name="example-3"></a><span data-ttu-id="b7f78-281">示例 3</span><span class="sxs-lookup"><span data-stu-id="b7f78-281">Example 3</span></span>
<span data-ttu-id="b7f78-282">本示例中，用户 nawu@fimdev.net 停用活动的帐单读取器角色。</span><span class="sxs-lookup"><span data-stu-id="b7f78-282">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="b7f78-283">属性</span><span class="sxs-lookup"><span data-stu-id="b7f78-283">Property</span></span>     | <span data-ttu-id="b7f78-284">类型</span><span class="sxs-lookup"><span data-stu-id="b7f78-284">Type</span></span>    |<span data-ttu-id="b7f78-285">是否必需</span><span class="sxs-lookup"><span data-stu-id="b7f78-285">Required</span></span>|  <span data-ttu-id="b7f78-286">值</span><span class="sxs-lookup"><span data-stu-id="b7f78-286">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="b7f78-287">resourceId</span><span class="sxs-lookup"><span data-stu-id="b7f78-287">resourceId</span></span>|<span data-ttu-id="b7f78-288">String</span><span class="sxs-lookup"><span data-stu-id="b7f78-288">String</span></span>|<span data-ttu-id="b7f78-289">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-289">Yes</span></span>|<span data-ttu-id="b7f78-290">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="b7f78-290">\<resourceId\></span></span>|
|<span data-ttu-id="b7f78-291">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b7f78-291">roleDefinitionId</span></span>|<span data-ttu-id="b7f78-292">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-292">String</span></span>|<span data-ttu-id="b7f78-293">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-293">Yes</span></span>|<span data-ttu-id="b7f78-294">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="b7f78-294">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="b7f78-295">subjectId</span><span class="sxs-lookup"><span data-stu-id="b7f78-295">subjectId</span></span>|<span data-ttu-id="b7f78-296">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-296">String</span></span>|<span data-ttu-id="b7f78-297">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-297">Yes</span></span>|<span data-ttu-id="b7f78-298">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="b7f78-298">\<subjectId\></span></span>|
|<span data-ttu-id="b7f78-299">assignmentState</span><span class="sxs-lookup"><span data-stu-id="b7f78-299">assignmentState</span></span>|<span data-ttu-id="b7f78-300">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-300">String</span></span>|<span data-ttu-id="b7f78-301">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-301">Yes</span></span>| <span data-ttu-id="b7f78-302">活动</span><span class="sxs-lookup"><span data-stu-id="b7f78-302">Active</span></span>|
|<span data-ttu-id="b7f78-303">type</span><span class="sxs-lookup"><span data-stu-id="b7f78-303">type</span></span>|<span data-ttu-id="b7f78-304">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-304">String</span></span>|<span data-ttu-id="b7f78-305">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-305">Yes</span></span>| <span data-ttu-id="b7f78-306">UserRemove</span><span class="sxs-lookup"><span data-stu-id="b7f78-306">UserRemove</span></span>|
|<span data-ttu-id="b7f78-307">原因</span><span class="sxs-lookup"><span data-stu-id="b7f78-307">reason</span></span>|<span data-ttu-id="b7f78-308">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-308">String</span></span>| <span data-ttu-id="b7f78-309">否</span><span class="sxs-lookup"><span data-stu-id="b7f78-309">No</span></span>||
|<span data-ttu-id="b7f78-310">计划</span><span class="sxs-lookup"><span data-stu-id="b7f78-310">schedule</span></span>|[<span data-ttu-id="b7f78-311">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b7f78-311">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="b7f78-312">否</span><span class="sxs-lookup"><span data-stu-id="b7f78-312">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="b7f78-313">请求</span><span class="sxs-lookup"><span data-stu-id="b7f78-313">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="b7f78-314">响应</span><span class="sxs-lookup"><span data-stu-id="b7f78-314">Response</span></span>
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

### <a name="example-4"></a><span data-ttu-id="b7f78-315">示例 4</span><span class="sxs-lookup"><span data-stu-id="b7f78-315">Example 4</span></span>
<span data-ttu-id="b7f78-316">本示例中，管理员从帐单读者角色中移除用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="b7f78-316">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="b7f78-317">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="b7f78-317">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="b7f78-318">属性</span><span class="sxs-lookup"><span data-stu-id="b7f78-318">Property</span></span>     | <span data-ttu-id="b7f78-319">类型</span><span class="sxs-lookup"><span data-stu-id="b7f78-319">Type</span></span>    |<span data-ttu-id="b7f78-320">是否必需</span><span class="sxs-lookup"><span data-stu-id="b7f78-320">Required</span></span>|  <span data-ttu-id="b7f78-321">值</span><span class="sxs-lookup"><span data-stu-id="b7f78-321">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="b7f78-322">resourceId</span><span class="sxs-lookup"><span data-stu-id="b7f78-322">resourceId</span></span>|<span data-ttu-id="b7f78-323">String</span><span class="sxs-lookup"><span data-stu-id="b7f78-323">String</span></span>|<span data-ttu-id="b7f78-324">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-324">Yes</span></span>|<span data-ttu-id="b7f78-325">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="b7f78-325">\<resourceId\></span></span>|
|<span data-ttu-id="b7f78-326">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b7f78-326">roleDefinitionId</span></span>|<span data-ttu-id="b7f78-327">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-327">String</span></span>|<span data-ttu-id="b7f78-328">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-328">Yes</span></span>|<span data-ttu-id="b7f78-329">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="b7f78-329">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="b7f78-330">subjectId</span><span class="sxs-lookup"><span data-stu-id="b7f78-330">subjectId</span></span>|<span data-ttu-id="b7f78-331">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-331">String</span></span>|<span data-ttu-id="b7f78-332">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-332">Yes</span></span>|<span data-ttu-id="b7f78-333">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="b7f78-333">\<subjectId\></span></span>|
|<span data-ttu-id="b7f78-334">assignmentState</span><span class="sxs-lookup"><span data-stu-id="b7f78-334">assignmentState</span></span>|<span data-ttu-id="b7f78-335">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-335">String</span></span>|<span data-ttu-id="b7f78-336">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-336">Yes</span></span>| <span data-ttu-id="b7f78-337">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="b7f78-337">Eligible / Active</span></span>|
|<span data-ttu-id="b7f78-338">type</span><span class="sxs-lookup"><span data-stu-id="b7f78-338">type</span></span>|<span data-ttu-id="b7f78-339">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-339">String</span></span>|<span data-ttu-id="b7f78-340">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-340">Yes</span></span>| <span data-ttu-id="b7f78-341">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="b7f78-341">AdminRemove</span></span>|
|<span data-ttu-id="b7f78-342">原因</span><span class="sxs-lookup"><span data-stu-id="b7f78-342">reason</span></span>|<span data-ttu-id="b7f78-343">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-343">String</span></span>| <span data-ttu-id="b7f78-344">否</span><span class="sxs-lookup"><span data-stu-id="b7f78-344">No</span></span>||
|<span data-ttu-id="b7f78-345">计划</span><span class="sxs-lookup"><span data-stu-id="b7f78-345">schedule</span></span>|[<span data-ttu-id="b7f78-346">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b7f78-346">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="b7f78-347">否</span><span class="sxs-lookup"><span data-stu-id="b7f78-347">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="b7f78-348">请求</span><span class="sxs-lookup"><span data-stu-id="b7f78-348">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="b7f78-349">响应</span><span class="sxs-lookup"><span data-stu-id="b7f78-349">Response</span></span>
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

### <a name="example-5"></a><span data-ttu-id="b7f78-350">示例 5</span><span class="sxs-lookup"><span data-stu-id="b7f78-350">Example 5</span></span>
<span data-ttu-id="b7f78-351">本示例中，管理员向所有者更新用户 nawu@fimdev.net 的角色分配。</span><span class="sxs-lookup"><span data-stu-id="b7f78-351">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="b7f78-352">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="b7f78-352">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="b7f78-353">属性</span><span class="sxs-lookup"><span data-stu-id="b7f78-353">Property</span></span>     | <span data-ttu-id="b7f78-354">类型</span><span class="sxs-lookup"><span data-stu-id="b7f78-354">Type</span></span>    |<span data-ttu-id="b7f78-355">是否必需</span><span class="sxs-lookup"><span data-stu-id="b7f78-355">Required</span></span>|  <span data-ttu-id="b7f78-356">值</span><span class="sxs-lookup"><span data-stu-id="b7f78-356">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="b7f78-357">resourceId</span><span class="sxs-lookup"><span data-stu-id="b7f78-357">resourceId</span></span>|<span data-ttu-id="b7f78-358">String</span><span class="sxs-lookup"><span data-stu-id="b7f78-358">String</span></span>|<span data-ttu-id="b7f78-359">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-359">Yes</span></span>|<span data-ttu-id="b7f78-360">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="b7f78-360">\<resourceId\></span></span>|
|<span data-ttu-id="b7f78-361">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b7f78-361">roleDefinitionId</span></span>|<span data-ttu-id="b7f78-362">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-362">String</span></span>|<span data-ttu-id="b7f78-363">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-363">Yes</span></span>|<span data-ttu-id="b7f78-364">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="b7f78-364">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="b7f78-365">subjectId</span><span class="sxs-lookup"><span data-stu-id="b7f78-365">subjectId</span></span>|<span data-ttu-id="b7f78-366">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-366">String</span></span>|<span data-ttu-id="b7f78-367">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-367">Yes</span></span>|<span data-ttu-id="b7f78-368">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="b7f78-368">\<subjectId\></span></span>|
|<span data-ttu-id="b7f78-369">assignmentState</span><span class="sxs-lookup"><span data-stu-id="b7f78-369">assignmentState</span></span>|<span data-ttu-id="b7f78-370">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-370">String</span></span>|<span data-ttu-id="b7f78-371">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-371">Yes</span></span>| <span data-ttu-id="b7f78-372">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="b7f78-372">Eligible / Active</span></span>|
|<span data-ttu-id="b7f78-373">type</span><span class="sxs-lookup"><span data-stu-id="b7f78-373">type</span></span>|<span data-ttu-id="b7f78-374">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-374">String</span></span>|<span data-ttu-id="b7f78-375">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-375">Yes</span></span>| <span data-ttu-id="b7f78-376">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="b7f78-376">AdminUpdate</span></span>|
|<span data-ttu-id="b7f78-377">原因</span><span class="sxs-lookup"><span data-stu-id="b7f78-377">reason</span></span>|<span data-ttu-id="b7f78-378">String</span><span class="sxs-lookup"><span data-stu-id="b7f78-378">String</span></span>| <span data-ttu-id="b7f78-379">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="b7f78-379">depends on roleSettings</span></span>||
|<span data-ttu-id="b7f78-380">计划</span><span class="sxs-lookup"><span data-stu-id="b7f78-380">schedule</span></span>|[<span data-ttu-id="b7f78-381">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b7f78-381">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="b7f78-382">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-382">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="b7f78-383">请求</span><span class="sxs-lookup"><span data-stu-id="b7f78-383">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="b7f78-384">响应</span><span class="sxs-lookup"><span data-stu-id="b7f78-384">Response</span></span>
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

### <a name="example-6"></a><span data-ttu-id="b7f78-385">示例 6</span><span class="sxs-lookup"><span data-stu-id="b7f78-385">Example 6</span></span>
<span data-ttu-id="b7f78-386">本示例将用户 ANUJCUSER 即将过期的角色分配给 API 管理服务参与者。</span><span class="sxs-lookup"><span data-stu-id="b7f78-386">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="b7f78-387">**注意：** 另外还包括的权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="b7f78-387">**Note:** In additon to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="b7f78-388">属性</span><span class="sxs-lookup"><span data-stu-id="b7f78-388">Property</span></span>     | <span data-ttu-id="b7f78-389">类型</span><span class="sxs-lookup"><span data-stu-id="b7f78-389">Type</span></span>    |<span data-ttu-id="b7f78-390">是否必需</span><span class="sxs-lookup"><span data-stu-id="b7f78-390">Required</span></span>|  <span data-ttu-id="b7f78-391">值</span><span class="sxs-lookup"><span data-stu-id="b7f78-391">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="b7f78-392">resourceId</span><span class="sxs-lookup"><span data-stu-id="b7f78-392">resourceId</span></span>|<span data-ttu-id="b7f78-393">String</span><span class="sxs-lookup"><span data-stu-id="b7f78-393">String</span></span>|<span data-ttu-id="b7f78-394">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-394">Yes</span></span>|<span data-ttu-id="b7f78-395">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="b7f78-395">\<resourceId\></span></span>|
|<span data-ttu-id="b7f78-396">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b7f78-396">roleDefinitionId</span></span>|<span data-ttu-id="b7f78-397">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-397">String</span></span>|<span data-ttu-id="b7f78-398">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-398">Yes</span></span>|<span data-ttu-id="b7f78-399">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="b7f78-399">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="b7f78-400">subjectId</span><span class="sxs-lookup"><span data-stu-id="b7f78-400">subjectId</span></span>|<span data-ttu-id="b7f78-401">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-401">String</span></span>|<span data-ttu-id="b7f78-402">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-402">Yes</span></span>|<span data-ttu-id="b7f78-403">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="b7f78-403">\<subjectId\></span></span>|
|<span data-ttu-id="b7f78-404">assignmentState</span><span class="sxs-lookup"><span data-stu-id="b7f78-404">assignmentState</span></span>|<span data-ttu-id="b7f78-405">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-405">String</span></span>|<span data-ttu-id="b7f78-406">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-406">Yes</span></span>| <span data-ttu-id="b7f78-407">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="b7f78-407">Eligible / Active</span></span> |
|<span data-ttu-id="b7f78-408">type</span><span class="sxs-lookup"><span data-stu-id="b7f78-408">type</span></span>|<span data-ttu-id="b7f78-409">字符串</span><span class="sxs-lookup"><span data-stu-id="b7f78-409">String</span></span>|<span data-ttu-id="b7f78-410">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-410">Yes</span></span>| <span data-ttu-id="b7f78-411">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="b7f78-411">AdminExtend</span></span>|
|<span data-ttu-id="b7f78-412">原因</span><span class="sxs-lookup"><span data-stu-id="b7f78-412">reason</span></span>|<span data-ttu-id="b7f78-413">String</span><span class="sxs-lookup"><span data-stu-id="b7f78-413">String</span></span>| <span data-ttu-id="b7f78-414">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="b7f78-414">depends on roleSettings</span></span>||
|<span data-ttu-id="b7f78-415">计划</span><span class="sxs-lookup"><span data-stu-id="b7f78-415">schedule</span></span>|[<span data-ttu-id="b7f78-416">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b7f78-416">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="b7f78-417">是</span><span class="sxs-lookup"><span data-stu-id="b7f78-417">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="b7f78-418">请求</span><span class="sxs-lookup"><span data-stu-id="b7f78-418">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="b7f78-419">响应</span><span class="sxs-lookup"><span data-stu-id="b7f78-419">Response</span></span>
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
