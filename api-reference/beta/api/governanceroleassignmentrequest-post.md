---
title: 创建 governanceRoleAssignmentRequest
description: 创建角色分配请求以表示该操作所需角色分配。 下表列出的操作。
localization_priority: Normal
ms.openlocfilehash: 104ab1a0d4909bc2181df70bc4fc895fc4558260
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967219"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="e5607-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="e5607-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5607-105">创建角色分配请求以表示该操作所需角色分配。</span><span class="sxs-lookup"><span data-stu-id="e5607-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="e5607-106">下表列出的操作。</span><span class="sxs-lookup"><span data-stu-id="e5607-106">The following table lists the operations.</span></span>

| <span data-ttu-id="e5607-107">Operation</span><span class="sxs-lookup"><span data-stu-id="e5607-107">Operation</span></span>                                   | <span data-ttu-id="e5607-108">Type</span><span class="sxs-lookup"><span data-stu-id="e5607-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="e5607-109">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="e5607-109">Assign a role assignment</span></span>                    | <span data-ttu-id="e5607-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="e5607-110">AdminAdd</span></span>    |
| <span data-ttu-id="e5607-111">激活合格的角色分配</span><span class="sxs-lookup"><span data-stu-id="e5607-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="e5607-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="e5607-112">UserAdd</span></span>     |
| <span data-ttu-id="e5607-113">停用已激活的角色分配</span><span class="sxs-lookup"><span data-stu-id="e5607-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="e5607-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="e5607-114">UserRemove</span></span>  |
| <span data-ttu-id="e5607-115">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="e5607-115">Remove a role assignment</span></span>                    | <span data-ttu-id="e5607-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="e5607-116">AdminRemove</span></span> |
| <span data-ttu-id="e5607-117">更新一个角色分配</span><span class="sxs-lookup"><span data-stu-id="e5607-117">Update a role assignment</span></span>                    | <span data-ttu-id="e5607-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="e5607-118">AdminUpdate</span></span> |
| <span data-ttu-id="e5607-119">请求扩展我角色分配</span><span class="sxs-lookup"><span data-stu-id="e5607-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="e5607-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="e5607-120">UserExtend</span></span>  |
| <span data-ttu-id="e5607-121">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="e5607-121">Extend a role assignment</span></span>                    | <span data-ttu-id="e5607-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="e5607-122">AdminExtend</span></span> |
| <span data-ttu-id="e5607-123">请求续订我过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="e5607-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="e5607-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="e5607-124">UserRenew</span></span>   |
| <span data-ttu-id="e5607-125">续订已过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="e5607-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="e5607-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="e5607-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="e5607-127">权限</span><span class="sxs-lookup"><span data-stu-id="e5607-127">Permissions</span></span>

<span data-ttu-id="e5607-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5607-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e5607-130">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5607-130">Permission type</span></span>                        | <span data-ttu-id="e5607-131">权限</span><span class="sxs-lookup"><span data-stu-id="e5607-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="e5607-132">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5607-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5607-133">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e5607-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="e5607-134">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5607-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5607-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5607-135">Not supported.</span></span>                            |
| <span data-ttu-id="e5607-136">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5607-136">Application</span></span>                            | <span data-ttu-id="e5607-137">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e5607-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5607-138">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5607-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="e5607-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5607-139">Request headers</span></span>

| <span data-ttu-id="e5607-140">Name</span><span class="sxs-lookup"><span data-stu-id="e5607-140">Name</span></span>          | <span data-ttu-id="e5607-141">说明</span><span class="sxs-lookup"><span data-stu-id="e5607-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="e5607-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5607-142">Authorization</span></span> | <span data-ttu-id="e5607-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e5607-143">Bearer {code}</span></span>    |
| <span data-ttu-id="e5607-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="e5607-144">Content-type</span></span>  | <span data-ttu-id="e5607-145">application/json</span><span class="sxs-lookup"><span data-stu-id="e5607-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5607-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5607-146">Request body</span></span>

