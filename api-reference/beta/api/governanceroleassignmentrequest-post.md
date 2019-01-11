---
title: 创建 governanceRoleAssignmentRequest
description: 创建角色分配请求以表示该操作所需角色分配。 下表列出的操作。
localization_priority: Normal
ms.openlocfilehash: 09adb824147dba745649efc7589ca763f815278d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823770"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="8acb8-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8acb8-104">Create governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="8acb8-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8acb8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8acb8-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8acb8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8acb8-107">创建角色分配请求以表示该操作所需角色分配。</span><span class="sxs-lookup"><span data-stu-id="8acb8-107">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="8acb8-108">下表列出的操作。</span><span class="sxs-lookup"><span data-stu-id="8acb8-108">The following table lists the operations.</span></span>

| <span data-ttu-id="8acb8-109">操作</span><span class="sxs-lookup"><span data-stu-id="8acb8-109">Operation</span></span>       | <span data-ttu-id="8acb8-110">类型</span><span class="sxs-lookup"><span data-stu-id="8acb8-110">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="8acb8-111">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="8acb8-111">Assign a role assignment</span></span>| <span data-ttu-id="8acb8-112">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="8acb8-112">AdminAdd</span></span> |
| <span data-ttu-id="8acb8-113">激活合格的角色分配</span><span class="sxs-lookup"><span data-stu-id="8acb8-113">Activate an eligible role assignment</span></span>| <span data-ttu-id="8acb8-114">UserAdd</span><span class="sxs-lookup"><span data-stu-id="8acb8-114">UserAdd</span></span> | 
| <span data-ttu-id="8acb8-115">停用已激活的角色分配</span><span class="sxs-lookup"><span data-stu-id="8acb8-115">Deactivate an activated role assignment</span></span>| <span data-ttu-id="8acb8-116">UserRemove</span><span class="sxs-lookup"><span data-stu-id="8acb8-116">UserRemove</span></span> | 
| <span data-ttu-id="8acb8-117">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="8acb8-117">Remove a role assignment</span></span>| <span data-ttu-id="8acb8-118">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="8acb8-118">AdminRemove</span></span> |
| <span data-ttu-id="8acb8-119">更新一个角色分配</span><span class="sxs-lookup"><span data-stu-id="8acb8-119">Update a role assignment</span></span>| <span data-ttu-id="8acb8-120">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="8acb8-120">AdminUpdate</span></span> |
| <span data-ttu-id="8acb8-121">请求扩展我角色分配</span><span class="sxs-lookup"><span data-stu-id="8acb8-121">Request to extend my role assignment</span></span>| <span data-ttu-id="8acb8-122">UserExtend</span><span class="sxs-lookup"><span data-stu-id="8acb8-122">UserExtend</span></span> | 
| <span data-ttu-id="8acb8-123">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="8acb8-123">Extend a role assignment</span></span>| <span data-ttu-id="8acb8-124">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="8acb8-124">AdminExtend</span></span> | 
| <span data-ttu-id="8acb8-125">请求续订我过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="8acb8-125">Request to renew my expired role assignment</span></span>| <span data-ttu-id="8acb8-126">UserRenew</span><span class="sxs-lookup"><span data-stu-id="8acb8-126">UserRenew</span></span> | 
| <span data-ttu-id="8acb8-127">续订已过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="8acb8-127">Renew an expired role assignment</span></span>| <span data-ttu-id="8acb8-128">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="8acb8-128">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="8acb8-129">权限</span><span class="sxs-lookup"><span data-stu-id="8acb8-129">Permissions</span></span>
<span data-ttu-id="8acb8-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8acb8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8acb8-132">权限类型</span><span class="sxs-lookup"><span data-stu-id="8acb8-132">Permission type</span></span>      | <span data-ttu-id="8acb8-133">Permissions</span><span class="sxs-lookup"><span data-stu-id="8acb8-133">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8acb8-134">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8acb8-134">Delegated (work or school account)</span></span> | <span data-ttu-id="8acb8-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="8acb8-135">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="8acb8-136">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8acb8-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8acb8-137">不支持。</span><span class="sxs-lookup"><span data-stu-id="8acb8-137">Not supported.</span></span>    |
|<span data-ttu-id="8acb8-138">应用程序</span><span class="sxs-lookup"><span data-stu-id="8acb8-138">Application</span></span> | <span data-ttu-id="8acb8-139">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="8acb8-139">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="8acb8-140">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8acb8-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="8acb8-141">请求标头</span><span class="sxs-lookup"><span data-stu-id="8acb8-141">Request headers</span></span>
| <span data-ttu-id="8acb8-142">名称</span><span class="sxs-lookup"><span data-stu-id="8acb8-142">Name</span></span>       | <span data-ttu-id="8acb8-143">说明</span><span class="sxs-lookup"><span data-stu-id="8acb8-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8acb8-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="8acb8-144">Authorization</span></span>  | <span data-ttu-id="8acb8-145">持有者 {code}</span><span class="sxs-lookup"><span data-stu-id="8acb8-145">Bearer {code}</span></span>|
| <span data-ttu-id="8acb8-146">Content-type</span><span class="sxs-lookup"><span data-stu-id="8acb8-146">Content-type</span></span>  | <span data-ttu-id="8acb8-147">application/json</span><span class="sxs-lookup"><span data-stu-id="8acb8-147">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8acb8-148">请求正文</span><span class="sxs-lookup"><span data-stu-id="8acb8-148">Request body</span></span>
<span data-ttu-id="8acb8-149">在请求正文中，提供[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8acb8-149">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="8acb8-150">属性</span><span class="sxs-lookup"><span data-stu-id="8acb8-150">Property</span></span>     | <span data-ttu-id="8acb8-151">类型</span><span class="sxs-lookup"><span data-stu-id="8acb8-151">Type</span></span>    |<span data-ttu-id="8acb8-152">是否必需</span><span class="sxs-lookup"><span data-stu-id="8acb8-152">Required</span></span>|  <span data-ttu-id="8acb8-153">Description</span><span class="sxs-lookup"><span data-stu-id="8acb8-153">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="8acb8-154">resourceId</span><span class="sxs-lookup"><span data-stu-id="8acb8-154">resourceId</span></span>|<span data-ttu-id="8acb8-155">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-155">String</span></span>|<span data-ttu-id="8acb8-156">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-156">Yes</span></span>|<span data-ttu-id="8acb8-157">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="8acb8-157">The ID of the resource.</span></span>|
|<span data-ttu-id="8acb8-158">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8acb8-158">roleDefinitionId</span></span>|<span data-ttu-id="8acb8-159">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-159">String</span></span>|<span data-ttu-id="8acb8-160">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-160">Yes</span></span>|<span data-ttu-id="8acb8-161">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="8acb8-161">The ID of the role definition.</span></span>|
|<span data-ttu-id="8acb8-162">subjectId</span><span class="sxs-lookup"><span data-stu-id="8acb8-162">subjectId</span></span>|<span data-ttu-id="8acb8-163">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-163">String</span></span>|<span data-ttu-id="8acb8-164">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-164">Yes</span></span>|<span data-ttu-id="8acb8-165">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="8acb8-165">The ID of the subject.</span></span>|
|<span data-ttu-id="8acb8-166">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8acb8-166">assignmentState</span></span>|<span data-ttu-id="8acb8-167">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-167">String</span></span>|<span data-ttu-id="8acb8-168">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-168">Yes</span></span>|<span data-ttu-id="8acb8-169">工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="8acb8-169">The state of assignment.</span></span> <span data-ttu-id="8acb8-170">值可以是``Eligible``和``Active``。</span><span class="sxs-lookup"><span data-stu-id="8acb8-170">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="8acb8-171">type</span><span class="sxs-lookup"><span data-stu-id="8acb8-171">type</span></span>|<span data-ttu-id="8acb8-172">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-172">String</span></span>|<span data-ttu-id="8acb8-173">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-173">Yes</span></span>|<span data-ttu-id="8acb8-174">请求类型。</span><span class="sxs-lookup"><span data-stu-id="8acb8-174">The request type.</span></span> <span data-ttu-id="8acb8-175">值可以是`AdminAdd`， `UserAdd`， `AdminUpdate`， `AdminRemove`， `UserRemove`， `UserExtend`， `UserRenew`，`AdminRenew`和`AdminExtend`。</span><span class="sxs-lookup"><span data-stu-id="8acb8-175">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="8acb8-176">原因</span><span class="sxs-lookup"><span data-stu-id="8acb8-176">reason</span></span>|<span data-ttu-id="8acb8-177">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-177">String</span></span>| |<span data-ttu-id="8acb8-178">原因需要提供角色分配请求的审核和查看用途。</span><span class="sxs-lookup"><span data-stu-id="8acb8-178">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="8acb8-179">计划</span><span class="sxs-lookup"><span data-stu-id="8acb8-179">schedule</span></span>|[<span data-ttu-id="8acb8-180">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8acb8-180">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="8acb8-181">角色分配请求的时间表。</span><span class="sxs-lookup"><span data-stu-id="8acb8-181">The schedule of the role assignment request.</span></span> <span data-ttu-id="8acb8-182">请求类型的`UserAdd`， `AdminAdd`， `AdminUpdate`，和`AdminExtend`，需要。</span><span class="sxs-lookup"><span data-stu-id="8acb8-182">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

## <a name="response"></a><span data-ttu-id="8acb8-183">响应</span><span class="sxs-lookup"><span data-stu-id="8acb8-183">Response</span></span>
<span data-ttu-id="8acb8-184">如果成功，此方法返回`201 Created`响应代码和响应正文中的[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8acb8-184">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="8acb8-185">错误代码</span><span class="sxs-lookup"><span data-stu-id="8acb8-185">Error codes</span></span>
<span data-ttu-id="8acb8-186">此 API 返回的标准 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="8acb8-186">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="8acb8-187">此外，它也会返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="8acb8-187">In addition, it also returns the error codes listed in the following table.</span></span>

|<span data-ttu-id="8acb8-188">错误代码</span><span class="sxs-lookup"><span data-stu-id="8acb8-188">Error code</span></span>     | <span data-ttu-id="8acb8-189">错误消息</span><span class="sxs-lookup"><span data-stu-id="8acb8-189">Error message</span></span>              | <span data-ttu-id="8acb8-190">详细信息</span><span class="sxs-lookup"><span data-stu-id="8acb8-190">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="8acb8-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8acb8-191">400 BadRequest</span></span> | <span data-ttu-id="8acb8-192">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="8acb8-192">RoleNotFound</span></span>    | <span data-ttu-id="8acb8-193">`roleDefinitionId`提供在请求正文找不到。</span><span class="sxs-lookup"><span data-stu-id="8acb8-193">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="8acb8-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8acb8-194">400 BadRequest</span></span> | <span data-ttu-id="8acb8-195">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="8acb8-195">ResourceIsLocked</span></span>    | <span data-ttu-id="8acb8-196">在请求正文中提供的资源处于状态的`Locked`和无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="8acb8-196">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="8acb8-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8acb8-197">400 BadRequest</span></span> | <span data-ttu-id="8acb8-198">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="8acb8-198">SubjectNotFound</span></span>    | <span data-ttu-id="8acb8-199">`subjectId`提供在请求正文找不到。</span><span class="sxs-lookup"><span data-stu-id="8acb8-199">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="8acb8-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8acb8-200">400 BadRequest</span></span> | <span data-ttu-id="8acb8-201">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8acb8-201">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="8acb8-202">已存在挂起[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)系统中。</span><span class="sxs-lookup"><span data-stu-id="8acb8-202">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="8acb8-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8acb8-203">400 BadRequest</span></span> | <span data-ttu-id="8acb8-204">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="8acb8-204">RoleAssignmentExists</span></span>    | <span data-ttu-id="8acb8-205">系统中存在[governanceRoleAssignment](../resources/governanceroleassignment.md)请求已创建。</span><span class="sxs-lookup"><span data-stu-id="8acb8-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="8acb8-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8acb8-206">400 BadRequest</span></span> | <span data-ttu-id="8acb8-207">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="8acb8-207">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="8acb8-208">系统中不存在[governanceRoleAssignment](../resources/governanceroleassignment.md)请求来更新/扩展。</span><span class="sxs-lookup"><span data-stu-id="8acb8-208">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="8acb8-209">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8acb8-209">400 BadRequest</span></span> | <span data-ttu-id="8acb8-210">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="8acb8-210">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="8acb8-211">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部的策略，且无法创建。</span><span class="sxs-lookup"><span data-stu-id="8acb8-211">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="examples"></a><span data-ttu-id="8acb8-212">示例</span><span class="sxs-lookup"><span data-stu-id="8acb8-212">Examples</span></span>
<span data-ttu-id="8acb8-213">下面的示例演示如何使用此 API。</span><span class="sxs-lookup"><span data-stu-id="8acb8-213">The following examples show how to use this API.</span></span>

### <a name="example-1"></a><span data-ttu-id="8acb8-214">示例 1</span><span class="sxs-lookup"><span data-stu-id="8acb8-214">Example 1</span></span>
<span data-ttu-id="8acb8-215">本示例中，管理员为帐单读者角色分配用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="8acb8-215">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="8acb8-216">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="8acb8-216">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="8acb8-217">属性</span><span class="sxs-lookup"><span data-stu-id="8acb8-217">Property</span></span>     | <span data-ttu-id="8acb8-218">类型</span><span class="sxs-lookup"><span data-stu-id="8acb8-218">Type</span></span>    |<span data-ttu-id="8acb8-219">是否必需</span><span class="sxs-lookup"><span data-stu-id="8acb8-219">Required</span></span>|  <span data-ttu-id="8acb8-220">值</span><span class="sxs-lookup"><span data-stu-id="8acb8-220">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="8acb8-221">resourceId</span><span class="sxs-lookup"><span data-stu-id="8acb8-221">resourceId</span></span>|<span data-ttu-id="8acb8-222">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-222">String</span></span>|<span data-ttu-id="8acb8-223">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-223">Yes</span></span>|<span data-ttu-id="8acb8-224">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="8acb8-224">\<resourceId\></span></span>|
|<span data-ttu-id="8acb8-225">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8acb8-225">roleDefinitionId</span></span>|<span data-ttu-id="8acb8-226">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-226">String</span></span>|<span data-ttu-id="8acb8-227">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-227">Yes</span></span>|<span data-ttu-id="8acb8-228">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="8acb8-228">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="8acb8-229">subjectId</span><span class="sxs-lookup"><span data-stu-id="8acb8-229">subjectId</span></span>|<span data-ttu-id="8acb8-230">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-230">String</span></span>|<span data-ttu-id="8acb8-231">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-231">Yes</span></span>|<span data-ttu-id="8acb8-232">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="8acb8-232">\<subjectId\></span></span>|
|<span data-ttu-id="8acb8-233">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8acb8-233">assignmentState</span></span>|<span data-ttu-id="8acb8-234">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-234">String</span></span>|<span data-ttu-id="8acb8-235">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-235">Yes</span></span>| <span data-ttu-id="8acb8-236">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="8acb8-236">Eligible / Active</span></span>|
|<span data-ttu-id="8acb8-237">type</span><span class="sxs-lookup"><span data-stu-id="8acb8-237">type</span></span>|<span data-ttu-id="8acb8-238">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-238">String</span></span>|<span data-ttu-id="8acb8-239">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-239">Yes</span></span>| <span data-ttu-id="8acb8-240">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="8acb8-240">AdminAdd</span></span>|
|<span data-ttu-id="8acb8-241">原因</span><span class="sxs-lookup"><span data-stu-id="8acb8-241">reason</span></span>|<span data-ttu-id="8acb8-242">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-242">String</span></span>| <span data-ttu-id="8acb8-243">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="8acb8-243">depends on role Settings</span></span>||
|<span data-ttu-id="8acb8-244">计划</span><span class="sxs-lookup"><span data-stu-id="8acb8-244">schedule</span></span>|[<span data-ttu-id="8acb8-245">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8acb8-245">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="8acb8-246">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-246">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="8acb8-247">请求</span><span class="sxs-lookup"><span data-stu-id="8acb8-247">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="8acb8-248">响应</span><span class="sxs-lookup"><span data-stu-id="8acb8-248">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="8acb8-249">示例 2</span><span class="sxs-lookup"><span data-stu-id="8acb8-249">Example 2</span></span>
<span data-ttu-id="8acb8-250">本示例中，用户 nawu@fimdev.net 激活合格的帐单读取器角色。</span><span class="sxs-lookup"><span data-stu-id="8acb8-250">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="8acb8-251">属性</span><span class="sxs-lookup"><span data-stu-id="8acb8-251">Property</span></span>     | <span data-ttu-id="8acb8-252">类型</span><span class="sxs-lookup"><span data-stu-id="8acb8-252">Type</span></span>    |<span data-ttu-id="8acb8-253">是否必需</span><span class="sxs-lookup"><span data-stu-id="8acb8-253">Required</span></span>|  <span data-ttu-id="8acb8-254">值</span><span class="sxs-lookup"><span data-stu-id="8acb8-254">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="8acb8-255">resourceId</span><span class="sxs-lookup"><span data-stu-id="8acb8-255">resourceId</span></span>|<span data-ttu-id="8acb8-256">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-256">String</span></span>|<span data-ttu-id="8acb8-257">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-257">Yes</span></span>|<span data-ttu-id="8acb8-258">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="8acb8-258">\<resourceId\></span></span>|
|<span data-ttu-id="8acb8-259">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8acb8-259">roleDefinitionId</span></span>|<span data-ttu-id="8acb8-260">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-260">String</span></span>|<span data-ttu-id="8acb8-261">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-261">Yes</span></span>|<span data-ttu-id="8acb8-262">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="8acb8-262">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="8acb8-263">subjectId</span><span class="sxs-lookup"><span data-stu-id="8acb8-263">subjectId</span></span>|<span data-ttu-id="8acb8-264">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-264">String</span></span>|<span data-ttu-id="8acb8-265">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-265">Yes</span></span>|<span data-ttu-id="8acb8-266">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="8acb8-266">\<subjectId\></span></span>|
|<span data-ttu-id="8acb8-267">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8acb8-267">assignmentState</span></span>|<span data-ttu-id="8acb8-268">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-268">String</span></span>|<span data-ttu-id="8acb8-269">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-269">Yes</span></span>| <span data-ttu-id="8acb8-270">活动</span><span class="sxs-lookup"><span data-stu-id="8acb8-270">Active</span></span>|
|<span data-ttu-id="8acb8-271">type</span><span class="sxs-lookup"><span data-stu-id="8acb8-271">type</span></span>|<span data-ttu-id="8acb8-272">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-272">String</span></span>|<span data-ttu-id="8acb8-273">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-273">Yes</span></span>| <span data-ttu-id="8acb8-274">UserAdd</span><span class="sxs-lookup"><span data-stu-id="8acb8-274">UserAdd</span></span>|
|<span data-ttu-id="8acb8-275">原因</span><span class="sxs-lookup"><span data-stu-id="8acb8-275">reason</span></span>|<span data-ttu-id="8acb8-276">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-276">String</span></span>| <span data-ttu-id="8acb8-277">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="8acb8-277">depends on role Settings</span></span>||
|<span data-ttu-id="8acb8-278">计划</span><span class="sxs-lookup"><span data-stu-id="8acb8-278">schedule</span></span>|[<span data-ttu-id="8acb8-279">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8acb8-279">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="8acb8-280">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-280">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="8acb8-281">请求</span><span class="sxs-lookup"><span data-stu-id="8acb8-281">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="8acb8-282">响应</span><span class="sxs-lookup"><span data-stu-id="8acb8-282">Response</span></span>
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

### <a name="example-3"></a><span data-ttu-id="8acb8-283">示例 3</span><span class="sxs-lookup"><span data-stu-id="8acb8-283">Example 3</span></span>
<span data-ttu-id="8acb8-284">本示例中，用户 nawu@fimdev.net 停用活动的帐单读取器角色。</span><span class="sxs-lookup"><span data-stu-id="8acb8-284">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="8acb8-285">属性</span><span class="sxs-lookup"><span data-stu-id="8acb8-285">Property</span></span>     | <span data-ttu-id="8acb8-286">类型</span><span class="sxs-lookup"><span data-stu-id="8acb8-286">Type</span></span>    |<span data-ttu-id="8acb8-287">是否必需</span><span class="sxs-lookup"><span data-stu-id="8acb8-287">Required</span></span>|  <span data-ttu-id="8acb8-288">值</span><span class="sxs-lookup"><span data-stu-id="8acb8-288">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="8acb8-289">resourceId</span><span class="sxs-lookup"><span data-stu-id="8acb8-289">resourceId</span></span>|<span data-ttu-id="8acb8-290">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-290">String</span></span>|<span data-ttu-id="8acb8-291">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-291">Yes</span></span>|<span data-ttu-id="8acb8-292">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="8acb8-292">\<resourceId\></span></span>|
|<span data-ttu-id="8acb8-293">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8acb8-293">roleDefinitionId</span></span>|<span data-ttu-id="8acb8-294">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-294">String</span></span>|<span data-ttu-id="8acb8-295">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-295">Yes</span></span>|<span data-ttu-id="8acb8-296">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="8acb8-296">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="8acb8-297">subjectId</span><span class="sxs-lookup"><span data-stu-id="8acb8-297">subjectId</span></span>|<span data-ttu-id="8acb8-298">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-298">String</span></span>|<span data-ttu-id="8acb8-299">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-299">Yes</span></span>|<span data-ttu-id="8acb8-300">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="8acb8-300">\<subjectId\></span></span>|
|<span data-ttu-id="8acb8-301">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8acb8-301">assignmentState</span></span>|<span data-ttu-id="8acb8-302">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-302">String</span></span>|<span data-ttu-id="8acb8-303">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-303">Yes</span></span>| <span data-ttu-id="8acb8-304">活动</span><span class="sxs-lookup"><span data-stu-id="8acb8-304">Active</span></span>|
|<span data-ttu-id="8acb8-305">type</span><span class="sxs-lookup"><span data-stu-id="8acb8-305">type</span></span>|<span data-ttu-id="8acb8-306">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-306">String</span></span>|<span data-ttu-id="8acb8-307">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-307">Yes</span></span>| <span data-ttu-id="8acb8-308">UserRemove</span><span class="sxs-lookup"><span data-stu-id="8acb8-308">UserRemove</span></span>|
|<span data-ttu-id="8acb8-309">原因</span><span class="sxs-lookup"><span data-stu-id="8acb8-309">reason</span></span>|<span data-ttu-id="8acb8-310">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-310">String</span></span>| <span data-ttu-id="8acb8-311">否</span><span class="sxs-lookup"><span data-stu-id="8acb8-311">No</span></span>||
|<span data-ttu-id="8acb8-312">计划</span><span class="sxs-lookup"><span data-stu-id="8acb8-312">schedule</span></span>|[<span data-ttu-id="8acb8-313">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8acb8-313">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="8acb8-314">否</span><span class="sxs-lookup"><span data-stu-id="8acb8-314">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="8acb8-315">请求</span><span class="sxs-lookup"><span data-stu-id="8acb8-315">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="8acb8-316">响应</span><span class="sxs-lookup"><span data-stu-id="8acb8-316">Response</span></span>
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

### <a name="example-4"></a><span data-ttu-id="8acb8-317">示例 4</span><span class="sxs-lookup"><span data-stu-id="8acb8-317">Example 4</span></span>
<span data-ttu-id="8acb8-318">本示例中，管理员从帐单读者角色中移除用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="8acb8-318">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="8acb8-319">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="8acb8-319">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="8acb8-320">属性</span><span class="sxs-lookup"><span data-stu-id="8acb8-320">Property</span></span>     | <span data-ttu-id="8acb8-321">类型</span><span class="sxs-lookup"><span data-stu-id="8acb8-321">Type</span></span>    |<span data-ttu-id="8acb8-322">是否必需</span><span class="sxs-lookup"><span data-stu-id="8acb8-322">Required</span></span>|  <span data-ttu-id="8acb8-323">值</span><span class="sxs-lookup"><span data-stu-id="8acb8-323">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="8acb8-324">resourceId</span><span class="sxs-lookup"><span data-stu-id="8acb8-324">resourceId</span></span>|<span data-ttu-id="8acb8-325">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-325">String</span></span>|<span data-ttu-id="8acb8-326">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-326">Yes</span></span>|<span data-ttu-id="8acb8-327">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="8acb8-327">\<resourceId\></span></span>|
|<span data-ttu-id="8acb8-328">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8acb8-328">roleDefinitionId</span></span>|<span data-ttu-id="8acb8-329">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-329">String</span></span>|<span data-ttu-id="8acb8-330">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-330">Yes</span></span>|<span data-ttu-id="8acb8-331">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="8acb8-331">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="8acb8-332">subjectId</span><span class="sxs-lookup"><span data-stu-id="8acb8-332">subjectId</span></span>|<span data-ttu-id="8acb8-333">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-333">String</span></span>|<span data-ttu-id="8acb8-334">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-334">Yes</span></span>|<span data-ttu-id="8acb8-335">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="8acb8-335">\<subjectId\></span></span>|
|<span data-ttu-id="8acb8-336">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8acb8-336">assignmentState</span></span>|<span data-ttu-id="8acb8-337">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-337">String</span></span>|<span data-ttu-id="8acb8-338">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-338">Yes</span></span>| <span data-ttu-id="8acb8-339">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="8acb8-339">Eligible / Active</span></span>|
|<span data-ttu-id="8acb8-340">type</span><span class="sxs-lookup"><span data-stu-id="8acb8-340">type</span></span>|<span data-ttu-id="8acb8-341">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-341">String</span></span>|<span data-ttu-id="8acb8-342">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-342">Yes</span></span>| <span data-ttu-id="8acb8-343">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="8acb8-343">AdminRemove</span></span>|
|<span data-ttu-id="8acb8-344">原因</span><span class="sxs-lookup"><span data-stu-id="8acb8-344">reason</span></span>|<span data-ttu-id="8acb8-345">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-345">String</span></span>| <span data-ttu-id="8acb8-346">否</span><span class="sxs-lookup"><span data-stu-id="8acb8-346">No</span></span>||
|<span data-ttu-id="8acb8-347">计划</span><span class="sxs-lookup"><span data-stu-id="8acb8-347">schedule</span></span>|[<span data-ttu-id="8acb8-348">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8acb8-348">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="8acb8-349">否</span><span class="sxs-lookup"><span data-stu-id="8acb8-349">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="8acb8-350">请求</span><span class="sxs-lookup"><span data-stu-id="8acb8-350">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="8acb8-351">响应</span><span class="sxs-lookup"><span data-stu-id="8acb8-351">Response</span></span>
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

### <a name="example-5"></a><span data-ttu-id="8acb8-352">示例 5</span><span class="sxs-lookup"><span data-stu-id="8acb8-352">Example 5</span></span>
<span data-ttu-id="8acb8-353">本示例中，管理员向所有者更新用户 nawu@fimdev.net 的角色分配。</span><span class="sxs-lookup"><span data-stu-id="8acb8-353">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="8acb8-354">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="8acb8-354">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="8acb8-355">属性</span><span class="sxs-lookup"><span data-stu-id="8acb8-355">Property</span></span>     | <span data-ttu-id="8acb8-356">类型</span><span class="sxs-lookup"><span data-stu-id="8acb8-356">Type</span></span>    |<span data-ttu-id="8acb8-357">是否必需</span><span class="sxs-lookup"><span data-stu-id="8acb8-357">Required</span></span>|  <span data-ttu-id="8acb8-358">值</span><span class="sxs-lookup"><span data-stu-id="8acb8-358">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="8acb8-359">resourceId</span><span class="sxs-lookup"><span data-stu-id="8acb8-359">resourceId</span></span>|<span data-ttu-id="8acb8-360">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-360">String</span></span>|<span data-ttu-id="8acb8-361">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-361">Yes</span></span>|<span data-ttu-id="8acb8-362">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="8acb8-362">\<resourceId\></span></span>|
|<span data-ttu-id="8acb8-363">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8acb8-363">roleDefinitionId</span></span>|<span data-ttu-id="8acb8-364">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-364">String</span></span>|<span data-ttu-id="8acb8-365">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-365">Yes</span></span>|<span data-ttu-id="8acb8-366">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="8acb8-366">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="8acb8-367">subjectId</span><span class="sxs-lookup"><span data-stu-id="8acb8-367">subjectId</span></span>|<span data-ttu-id="8acb8-368">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-368">String</span></span>|<span data-ttu-id="8acb8-369">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-369">Yes</span></span>|<span data-ttu-id="8acb8-370">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="8acb8-370">\<subjectId\></span></span>|
|<span data-ttu-id="8acb8-371">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8acb8-371">assignmentState</span></span>|<span data-ttu-id="8acb8-372">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-372">String</span></span>|<span data-ttu-id="8acb8-373">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-373">Yes</span></span>| <span data-ttu-id="8acb8-374">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="8acb8-374">Eligible / Active</span></span>|
|<span data-ttu-id="8acb8-375">type</span><span class="sxs-lookup"><span data-stu-id="8acb8-375">type</span></span>|<span data-ttu-id="8acb8-376">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-376">String</span></span>|<span data-ttu-id="8acb8-377">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-377">Yes</span></span>| <span data-ttu-id="8acb8-378">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="8acb8-378">AdminUpdate</span></span>|
|<span data-ttu-id="8acb8-379">原因</span><span class="sxs-lookup"><span data-stu-id="8acb8-379">reason</span></span>|<span data-ttu-id="8acb8-380">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-380">String</span></span>| <span data-ttu-id="8acb8-381">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="8acb8-381">depends on roleSettings</span></span>||
|<span data-ttu-id="8acb8-382">计划</span><span class="sxs-lookup"><span data-stu-id="8acb8-382">schedule</span></span>|[<span data-ttu-id="8acb8-383">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8acb8-383">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="8acb8-384">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-384">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="8acb8-385">请求</span><span class="sxs-lookup"><span data-stu-id="8acb8-385">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="8acb8-386">响应</span><span class="sxs-lookup"><span data-stu-id="8acb8-386">Response</span></span>
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

### <a name="example-6"></a><span data-ttu-id="8acb8-387">示例 6</span><span class="sxs-lookup"><span data-stu-id="8acb8-387">Example 6</span></span>
<span data-ttu-id="8acb8-388">本示例将用户 ANUJCUSER 即将过期的角色分配给 API 管理服务参与者。</span><span class="sxs-lookup"><span data-stu-id="8acb8-388">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="8acb8-389">**注意：** 另外还包括的权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="8acb8-389">**Note:** In additon to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="8acb8-390">属性</span><span class="sxs-lookup"><span data-stu-id="8acb8-390">Property</span></span>     | <span data-ttu-id="8acb8-391">类型</span><span class="sxs-lookup"><span data-stu-id="8acb8-391">Type</span></span>    |<span data-ttu-id="8acb8-392">是否必需</span><span class="sxs-lookup"><span data-stu-id="8acb8-392">Required</span></span>|  <span data-ttu-id="8acb8-393">值</span><span class="sxs-lookup"><span data-stu-id="8acb8-393">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="8acb8-394">resourceId</span><span class="sxs-lookup"><span data-stu-id="8acb8-394">resourceId</span></span>|<span data-ttu-id="8acb8-395">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-395">String</span></span>|<span data-ttu-id="8acb8-396">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-396">Yes</span></span>|<span data-ttu-id="8acb8-397">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="8acb8-397">\<resourceId\></span></span>|
|<span data-ttu-id="8acb8-398">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8acb8-398">roleDefinitionId</span></span>|<span data-ttu-id="8acb8-399">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-399">String</span></span>|<span data-ttu-id="8acb8-400">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-400">Yes</span></span>|<span data-ttu-id="8acb8-401">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="8acb8-401">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="8acb8-402">subjectId</span><span class="sxs-lookup"><span data-stu-id="8acb8-402">subjectId</span></span>|<span data-ttu-id="8acb8-403">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-403">String</span></span>|<span data-ttu-id="8acb8-404">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-404">Yes</span></span>|<span data-ttu-id="8acb8-405">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="8acb8-405">\<subjectId\></span></span>|
|<span data-ttu-id="8acb8-406">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8acb8-406">assignmentState</span></span>|<span data-ttu-id="8acb8-407">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-407">String</span></span>|<span data-ttu-id="8acb8-408">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-408">Yes</span></span>| <span data-ttu-id="8acb8-409">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="8acb8-409">Eligible / Active</span></span> |
|<span data-ttu-id="8acb8-410">type</span><span class="sxs-lookup"><span data-stu-id="8acb8-410">type</span></span>|<span data-ttu-id="8acb8-411">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-411">String</span></span>|<span data-ttu-id="8acb8-412">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-412">Yes</span></span>| <span data-ttu-id="8acb8-413">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="8acb8-413">AdminExtend</span></span>|
|<span data-ttu-id="8acb8-414">原因</span><span class="sxs-lookup"><span data-stu-id="8acb8-414">reason</span></span>|<span data-ttu-id="8acb8-415">字符串</span><span class="sxs-lookup"><span data-stu-id="8acb8-415">String</span></span>| <span data-ttu-id="8acb8-416">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="8acb8-416">depends on roleSettings</span></span>||
|<span data-ttu-id="8acb8-417">计划</span><span class="sxs-lookup"><span data-stu-id="8acb8-417">schedule</span></span>|[<span data-ttu-id="8acb8-418">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8acb8-418">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="8acb8-419">是</span><span class="sxs-lookup"><span data-stu-id="8acb8-419">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="8acb8-420">请求</span><span class="sxs-lookup"><span data-stu-id="8acb8-420">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="8acb8-421">响应</span><span class="sxs-lookup"><span data-stu-id="8acb8-421">Response</span></span>
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