<span data-ttu-id="e5607-147">在请求正文中，提供[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5607-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="e5607-148">属性</span><span class="sxs-lookup"><span data-stu-id="e5607-148">Property</span></span>         | <span data-ttu-id="e5607-149">类型</span><span class="sxs-lookup"><span data-stu-id="e5607-149">Type</span></span>                                                     | <span data-ttu-id="e5607-150">说明</span><span class="sxs-lookup"><span data-stu-id="e5607-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="e5607-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="e5607-151">resourceId</span></span>       | <span data-ttu-id="e5607-152">String</span><span class="sxs-lookup"><span data-stu-id="e5607-152">String</span></span>                                                   | <span data-ttu-id="e5607-153">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="e5607-153">The ID of the resource.</span></span> <span data-ttu-id="e5607-154">必需。</span><span class="sxs-lookup"><span data-stu-id="e5607-154">Required.</span></span> |
| <span data-ttu-id="e5607-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e5607-155">roleDefinitionId</span></span> | <span data-ttu-id="e5607-156">String</span><span class="sxs-lookup"><span data-stu-id="e5607-156">String</span></span>                                                   | <span data-ttu-id="e5607-157">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="e5607-157">The ID of the role definition.</span></span> <span data-ttu-id="e5607-158">必需。</span><span class="sxs-lookup"><span data-stu-id="e5607-158">Required.</span></span> |
| <span data-ttu-id="e5607-159">subjectId</span><span class="sxs-lookup"><span data-stu-id="e5607-159">subjectId</span></span>        | <span data-ttu-id="e5607-160">String</span><span class="sxs-lookup"><span data-stu-id="e5607-160">String</span></span>                                                   | <span data-ttu-id="e5607-161">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="e5607-161">The ID of the subject.</span></span> <span data-ttu-id="e5607-162">必需。</span><span class="sxs-lookup"><span data-stu-id="e5607-162">Required.</span></span> |
| <span data-ttu-id="e5607-163">assignmentState</span><span class="sxs-lookup"><span data-stu-id="e5607-163">assignmentState</span></span>  | <span data-ttu-id="e5607-164">String</span><span class="sxs-lookup"><span data-stu-id="e5607-164">String</span></span>                                                   | <span data-ttu-id="e5607-165">工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="e5607-165">The state of assignment.</span></span> <span data-ttu-id="e5607-166">值可以是`Eligible`和`Active`。</span><span class="sxs-lookup"><span data-stu-id="e5607-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="e5607-167">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="e5607-167">Required.</span></span> |
| <span data-ttu-id="e5607-168">type</span><span class="sxs-lookup"><span data-stu-id="e5607-168">type</span></span>             | <span data-ttu-id="e5607-169">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-169">String</span></span>                                                   | <span data-ttu-id="e5607-170">请求类型。</span><span class="sxs-lookup"><span data-stu-id="e5607-170">The request type.</span></span> <span data-ttu-id="e5607-171">值可以是`AdminAdd`， `UserAdd`， `AdminUpdate`， `AdminRemove`， `UserRemove`， `UserExtend`， `UserRenew`，`AdminRenew`和`AdminExtend`。</span><span class="sxs-lookup"><span data-stu-id="e5607-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="e5607-172">必需。</span><span class="sxs-lookup"><span data-stu-id="e5607-172">Required.</span></span> |
| <span data-ttu-id="e5607-173">原因</span><span class="sxs-lookup"><span data-stu-id="e5607-173">reason</span></span>           | <span data-ttu-id="e5607-174">String</span><span class="sxs-lookup"><span data-stu-id="e5607-174">String</span></span>                                                   | <span data-ttu-id="e5607-175">原因需要提供角色分配请求的审核和查看用途。</span><span class="sxs-lookup"><span data-stu-id="e5607-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="e5607-176">计划</span><span class="sxs-lookup"><span data-stu-id="e5607-176">schedule</span></span>         | [<span data-ttu-id="e5607-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e5607-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="e5607-178">角色分配请求的时间表。</span><span class="sxs-lookup"><span data-stu-id="e5607-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="e5607-179">请求类型的`UserAdd`， `AdminAdd`， `AdminUpdate`，和`AdminExtend`，需要。</span><span class="sxs-lookup"><span data-stu-id="e5607-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="e5607-180">响应</span><span class="sxs-lookup"><span data-stu-id="e5607-180">Response</span></span>

<span data-ttu-id="e5607-181">如果成功，此方法返回`201 Created`响应代码和响应正文中的[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e5607-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="e5607-182">错误代码</span><span class="sxs-lookup"><span data-stu-id="e5607-182">Error codes</span></span>

<span data-ttu-id="e5607-183">此 API 返回的标准 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="e5607-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="e5607-184">此外，它也会返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="e5607-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="e5607-185">错误代码</span><span class="sxs-lookup"><span data-stu-id="e5607-185">Error code</span></span>     | <span data-ttu-id="e5607-186">错误消息</span><span class="sxs-lookup"><span data-stu-id="e5607-186">Error message</span></span>                               | <span data-ttu-id="e5607-187">详细信息</span><span class="sxs-lookup"><span data-stu-id="e5607-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="e5607-188">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e5607-188">400 BadRequest</span></span> | <span data-ttu-id="e5607-189">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="e5607-189">RoleNotFound</span></span>                                | <span data-ttu-id="e5607-190">`roleDefinitionId`提供在请求正文找不到。</span><span class="sxs-lookup"><span data-stu-id="e5607-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="e5607-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e5607-191">400 BadRequest</span></span> | <span data-ttu-id="e5607-192">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="e5607-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="e5607-193">在请求正文中提供的资源处于状态的`Locked`和无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="e5607-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="e5607-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e5607-194">400 BadRequest</span></span> | <span data-ttu-id="e5607-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="e5607-195">SubjectNotFound</span></span>                             | <span data-ttu-id="e5607-196">`subjectId`提供在请求正文找不到。</span><span class="sxs-lookup"><span data-stu-id="e5607-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="e5607-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e5607-197">400 BadRequest</span></span> | <span data-ttu-id="e5607-198">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="e5607-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="e5607-199">已存在挂起[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)系统中。</span><span class="sxs-lookup"><span data-stu-id="e5607-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="e5607-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e5607-200">400 BadRequest</span></span> | <span data-ttu-id="e5607-201">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="e5607-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="e5607-202">系统中存在[governanceRoleAssignment](../resources/governanceroleassignment.md)请求已创建。</span><span class="sxs-lookup"><span data-stu-id="e5607-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="e5607-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e5607-203">400 BadRequest</span></span> | <span data-ttu-id="e5607-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="e5607-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="e5607-205">系统中不存在[governanceRoleAssignment](../resources/governanceroleassignment.md)请求来更新/扩展。</span><span class="sxs-lookup"><span data-stu-id="e5607-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="e5607-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e5607-206">400 BadRequest</span></span> | <span data-ttu-id="e5607-207">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="e5607-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="e5607-208">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部的策略，且无法创建。</span><span class="sxs-lookup"><span data-stu-id="e5607-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="e5607-209">示例</span><span class="sxs-lookup"><span data-stu-id="e5607-209">Examples</span></span>

<span data-ttu-id="e5607-210">下面的示例演示如何使用此 API。</span><span class="sxs-lookup"><span data-stu-id="e5607-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="e5607-211">示例 1： 则管理员会将用户分配给某个角色</span><span class="sxs-lookup"><span data-stu-id="e5607-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="e5607-212">本示例中，管理员向帐单读者角色分配用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="e5607-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="e5607-213">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="e5607-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="e5607-214">属性</span><span class="sxs-lookup"><span data-stu-id="e5607-214">Property</span></span>         | <span data-ttu-id="e5607-215">类型</span><span class="sxs-lookup"><span data-stu-id="e5607-215">Type</span></span>                                                     | <span data-ttu-id="e5607-216">是否必需</span><span class="sxs-lookup"><span data-stu-id="e5607-216">Required</span></span>                 | <span data-ttu-id="e5607-217">值</span><span class="sxs-lookup"><span data-stu-id="e5607-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="e5607-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="e5607-218">resourceId</span></span>       | <span data-ttu-id="e5607-219">String</span><span class="sxs-lookup"><span data-stu-id="e5607-219">String</span></span>                                                   | <span data-ttu-id="e5607-220">是</span><span class="sxs-lookup"><span data-stu-id="e5607-220">Yes</span></span>                      | <span data-ttu-id="e5607-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="e5607-221">\<resourceId\></span></span> |
| <span data-ttu-id="e5607-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e5607-222">roleDefinitionId</span></span> | <span data-ttu-id="e5607-223">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-223">String</span></span>                                                   | <span data-ttu-id="e5607-224">是</span><span class="sxs-lookup"><span data-stu-id="e5607-224">Yes</span></span>                      | <span data-ttu-id="e5607-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="e5607-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="e5607-226">subjectId</span><span class="sxs-lookup"><span data-stu-id="e5607-226">subjectId</span></span>        | <span data-ttu-id="e5607-227">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-227">String</span></span>                                                   | <span data-ttu-id="e5607-228">是</span><span class="sxs-lookup"><span data-stu-id="e5607-228">Yes</span></span>                      | <span data-ttu-id="e5607-229">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="e5607-229">\<subjectId\></span></span> |
| <span data-ttu-id="e5607-230">assignmentState</span><span class="sxs-lookup"><span data-stu-id="e5607-230">assignmentState</span></span>  | <span data-ttu-id="e5607-231">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-231">String</span></span>                                                   | <span data-ttu-id="e5607-232">是</span><span class="sxs-lookup"><span data-stu-id="e5607-232">Yes</span></span>                      | <span data-ttu-id="e5607-233">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="e5607-233">Eligible / Active</span></span> |
| <span data-ttu-id="e5607-234">type</span><span class="sxs-lookup"><span data-stu-id="e5607-234">type</span></span>             | <span data-ttu-id="e5607-235">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-235">String</span></span>                                                   | <span data-ttu-id="e5607-236">是</span><span class="sxs-lookup"><span data-stu-id="e5607-236">Yes</span></span>                      | <span data-ttu-id="e5607-237">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="e5607-237">AdminAdd</span></span> |
| <span data-ttu-id="e5607-238">原因</span><span class="sxs-lookup"><span data-stu-id="e5607-238">reason</span></span>           | <span data-ttu-id="e5607-239">String</span><span class="sxs-lookup"><span data-stu-id="e5607-239">String</span></span>                                                   | <span data-ttu-id="e5607-240">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="e5607-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="e5607-241">计划</span><span class="sxs-lookup"><span data-stu-id="e5607-241">schedule</span></span>         | [<span data-ttu-id="e5607-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e5607-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="e5607-243">是</span><span class="sxs-lookup"><span data-stu-id="e5607-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="e5607-244">请求</span><span class="sxs-lookup"><span data-stu-id="e5607-244">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Eligible",
  "type": "AdminAdd",
  "reason": "Assign an eligible role",
  "schedule": {
    "startDateTime": "2018-05-12T23:37:43.356Z",
    "endDateTime": "2018-11-08T23:37:43.356Z",
    "type": "Once"
  }
}
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="e5607-245">响应</span><span class="sxs-lookup"><span data-stu-id="e5607-245">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="e5607-246">示例 2： 用户激活合格的角色</span><span class="sxs-lookup"><span data-stu-id="e5607-246">Example 2: User activates eligible role</span></span>

<span data-ttu-id="e5607-247">本示例中，用户 nawu@fimdev.net 激活合格的帐单读取器角色。</span><span class="sxs-lookup"><span data-stu-id="e5607-247">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="e5607-248">属性</span><span class="sxs-lookup"><span data-stu-id="e5607-248">Property</span></span>         | <span data-ttu-id="e5607-249">类型</span><span class="sxs-lookup"><span data-stu-id="e5607-249">Type</span></span>                                                     | <span data-ttu-id="e5607-250">是否必需</span><span class="sxs-lookup"><span data-stu-id="e5607-250">Required</span></span>                 | <span data-ttu-id="e5607-251">值</span><span class="sxs-lookup"><span data-stu-id="e5607-251">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="e5607-252">resourceId</span><span class="sxs-lookup"><span data-stu-id="e5607-252">resourceId</span></span>       | <span data-ttu-id="e5607-253">String</span><span class="sxs-lookup"><span data-stu-id="e5607-253">String</span></span>                                                   | <span data-ttu-id="e5607-254">是</span><span class="sxs-lookup"><span data-stu-id="e5607-254">Yes</span></span>                      | <span data-ttu-id="e5607-255">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="e5607-255">\<resourceId\></span></span> |
| <span data-ttu-id="e5607-256">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e5607-256">roleDefinitionId</span></span> | <span data-ttu-id="e5607-257">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-257">String</span></span>                                                   | <span data-ttu-id="e5607-258">是</span><span class="sxs-lookup"><span data-stu-id="e5607-258">Yes</span></span>                      | <span data-ttu-id="e5607-259">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="e5607-259">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="e5607-260">subjectId</span><span class="sxs-lookup"><span data-stu-id="e5607-260">subjectId</span></span>        | <span data-ttu-id="e5607-261">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-261">String</span></span>                                                   | <span data-ttu-id="e5607-262">是</span><span class="sxs-lookup"><span data-stu-id="e5607-262">Yes</span></span>                      | <span data-ttu-id="e5607-263">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="e5607-263">\<subjectId\></span></span> |
| <span data-ttu-id="e5607-264">assignmentState</span><span class="sxs-lookup"><span data-stu-id="e5607-264">assignmentState</span></span>  | <span data-ttu-id="e5607-265">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-265">String</span></span>                                                   | <span data-ttu-id="e5607-266">是</span><span class="sxs-lookup"><span data-stu-id="e5607-266">Yes</span></span>                      | <span data-ttu-id="e5607-267">活动</span><span class="sxs-lookup"><span data-stu-id="e5607-267">Active</span></span> |
| <span data-ttu-id="e5607-268">type</span><span class="sxs-lookup"><span data-stu-id="e5607-268">type</span></span>             | <span data-ttu-id="e5607-269">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-269">String</span></span>                                                   | <span data-ttu-id="e5607-270">是</span><span class="sxs-lookup"><span data-stu-id="e5607-270">Yes</span></span>                      | <span data-ttu-id="e5607-271">UserAdd</span><span class="sxs-lookup"><span data-stu-id="e5607-271">UserAdd</span></span> |
| <span data-ttu-id="e5607-272">原因</span><span class="sxs-lookup"><span data-stu-id="e5607-272">reason</span></span>           | <span data-ttu-id="e5607-273">String</span><span class="sxs-lookup"><span data-stu-id="e5607-273">String</span></span>                                                   | <span data-ttu-id="e5607-274">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="e5607-274">depends on role Settings</span></span> |   |
| <span data-ttu-id="e5607-275">计划</span><span class="sxs-lookup"><span data-stu-id="e5607-275">schedule</span></span>         | [<span data-ttu-id="e5607-276">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e5607-276">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="e5607-277">是</span><span class="sxs-lookup"><span data-stu-id="e5607-277">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="e5607-278">请求</span><span class="sxs-lookup"><span data-stu-id="e5607-278">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserAdd",
  "reason": "Activate the owner role",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:28:43.537Z",
    "duration": "PT9H"
  },
  "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394"
}
```

#### <a name="response"></a><span data-ttu-id="e5607-279">响应</span><span class="sxs-lookup"><span data-stu-id="e5607-279">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="e5607-280">示例 3： 停用用户分配的角色</span><span class="sxs-lookup"><span data-stu-id="e5607-280">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="e5607-281">本示例中，用户 nawu@fimdev.net 停用活动的帐单读取器角色。</span><span class="sxs-lookup"><span data-stu-id="e5607-281">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="e5607-282">属性</span><span class="sxs-lookup"><span data-stu-id="e5607-282">Property</span></span>         | <span data-ttu-id="e5607-283">类型</span><span class="sxs-lookup"><span data-stu-id="e5607-283">Type</span></span>                                                     | <span data-ttu-id="e5607-284">是否必需</span><span class="sxs-lookup"><span data-stu-id="e5607-284">Required</span></span> | <span data-ttu-id="e5607-285">值</span><span class="sxs-lookup"><span data-stu-id="e5607-285">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="e5607-286">resourceId</span><span class="sxs-lookup"><span data-stu-id="e5607-286">resourceId</span></span>       | <span data-ttu-id="e5607-287">String</span><span class="sxs-lookup"><span data-stu-id="e5607-287">String</span></span>                                                   | <span data-ttu-id="e5607-288">是</span><span class="sxs-lookup"><span data-stu-id="e5607-288">Yes</span></span>      | <span data-ttu-id="e5607-289">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="e5607-289">\<resourceId\></span></span> |
| <span data-ttu-id="e5607-290">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e5607-290">roleDefinitionId</span></span> | <span data-ttu-id="e5607-291">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-291">String</span></span>                                                   | <span data-ttu-id="e5607-292">是</span><span class="sxs-lookup"><span data-stu-id="e5607-292">Yes</span></span>      | <span data-ttu-id="e5607-293">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="e5607-293">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="e5607-294">subjectId</span><span class="sxs-lookup"><span data-stu-id="e5607-294">subjectId</span></span>        | <span data-ttu-id="e5607-295">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-295">String</span></span>                                                   | <span data-ttu-id="e5607-296">是</span><span class="sxs-lookup"><span data-stu-id="e5607-296">Yes</span></span>      | <span data-ttu-id="e5607-297">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="e5607-297">\<subjectId\></span></span> |
| <span data-ttu-id="e5607-298">assignmentState</span><span class="sxs-lookup"><span data-stu-id="e5607-298">assignmentState</span></span>  | <span data-ttu-id="e5607-299">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-299">String</span></span>                                                   | <span data-ttu-id="e5607-300">是</span><span class="sxs-lookup"><span data-stu-id="e5607-300">Yes</span></span>      | <span data-ttu-id="e5607-301">活动</span><span class="sxs-lookup"><span data-stu-id="e5607-301">Active</span></span> |
| <span data-ttu-id="e5607-302">type</span><span class="sxs-lookup"><span data-stu-id="e5607-302">type</span></span>             | <span data-ttu-id="e5607-303">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-303">String</span></span>                                                   | <span data-ttu-id="e5607-304">是</span><span class="sxs-lookup"><span data-stu-id="e5607-304">Yes</span></span>      | <span data-ttu-id="e5607-305">UserRemove</span><span class="sxs-lookup"><span data-stu-id="e5607-305">UserRemove</span></span> |
| <span data-ttu-id="e5607-306">原因</span><span class="sxs-lookup"><span data-stu-id="e5607-306">reason</span></span>           | <span data-ttu-id="e5607-307">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-307">String</span></span>                                                   | <span data-ttu-id="e5607-308">否</span><span class="sxs-lookup"><span data-stu-id="e5607-308">No</span></span>       |   |
| <span data-ttu-id="e5607-309">计划</span><span class="sxs-lookup"><span data-stu-id="e5607-309">schedule</span></span>         | [<span data-ttu-id="e5607-310">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e5607-310">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="e5607-311">否</span><span class="sxs-lookup"><span data-stu-id="e5607-311">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="e5607-312">请求</span><span class="sxs-lookup"><span data-stu-id="e5607-312">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
  "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserRemove",
  "reason": "Deactivate the role",
  "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```

#### <a name="response"></a><span data-ttu-id="e5607-313">响应</span><span class="sxs-lookup"><span data-stu-id="e5607-313">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="e5607-314">示例 4： 管理员删除用户从角色</span><span class="sxs-lookup"><span data-stu-id="e5607-314">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="e5607-315">本示例中，管理员从帐单读者角色中删除用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="e5607-315">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="e5607-316">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="e5607-316">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="e5607-317">属性</span><span class="sxs-lookup"><span data-stu-id="e5607-317">Property</span></span>         | <span data-ttu-id="e5607-318">类型</span><span class="sxs-lookup"><span data-stu-id="e5607-318">Type</span></span>                                                     | <span data-ttu-id="e5607-319">是否必需</span><span class="sxs-lookup"><span data-stu-id="e5607-319">Required</span></span> | <span data-ttu-id="e5607-320">值</span><span class="sxs-lookup"><span data-stu-id="e5607-320">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="e5607-321">resourceId</span><span class="sxs-lookup"><span data-stu-id="e5607-321">resourceId</span></span>       | <span data-ttu-id="e5607-322">String</span><span class="sxs-lookup"><span data-stu-id="e5607-322">String</span></span>                                                   | <span data-ttu-id="e5607-323">是</span><span class="sxs-lookup"><span data-stu-id="e5607-323">Yes</span></span>      | <span data-ttu-id="e5607-324">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="e5607-324">\<resourceId\></span></span> |
| <span data-ttu-id="e5607-325">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e5607-325">roleDefinitionId</span></span> | <span data-ttu-id="e5607-326">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-326">String</span></span>                                                   | <span data-ttu-id="e5607-327">是</span><span class="sxs-lookup"><span data-stu-id="e5607-327">Yes</span></span>      | <span data-ttu-id="e5607-328">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="e5607-328">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="e5607-329">subjectId</span><span class="sxs-lookup"><span data-stu-id="e5607-329">subjectId</span></span>        | <span data-ttu-id="e5607-330">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-330">String</span></span>                                                   | <span data-ttu-id="e5607-331">是</span><span class="sxs-lookup"><span data-stu-id="e5607-331">Yes</span></span>      | <span data-ttu-id="e5607-332">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="e5607-332">\<subjectId\></span></span> |
| <span data-ttu-id="e5607-333">assignmentState</span><span class="sxs-lookup"><span data-stu-id="e5607-333">assignmentState</span></span>  | <span data-ttu-id="e5607-334">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-334">String</span></span>                                                   | <span data-ttu-id="e5607-335">是</span><span class="sxs-lookup"><span data-stu-id="e5607-335">Yes</span></span>      | <span data-ttu-id="e5607-336">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="e5607-336">Eligible / Active</span></span> |
| <span data-ttu-id="e5607-337">type</span><span class="sxs-lookup"><span data-stu-id="e5607-337">type</span></span>             | <span data-ttu-id="e5607-338">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-338">String</span></span>                                                   | <span data-ttu-id="e5607-339">是</span><span class="sxs-lookup"><span data-stu-id="e5607-339">Yes</span></span>      | <span data-ttu-id="e5607-340">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="e5607-340">AdminRemove</span></span> |
| <span data-ttu-id="e5607-341">原因</span><span class="sxs-lookup"><span data-stu-id="e5607-341">reason</span></span>           | <span data-ttu-id="e5607-342">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-342">String</span></span>                                                   | <span data-ttu-id="e5607-343">否</span><span class="sxs-lookup"><span data-stu-id="e5607-343">No</span></span>       |   |
| <span data-ttu-id="e5607-344">计划</span><span class="sxs-lookup"><span data-stu-id="e5607-344">schedule</span></span>         | [<span data-ttu-id="e5607-345">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e5607-345">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="e5607-346">否</span><span class="sxs-lookup"><span data-stu-id="e5607-346">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="e5607-347">请求</span><span class="sxs-lookup"><span data-stu-id="e5607-347">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminRemove"
}
```

#### <a name="response"></a><span data-ttu-id="e5607-348">响应</span><span class="sxs-lookup"><span data-stu-id="e5607-348">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminRemove",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
  "status": {
    "status": "Closed",
    "subStatus": "Revoked",
    "statusDetails": []
  },
  "schedule": null
}
```

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="e5607-349">示例 5： 管理员更新角色分配</span><span class="sxs-lookup"><span data-stu-id="e5607-349">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="e5607-350">本示例中，管理员向所有者更新用户 nawu@fimdev.net 的角色分配。</span><span class="sxs-lookup"><span data-stu-id="e5607-350">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="e5607-351">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="e5607-351">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="e5607-352">属性</span><span class="sxs-lookup"><span data-stu-id="e5607-352">Property</span></span>         | <span data-ttu-id="e5607-353">类型</span><span class="sxs-lookup"><span data-stu-id="e5607-353">Type</span></span>                                                     | <span data-ttu-id="e5607-354">是否必需</span><span class="sxs-lookup"><span data-stu-id="e5607-354">Required</span></span>                | <span data-ttu-id="e5607-355">值</span><span class="sxs-lookup"><span data-stu-id="e5607-355">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="e5607-356">resourceId</span><span class="sxs-lookup"><span data-stu-id="e5607-356">resourceId</span></span>       | <span data-ttu-id="e5607-357">String</span><span class="sxs-lookup"><span data-stu-id="e5607-357">String</span></span>                                                   | <span data-ttu-id="e5607-358">是</span><span class="sxs-lookup"><span data-stu-id="e5607-358">Yes</span></span>                     | <span data-ttu-id="e5607-359">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="e5607-359">\<resourceId\></span></span> |
| <span data-ttu-id="e5607-360">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e5607-360">roleDefinitionId</span></span> | <span data-ttu-id="e5607-361">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-361">String</span></span>                                                   | <span data-ttu-id="e5607-362">是</span><span class="sxs-lookup"><span data-stu-id="e5607-362">Yes</span></span>                     | <span data-ttu-id="e5607-363">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="e5607-363">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="e5607-364">subjectId</span><span class="sxs-lookup"><span data-stu-id="e5607-364">subjectId</span></span>        | <span data-ttu-id="e5607-365">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-365">String</span></span>                                                   | <span data-ttu-id="e5607-366">是</span><span class="sxs-lookup"><span data-stu-id="e5607-366">Yes</span></span>                     | <span data-ttu-id="e5607-367">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="e5607-367">\<subjectId\></span></span> |
| <span data-ttu-id="e5607-368">assignmentState</span><span class="sxs-lookup"><span data-stu-id="e5607-368">assignmentState</span></span>  | <span data-ttu-id="e5607-369">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-369">String</span></span>                                                   | <span data-ttu-id="e5607-370">是</span><span class="sxs-lookup"><span data-stu-id="e5607-370">Yes</span></span>                     | <span data-ttu-id="e5607-371">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="e5607-371">Eligible / Active</span></span> |
| <span data-ttu-id="e5607-372">type</span><span class="sxs-lookup"><span data-stu-id="e5607-372">type</span></span>             | <span data-ttu-id="e5607-373">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-373">String</span></span>                                                   | <span data-ttu-id="e5607-374">是</span><span class="sxs-lookup"><span data-stu-id="e5607-374">Yes</span></span>                     | <span data-ttu-id="e5607-375">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="e5607-375">AdminUpdate</span></span> |
| <span data-ttu-id="e5607-376">原因</span><span class="sxs-lookup"><span data-stu-id="e5607-376">reason</span></span>           | <span data-ttu-id="e5607-377">String</span><span class="sxs-lookup"><span data-stu-id="e5607-377">String</span></span>                                                   | <span data-ttu-id="e5607-378">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="e5607-378">depends on roleSettings</span></span> |   |
| <span data-ttu-id="e5607-379">计划</span><span class="sxs-lookup"><span data-stu-id="e5607-379">schedule</span></span>         | [<span data-ttu-id="e5607-380">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e5607-380">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="e5607-381">是</span><span class="sxs-lookup"><span data-stu-id="e5607-381">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="e5607-382">请求</span><span class="sxs-lookup"><span data-stu-id="e5607-382">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState": "Eligible",
  "type": "AdminUpdate",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31.000Z"
  }
}
```

#### <a name="response"></a><span data-ttu-id="e5607-383">响应</span><span class="sxs-lookup"><span data-stu-id="e5607-383">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminUpdate",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
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
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31Z",
    "duration": "PT0S"
  }
}
```

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="e5607-384">示例 6： 管理员扩展即将过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="e5607-384">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="e5607-385">本示例将用户 ANUJCUSER 即将过期的角色分配给 API 管理服务参与者。</span><span class="sxs-lookup"><span data-stu-id="e5607-385">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="e5607-386">**注意：** 除了权限，此示例要求申请者有至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="e5607-386">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="e5607-387">属性</span><span class="sxs-lookup"><span data-stu-id="e5607-387">Property</span></span>         | <span data-ttu-id="e5607-388">类型</span><span class="sxs-lookup"><span data-stu-id="e5607-388">Type</span></span>                                                     | <span data-ttu-id="e5607-389">是否必需</span><span class="sxs-lookup"><span data-stu-id="e5607-389">Required</span></span>                | <span data-ttu-id="e5607-390">值</span><span class="sxs-lookup"><span data-stu-id="e5607-390">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="e5607-391">resourceId</span><span class="sxs-lookup"><span data-stu-id="e5607-391">resourceId</span></span>       | <span data-ttu-id="e5607-392">String</span><span class="sxs-lookup"><span data-stu-id="e5607-392">String</span></span>                                                   | <span data-ttu-id="e5607-393">是</span><span class="sxs-lookup"><span data-stu-id="e5607-393">Yes</span></span>                     | <span data-ttu-id="e5607-394">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="e5607-394">\<resourceId\></span></span> |
| <span data-ttu-id="e5607-395">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e5607-395">roleDefinitionId</span></span> | <span data-ttu-id="e5607-396">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-396">String</span></span>                                                   | <span data-ttu-id="e5607-397">是</span><span class="sxs-lookup"><span data-stu-id="e5607-397">Yes</span></span>                     | <span data-ttu-id="e5607-398">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="e5607-398">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="e5607-399">subjectId</span><span class="sxs-lookup"><span data-stu-id="e5607-399">subjectId</span></span>        | <span data-ttu-id="e5607-400">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-400">String</span></span>                                                   | <span data-ttu-id="e5607-401">是</span><span class="sxs-lookup"><span data-stu-id="e5607-401">Yes</span></span>                     | <span data-ttu-id="e5607-402">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="e5607-402">\<subjectId\></span></span> |
| <span data-ttu-id="e5607-403">assignmentState</span><span class="sxs-lookup"><span data-stu-id="e5607-403">assignmentState</span></span>  | <span data-ttu-id="e5607-404">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-404">String</span></span>                                                   | <span data-ttu-id="e5607-405">是</span><span class="sxs-lookup"><span data-stu-id="e5607-405">Yes</span></span>                     | <span data-ttu-id="e5607-406">合格 / 活动</span><span class="sxs-lookup"><span data-stu-id="e5607-406">Eligible / Active</span></span> |
| <span data-ttu-id="e5607-407">type</span><span class="sxs-lookup"><span data-stu-id="e5607-407">type</span></span>             | <span data-ttu-id="e5607-408">字符串</span><span class="sxs-lookup"><span data-stu-id="e5607-408">String</span></span>                                                   | <span data-ttu-id="e5607-409">是</span><span class="sxs-lookup"><span data-stu-id="e5607-409">Yes</span></span>                     | <span data-ttu-id="e5607-410">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="e5607-410">AdminExtend</span></span> |
| <span data-ttu-id="e5607-411">原因</span><span class="sxs-lookup"><span data-stu-id="e5607-411">reason</span></span>           | <span data-ttu-id="e5607-412">String</span><span class="sxs-lookup"><span data-stu-id="e5607-412">String</span></span>                                                   | <span data-ttu-id="e5607-413">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="e5607-413">depends on roleSettings</span></span> |   |
| <span data-ttu-id="e5607-414">计划</span><span class="sxs-lookup"><span data-stu-id="e5607-414">schedule</span></span>         | [<span data-ttu-id="e5607-415">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e5607-415">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="e5607-416">是</span><span class="sxs-lookup"><span data-stu-id="e5607-416">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="e5607-417">请求</span><span class="sxs-lookup"><span data-stu-id="e5607-417">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminExtend",
  "reason": "extend role assignment",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z"
  }
}
```

#### <a name="response"></a><span data-ttu-id="e5607-418">响应</span><span class="sxs-lookup"><span data-stu-id="e5607-418">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminExtend",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "extend role assignment",
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
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z",
    "duration": "PT0S"
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
