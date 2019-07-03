---
title: 创建 governanceRoleAssignmentRequest
description: 创建一个角色分配请求, 以代表在角色分配上所需的操作。 下表列出了这些操作。
localization_priority: Normal
ms.openlocfilehash: 614d5a90bbf71f8cb5794923ae4f56d85d06415e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440776"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="a506d-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="a506d-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a506d-105">创建一个角色分配请求, 以代表在角色分配上所需的操作。</span><span class="sxs-lookup"><span data-stu-id="a506d-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="a506d-106">下表列出了这些操作。</span><span class="sxs-lookup"><span data-stu-id="a506d-106">The following table lists the operations.</span></span>

| <span data-ttu-id="a506d-107">Operation</span><span class="sxs-lookup"><span data-stu-id="a506d-107">Operation</span></span>                                   | <span data-ttu-id="a506d-108">类型</span><span class="sxs-lookup"><span data-stu-id="a506d-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="a506d-109">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="a506d-109">Assign a role assignment</span></span>                    | <span data-ttu-id="a506d-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="a506d-110">AdminAdd</span></span>    |
| <span data-ttu-id="a506d-111">激活符合条件的角色分配</span><span class="sxs-lookup"><span data-stu-id="a506d-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="a506d-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="a506d-112">UserAdd</span></span>     |
| <span data-ttu-id="a506d-113">停用已激活的角色分配</span><span class="sxs-lookup"><span data-stu-id="a506d-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="a506d-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="a506d-114">UserRemove</span></span>  |
| <span data-ttu-id="a506d-115">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="a506d-115">Remove a role assignment</span></span>                    | <span data-ttu-id="a506d-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="a506d-116">AdminRemove</span></span> |
| <span data-ttu-id="a506d-117">更新角色分配</span><span class="sxs-lookup"><span data-stu-id="a506d-117">Update a role assignment</span></span>                    | <span data-ttu-id="a506d-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="a506d-118">AdminUpdate</span></span> |
| <span data-ttu-id="a506d-119">请求扩展我的角色分配</span><span class="sxs-lookup"><span data-stu-id="a506d-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="a506d-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="a506d-120">UserExtend</span></span>  |
| <span data-ttu-id="a506d-121">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="a506d-121">Extend a role assignment</span></span>                    | <span data-ttu-id="a506d-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="a506d-122">AdminExtend</span></span> |
| <span data-ttu-id="a506d-123">续订我的过期角色分配的请求</span><span class="sxs-lookup"><span data-stu-id="a506d-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="a506d-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="a506d-124">UserRenew</span></span>   |
| <span data-ttu-id="a506d-125">续订过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="a506d-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="a506d-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="a506d-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="a506d-127">权限</span><span class="sxs-lookup"><span data-stu-id="a506d-127">Permissions</span></span>

<span data-ttu-id="a506d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a506d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a506d-130">权限类型</span><span class="sxs-lookup"><span data-stu-id="a506d-130">Permission type</span></span>                        | <span data-ttu-id="a506d-131">权限</span><span class="sxs-lookup"><span data-stu-id="a506d-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="a506d-132">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a506d-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="a506d-133">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="a506d-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="a506d-134">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a506d-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a506d-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="a506d-135">Not supported.</span></span>                            |
| <span data-ttu-id="a506d-136">应用程序</span><span class="sxs-lookup"><span data-stu-id="a506d-136">Application</span></span>                            | <span data-ttu-id="a506d-137">不支持。</span><span class="sxs-lookup"><span data-stu-id="a506d-137">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a506d-138">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a506d-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="a506d-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="a506d-139">Request headers</span></span>

| <span data-ttu-id="a506d-140">名称</span><span class="sxs-lookup"><span data-stu-id="a506d-140">Name</span></span>          | <span data-ttu-id="a506d-141">说明</span><span class="sxs-lookup"><span data-stu-id="a506d-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="a506d-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="a506d-142">Authorization</span></span> | <span data-ttu-id="a506d-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a506d-143">Bearer {code}</span></span>    |
| <span data-ttu-id="a506d-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="a506d-144">Content-type</span></span>  | <span data-ttu-id="a506d-145">application/json</span><span class="sxs-lookup"><span data-stu-id="a506d-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a506d-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="a506d-146">Request body</span></span>

<span data-ttu-id="a506d-147">在请求正文中, 提供[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a506d-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="a506d-148">属性</span><span class="sxs-lookup"><span data-stu-id="a506d-148">Property</span></span>         | <span data-ttu-id="a506d-149">类型</span><span class="sxs-lookup"><span data-stu-id="a506d-149">Type</span></span>                                                     | <span data-ttu-id="a506d-150">说明</span><span class="sxs-lookup"><span data-stu-id="a506d-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="a506d-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="a506d-151">resourceId</span></span>       | <span data-ttu-id="a506d-152">String</span><span class="sxs-lookup"><span data-stu-id="a506d-152">String</span></span>                                                   | <span data-ttu-id="a506d-153">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="a506d-153">The ID of the resource.</span></span> <span data-ttu-id="a506d-154">必需。</span><span class="sxs-lookup"><span data-stu-id="a506d-154">Required.</span></span> |
| <span data-ttu-id="a506d-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a506d-155">roleDefinitionId</span></span> | <span data-ttu-id="a506d-156">String</span><span class="sxs-lookup"><span data-stu-id="a506d-156">String</span></span>                                                   | <span data-ttu-id="a506d-157">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="a506d-157">The ID of the role definition.</span></span> <span data-ttu-id="a506d-158">必需。</span><span class="sxs-lookup"><span data-stu-id="a506d-158">Required.</span></span> |
| <span data-ttu-id="a506d-159">subjectId</span><span class="sxs-lookup"><span data-stu-id="a506d-159">subjectId</span></span>        | <span data-ttu-id="a506d-160">String</span><span class="sxs-lookup"><span data-stu-id="a506d-160">String</span></span>                                                   | <span data-ttu-id="a506d-161">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="a506d-161">The ID of the subject.</span></span> <span data-ttu-id="a506d-162">必需。</span><span class="sxs-lookup"><span data-stu-id="a506d-162">Required.</span></span> |
| <span data-ttu-id="a506d-163">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a506d-163">assignmentState</span></span>  | <span data-ttu-id="a506d-164">String</span><span class="sxs-lookup"><span data-stu-id="a506d-164">String</span></span>                                                   | <span data-ttu-id="a506d-165">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="a506d-165">The state of assignment.</span></span> <span data-ttu-id="a506d-166">值可以是`Eligible`和`Active`。</span><span class="sxs-lookup"><span data-stu-id="a506d-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="a506d-167">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="a506d-167">Required.</span></span> |
| <span data-ttu-id="a506d-168">type</span><span class="sxs-lookup"><span data-stu-id="a506d-168">type</span></span>             | <span data-ttu-id="a506d-169">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-169">String</span></span>                                                   | <span data-ttu-id="a506d-170">请求类型。</span><span class="sxs-lookup"><span data-stu-id="a506d-170">The request type.</span></span> <span data-ttu-id="a506d-171">值可以是`AdminAdd` `UserAdd`、、 `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `AdminRenew` `AdminExtend`、、、、和。 `UserRenew`</span><span class="sxs-lookup"><span data-stu-id="a506d-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="a506d-172">必需。</span><span class="sxs-lookup"><span data-stu-id="a506d-172">Required.</span></span> |
| <span data-ttu-id="a506d-173">在于</span><span class="sxs-lookup"><span data-stu-id="a506d-173">reason</span></span>           | <span data-ttu-id="a506d-174">String</span><span class="sxs-lookup"><span data-stu-id="a506d-174">String</span></span>                                                   | <span data-ttu-id="a506d-175">需要为角色分配请求提供审核和审阅目的的原因。</span><span class="sxs-lookup"><span data-stu-id="a506d-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="a506d-176">schedule</span><span class="sxs-lookup"><span data-stu-id="a506d-176">schedule</span></span>         | [<span data-ttu-id="a506d-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a506d-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a506d-178">角色分配请求的日程安排。</span><span class="sxs-lookup"><span data-stu-id="a506d-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="a506d-179">对于的请求类型`UserAdd`, `AdminAdd` `AdminUpdate`、和`AdminExtend`, 它是必需的。</span><span class="sxs-lookup"><span data-stu-id="a506d-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="a506d-180">响应</span><span class="sxs-lookup"><span data-stu-id="a506d-180">Response</span></span>

<span data-ttu-id="a506d-181">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a506d-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="a506d-182">错误代码</span><span class="sxs-lookup"><span data-stu-id="a506d-182">Error codes</span></span>

<span data-ttu-id="a506d-183">此 API 返回标准的 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="a506d-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="a506d-184">此外, 它还返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="a506d-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="a506d-185">错误代码</span><span class="sxs-lookup"><span data-stu-id="a506d-185">Error code</span></span>     | <span data-ttu-id="a506d-186">错误消息</span><span class="sxs-lookup"><span data-stu-id="a506d-186">Error message</span></span>                               | <span data-ttu-id="a506d-187">详细信息</span><span class="sxs-lookup"><span data-stu-id="a506d-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="a506d-188">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a506d-188">400 BadRequest</span></span> | <span data-ttu-id="a506d-189">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="a506d-189">RoleNotFound</span></span>                                | <span data-ttu-id="a506d-190">找`roleDefinitionId`不到请求正文中提供的。</span><span class="sxs-lookup"><span data-stu-id="a506d-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="a506d-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a506d-191">400 BadRequest</span></span> | <span data-ttu-id="a506d-192">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="a506d-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="a506d-193">请求正文中提供的资源处于状态`Locked` , 并且无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="a506d-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="a506d-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a506d-194">400 BadRequest</span></span> | <span data-ttu-id="a506d-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="a506d-195">SubjectNotFound</span></span>                             | <span data-ttu-id="a506d-196">找`subjectId`不到请求正文中提供的。</span><span class="sxs-lookup"><span data-stu-id="a506d-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="a506d-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a506d-197">400 BadRequest</span></span> | <span data-ttu-id="a506d-198">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="a506d-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="a506d-199">系统中已存在一个挂起的[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 。</span><span class="sxs-lookup"><span data-stu-id="a506d-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="a506d-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a506d-200">400 BadRequest</span></span> | <span data-ttu-id="a506d-201">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="a506d-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="a506d-202">系统中已存在请求创建的[governanceRoleAssignment](../resources/governanceroleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="a506d-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="a506d-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a506d-203">400 BadRequest</span></span> | <span data-ttu-id="a506d-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="a506d-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="a506d-205">系统中不存在请求进行更新/扩展的[governanceRoleAssignment](../resources/governanceroleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="a506d-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="a506d-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a506d-206">400 BadRequest</span></span> | <span data-ttu-id="a506d-207">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="a506d-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="a506d-208">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部策略, 因此无法创建。</span><span class="sxs-lookup"><span data-stu-id="a506d-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="a506d-209">示例</span><span class="sxs-lookup"><span data-stu-id="a506d-209">Examples</span></span>

<span data-ttu-id="a506d-210">下面的示例演示如何使用此 API。</span><span class="sxs-lookup"><span data-stu-id="a506d-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="a506d-211">示例 1: 管理员为用户分配角色</span><span class="sxs-lookup"><span data-stu-id="a506d-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="a506d-212">在此示例中, 管理员向计费读者角色分配用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="a506d-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="a506d-213">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="a506d-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="a506d-214">属性</span><span class="sxs-lookup"><span data-stu-id="a506d-214">Property</span></span>         | <span data-ttu-id="a506d-215">类型</span><span class="sxs-lookup"><span data-stu-id="a506d-215">Type</span></span>                                                     | <span data-ttu-id="a506d-216">必需</span><span class="sxs-lookup"><span data-stu-id="a506d-216">Required</span></span>                 | <span data-ttu-id="a506d-217">值</span><span class="sxs-lookup"><span data-stu-id="a506d-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="a506d-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="a506d-218">resourceId</span></span>       | <span data-ttu-id="a506d-219">String</span><span class="sxs-lookup"><span data-stu-id="a506d-219">String</span></span>                                                   | <span data-ttu-id="a506d-220">是</span><span class="sxs-lookup"><span data-stu-id="a506d-220">Yes</span></span>                      | <span data-ttu-id="a506d-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a506d-221">\<resourceId\></span></span> |
| <span data-ttu-id="a506d-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a506d-222">roleDefinitionId</span></span> | <span data-ttu-id="a506d-223">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-223">String</span></span>                                                   | <span data-ttu-id="a506d-224">是</span><span class="sxs-lookup"><span data-stu-id="a506d-224">Yes</span></span>                      | <span data-ttu-id="a506d-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a506d-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="a506d-226">subjectId</span><span class="sxs-lookup"><span data-stu-id="a506d-226">subjectId</span></span>        | <span data-ttu-id="a506d-227">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-227">String</span></span>                                                   | <span data-ttu-id="a506d-228">是</span><span class="sxs-lookup"><span data-stu-id="a506d-228">Yes</span></span>                      | <span data-ttu-id="a506d-229">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a506d-229">\<subjectId\></span></span> |
| <span data-ttu-id="a506d-230">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a506d-230">assignmentState</span></span>  | <span data-ttu-id="a506d-231">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-231">String</span></span>                                                   | <span data-ttu-id="a506d-232">是</span><span class="sxs-lookup"><span data-stu-id="a506d-232">Yes</span></span>                      | <span data-ttu-id="a506d-233">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="a506d-233">Eligible / Active</span></span> |
| <span data-ttu-id="a506d-234">type</span><span class="sxs-lookup"><span data-stu-id="a506d-234">type</span></span>             | <span data-ttu-id="a506d-235">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-235">String</span></span>                                                   | <span data-ttu-id="a506d-236">是</span><span class="sxs-lookup"><span data-stu-id="a506d-236">Yes</span></span>                      | <span data-ttu-id="a506d-237">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="a506d-237">AdminAdd</span></span> |
| <span data-ttu-id="a506d-238">在于</span><span class="sxs-lookup"><span data-stu-id="a506d-238">reason</span></span>           | <span data-ttu-id="a506d-239">String</span><span class="sxs-lookup"><span data-stu-id="a506d-239">String</span></span>                                                   | <span data-ttu-id="a506d-240">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="a506d-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="a506d-241">schedule</span><span class="sxs-lookup"><span data-stu-id="a506d-241">schedule</span></span>         | [<span data-ttu-id="a506d-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a506d-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a506d-243">是</span><span class="sxs-lookup"><span data-stu-id="a506d-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="a506d-244">请求</span><span class="sxs-lookup"><span data-stu-id="a506d-244">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a506d-245">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a506d-245">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a506d-246">C#</span><span class="sxs-lookup"><span data-stu-id="a506d-246">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a506d-247">Javascript</span><span class="sxs-lookup"><span data-stu-id="a506d-247">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a506d-248">目标-C</span><span class="sxs-lookup"><span data-stu-id="a506d-248">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="a506d-249">响应</span><span class="sxs-lookup"><span data-stu-id="a506d-249">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="a506d-250">示例 2: 用户激活符合条件的角色</span><span class="sxs-lookup"><span data-stu-id="a506d-250">Example 2: User activates eligible role</span></span>

<span data-ttu-id="a506d-251">在此示例中, 用户 nawu@fimdev.net 激活符合条件的计费阅读者角色。</span><span class="sxs-lookup"><span data-stu-id="a506d-251">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="a506d-252">属性</span><span class="sxs-lookup"><span data-stu-id="a506d-252">Property</span></span>         | <span data-ttu-id="a506d-253">类型</span><span class="sxs-lookup"><span data-stu-id="a506d-253">Type</span></span>                                                     | <span data-ttu-id="a506d-254">必需</span><span class="sxs-lookup"><span data-stu-id="a506d-254">Required</span></span>                 | <span data-ttu-id="a506d-255">值</span><span class="sxs-lookup"><span data-stu-id="a506d-255">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="a506d-256">resourceId</span><span class="sxs-lookup"><span data-stu-id="a506d-256">resourceId</span></span>       | <span data-ttu-id="a506d-257">String</span><span class="sxs-lookup"><span data-stu-id="a506d-257">String</span></span>                                                   | <span data-ttu-id="a506d-258">是</span><span class="sxs-lookup"><span data-stu-id="a506d-258">Yes</span></span>                      | <span data-ttu-id="a506d-259">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a506d-259">\<resourceId\></span></span> |
| <span data-ttu-id="a506d-260">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a506d-260">roleDefinitionId</span></span> | <span data-ttu-id="a506d-261">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-261">String</span></span>                                                   | <span data-ttu-id="a506d-262">是</span><span class="sxs-lookup"><span data-stu-id="a506d-262">Yes</span></span>                      | <span data-ttu-id="a506d-263">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a506d-263">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="a506d-264">subjectId</span><span class="sxs-lookup"><span data-stu-id="a506d-264">subjectId</span></span>        | <span data-ttu-id="a506d-265">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-265">String</span></span>                                                   | <span data-ttu-id="a506d-266">是</span><span class="sxs-lookup"><span data-stu-id="a506d-266">Yes</span></span>                      | <span data-ttu-id="a506d-267">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a506d-267">\<subjectId\></span></span> |
| <span data-ttu-id="a506d-268">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a506d-268">assignmentState</span></span>  | <span data-ttu-id="a506d-269">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-269">String</span></span>                                                   | <span data-ttu-id="a506d-270">是</span><span class="sxs-lookup"><span data-stu-id="a506d-270">Yes</span></span>                      | <span data-ttu-id="a506d-271">活动</span><span class="sxs-lookup"><span data-stu-id="a506d-271">Active</span></span> |
| <span data-ttu-id="a506d-272">type</span><span class="sxs-lookup"><span data-stu-id="a506d-272">type</span></span>             | <span data-ttu-id="a506d-273">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-273">String</span></span>                                                   | <span data-ttu-id="a506d-274">是</span><span class="sxs-lookup"><span data-stu-id="a506d-274">Yes</span></span>                      | <span data-ttu-id="a506d-275">UserAdd</span><span class="sxs-lookup"><span data-stu-id="a506d-275">UserAdd</span></span> |
| <span data-ttu-id="a506d-276">在于</span><span class="sxs-lookup"><span data-stu-id="a506d-276">reason</span></span>           | <span data-ttu-id="a506d-277">String</span><span class="sxs-lookup"><span data-stu-id="a506d-277">String</span></span>                                                   | <span data-ttu-id="a506d-278">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="a506d-278">depends on role Settings</span></span> |   |
| <span data-ttu-id="a506d-279">schedule</span><span class="sxs-lookup"><span data-stu-id="a506d-279">schedule</span></span>         | [<span data-ttu-id="a506d-280">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a506d-280">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a506d-281">是</span><span class="sxs-lookup"><span data-stu-id="a506d-281">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="a506d-282">请求</span><span class="sxs-lookup"><span data-stu-id="a506d-282">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="a506d-283">响应</span><span class="sxs-lookup"><span data-stu-id="a506d-283">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="a506d-284">示例 3: 用户停用分配的角色</span><span class="sxs-lookup"><span data-stu-id="a506d-284">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="a506d-285">在此示例中, 用户 nawu@fimdev.net 停用活动的帐单阅读者角色。</span><span class="sxs-lookup"><span data-stu-id="a506d-285">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="a506d-286">属性</span><span class="sxs-lookup"><span data-stu-id="a506d-286">Property</span></span>         | <span data-ttu-id="a506d-287">类型</span><span class="sxs-lookup"><span data-stu-id="a506d-287">Type</span></span>                                                     | <span data-ttu-id="a506d-288">必需</span><span class="sxs-lookup"><span data-stu-id="a506d-288">Required</span></span> | <span data-ttu-id="a506d-289">值</span><span class="sxs-lookup"><span data-stu-id="a506d-289">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="a506d-290">resourceId</span><span class="sxs-lookup"><span data-stu-id="a506d-290">resourceId</span></span>       | <span data-ttu-id="a506d-291">String</span><span class="sxs-lookup"><span data-stu-id="a506d-291">String</span></span>                                                   | <span data-ttu-id="a506d-292">是</span><span class="sxs-lookup"><span data-stu-id="a506d-292">Yes</span></span>      | <span data-ttu-id="a506d-293">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a506d-293">\<resourceId\></span></span> |
| <span data-ttu-id="a506d-294">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a506d-294">roleDefinitionId</span></span> | <span data-ttu-id="a506d-295">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-295">String</span></span>                                                   | <span data-ttu-id="a506d-296">是</span><span class="sxs-lookup"><span data-stu-id="a506d-296">Yes</span></span>      | <span data-ttu-id="a506d-297">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a506d-297">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="a506d-298">subjectId</span><span class="sxs-lookup"><span data-stu-id="a506d-298">subjectId</span></span>        | <span data-ttu-id="a506d-299">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-299">String</span></span>                                                   | <span data-ttu-id="a506d-300">是</span><span class="sxs-lookup"><span data-stu-id="a506d-300">Yes</span></span>      | <span data-ttu-id="a506d-301">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a506d-301">\<subjectId\></span></span> |
| <span data-ttu-id="a506d-302">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a506d-302">assignmentState</span></span>  | <span data-ttu-id="a506d-303">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-303">String</span></span>                                                   | <span data-ttu-id="a506d-304">是</span><span class="sxs-lookup"><span data-stu-id="a506d-304">Yes</span></span>      | <span data-ttu-id="a506d-305">活动</span><span class="sxs-lookup"><span data-stu-id="a506d-305">Active</span></span> |
| <span data-ttu-id="a506d-306">type</span><span class="sxs-lookup"><span data-stu-id="a506d-306">type</span></span>             | <span data-ttu-id="a506d-307">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-307">String</span></span>                                                   | <span data-ttu-id="a506d-308">是</span><span class="sxs-lookup"><span data-stu-id="a506d-308">Yes</span></span>      | <span data-ttu-id="a506d-309">UserRemove</span><span class="sxs-lookup"><span data-stu-id="a506d-309">UserRemove</span></span> |
| <span data-ttu-id="a506d-310">在于</span><span class="sxs-lookup"><span data-stu-id="a506d-310">reason</span></span>           | <span data-ttu-id="a506d-311">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-311">String</span></span>                                                   | <span data-ttu-id="a506d-312">否</span><span class="sxs-lookup"><span data-stu-id="a506d-312">No</span></span>       |   |
| <span data-ttu-id="a506d-313">schedule</span><span class="sxs-lookup"><span data-stu-id="a506d-313">schedule</span></span>         | [<span data-ttu-id="a506d-314">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a506d-314">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a506d-315">否</span><span class="sxs-lookup"><span data-stu-id="a506d-315">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="a506d-316">请求</span><span class="sxs-lookup"><span data-stu-id="a506d-316">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="a506d-317">响应</span><span class="sxs-lookup"><span data-stu-id="a506d-317">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="a506d-318">示例 4: 管理员从角色中删除用户</span><span class="sxs-lookup"><span data-stu-id="a506d-318">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="a506d-319">在此示例中, 管理员从 "计费读者" 角色中删除用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="a506d-319">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="a506d-320">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="a506d-320">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="a506d-321">属性</span><span class="sxs-lookup"><span data-stu-id="a506d-321">Property</span></span>         | <span data-ttu-id="a506d-322">类型</span><span class="sxs-lookup"><span data-stu-id="a506d-322">Type</span></span>                                                     | <span data-ttu-id="a506d-323">必需</span><span class="sxs-lookup"><span data-stu-id="a506d-323">Required</span></span> | <span data-ttu-id="a506d-324">值</span><span class="sxs-lookup"><span data-stu-id="a506d-324">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="a506d-325">resourceId</span><span class="sxs-lookup"><span data-stu-id="a506d-325">resourceId</span></span>       | <span data-ttu-id="a506d-326">String</span><span class="sxs-lookup"><span data-stu-id="a506d-326">String</span></span>                                                   | <span data-ttu-id="a506d-327">是</span><span class="sxs-lookup"><span data-stu-id="a506d-327">Yes</span></span>      | <span data-ttu-id="a506d-328">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a506d-328">\<resourceId\></span></span> |
| <span data-ttu-id="a506d-329">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a506d-329">roleDefinitionId</span></span> | <span data-ttu-id="a506d-330">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-330">String</span></span>                                                   | <span data-ttu-id="a506d-331">是</span><span class="sxs-lookup"><span data-stu-id="a506d-331">Yes</span></span>      | <span data-ttu-id="a506d-332">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a506d-332">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="a506d-333">subjectId</span><span class="sxs-lookup"><span data-stu-id="a506d-333">subjectId</span></span>        | <span data-ttu-id="a506d-334">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-334">String</span></span>                                                   | <span data-ttu-id="a506d-335">是</span><span class="sxs-lookup"><span data-stu-id="a506d-335">Yes</span></span>      | <span data-ttu-id="a506d-336">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a506d-336">\<subjectId\></span></span> |
| <span data-ttu-id="a506d-337">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a506d-337">assignmentState</span></span>  | <span data-ttu-id="a506d-338">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-338">String</span></span>                                                   | <span data-ttu-id="a506d-339">是</span><span class="sxs-lookup"><span data-stu-id="a506d-339">Yes</span></span>      | <span data-ttu-id="a506d-340">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="a506d-340">Eligible / Active</span></span> |
| <span data-ttu-id="a506d-341">type</span><span class="sxs-lookup"><span data-stu-id="a506d-341">type</span></span>             | <span data-ttu-id="a506d-342">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-342">String</span></span>                                                   | <span data-ttu-id="a506d-343">是</span><span class="sxs-lookup"><span data-stu-id="a506d-343">Yes</span></span>      | <span data-ttu-id="a506d-344">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="a506d-344">AdminRemove</span></span> |
| <span data-ttu-id="a506d-345">在于</span><span class="sxs-lookup"><span data-stu-id="a506d-345">reason</span></span>           | <span data-ttu-id="a506d-346">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-346">String</span></span>                                                   | <span data-ttu-id="a506d-347">否</span><span class="sxs-lookup"><span data-stu-id="a506d-347">No</span></span>       |   |
| <span data-ttu-id="a506d-348">schedule</span><span class="sxs-lookup"><span data-stu-id="a506d-348">schedule</span></span>         | [<span data-ttu-id="a506d-349">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a506d-349">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a506d-350">否</span><span class="sxs-lookup"><span data-stu-id="a506d-350">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="a506d-351">请求</span><span class="sxs-lookup"><span data-stu-id="a506d-351">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="a506d-352">响应</span><span class="sxs-lookup"><span data-stu-id="a506d-352">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="a506d-353">示例 5: 管理员更新角色分配</span><span class="sxs-lookup"><span data-stu-id="a506d-353">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="a506d-354">在此示例中, 管理员将用户 nawu@fimdev.net 的角色分配更新为 "所有者"。</span><span class="sxs-lookup"><span data-stu-id="a506d-354">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="a506d-355">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="a506d-355">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="a506d-356">属性</span><span class="sxs-lookup"><span data-stu-id="a506d-356">Property</span></span>         | <span data-ttu-id="a506d-357">类型</span><span class="sxs-lookup"><span data-stu-id="a506d-357">Type</span></span>                                                     | <span data-ttu-id="a506d-358">必需</span><span class="sxs-lookup"><span data-stu-id="a506d-358">Required</span></span>                | <span data-ttu-id="a506d-359">值</span><span class="sxs-lookup"><span data-stu-id="a506d-359">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="a506d-360">resourceId</span><span class="sxs-lookup"><span data-stu-id="a506d-360">resourceId</span></span>       | <span data-ttu-id="a506d-361">String</span><span class="sxs-lookup"><span data-stu-id="a506d-361">String</span></span>                                                   | <span data-ttu-id="a506d-362">是</span><span class="sxs-lookup"><span data-stu-id="a506d-362">Yes</span></span>                     | <span data-ttu-id="a506d-363">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a506d-363">\<resourceId\></span></span> |
| <span data-ttu-id="a506d-364">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a506d-364">roleDefinitionId</span></span> | <span data-ttu-id="a506d-365">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-365">String</span></span>                                                   | <span data-ttu-id="a506d-366">是</span><span class="sxs-lookup"><span data-stu-id="a506d-366">Yes</span></span>                     | <span data-ttu-id="a506d-367">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a506d-367">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="a506d-368">subjectId</span><span class="sxs-lookup"><span data-stu-id="a506d-368">subjectId</span></span>        | <span data-ttu-id="a506d-369">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-369">String</span></span>                                                   | <span data-ttu-id="a506d-370">是</span><span class="sxs-lookup"><span data-stu-id="a506d-370">Yes</span></span>                     | <span data-ttu-id="a506d-371">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a506d-371">\<subjectId\></span></span> |
| <span data-ttu-id="a506d-372">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a506d-372">assignmentState</span></span>  | <span data-ttu-id="a506d-373">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-373">String</span></span>                                                   | <span data-ttu-id="a506d-374">是</span><span class="sxs-lookup"><span data-stu-id="a506d-374">Yes</span></span>                     | <span data-ttu-id="a506d-375">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="a506d-375">Eligible / Active</span></span> |
| <span data-ttu-id="a506d-376">type</span><span class="sxs-lookup"><span data-stu-id="a506d-376">type</span></span>             | <span data-ttu-id="a506d-377">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-377">String</span></span>                                                   | <span data-ttu-id="a506d-378">是</span><span class="sxs-lookup"><span data-stu-id="a506d-378">Yes</span></span>                     | <span data-ttu-id="a506d-379">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="a506d-379">AdminUpdate</span></span> |
| <span data-ttu-id="a506d-380">在于</span><span class="sxs-lookup"><span data-stu-id="a506d-380">reason</span></span>           | <span data-ttu-id="a506d-381">String</span><span class="sxs-lookup"><span data-stu-id="a506d-381">String</span></span>                                                   | <span data-ttu-id="a506d-382">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="a506d-382">depends on roleSettings</span></span> |   |
| <span data-ttu-id="a506d-383">schedule</span><span class="sxs-lookup"><span data-stu-id="a506d-383">schedule</span></span>         | [<span data-ttu-id="a506d-384">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a506d-384">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a506d-385">是</span><span class="sxs-lookup"><span data-stu-id="a506d-385">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="a506d-386">请求</span><span class="sxs-lookup"><span data-stu-id="a506d-386">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="a506d-387">响应</span><span class="sxs-lookup"><span data-stu-id="a506d-387">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="a506d-388">示例 6: 管理员扩展了即将过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="a506d-388">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="a506d-389">此示例将用户 ANUJCUSER 的过期角色分配扩展到 API Management Service 参与者。</span><span class="sxs-lookup"><span data-stu-id="a506d-389">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="a506d-390">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="a506d-390">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="a506d-391">属性</span><span class="sxs-lookup"><span data-stu-id="a506d-391">Property</span></span>         | <span data-ttu-id="a506d-392">类型</span><span class="sxs-lookup"><span data-stu-id="a506d-392">Type</span></span>                                                     | <span data-ttu-id="a506d-393">必需</span><span class="sxs-lookup"><span data-stu-id="a506d-393">Required</span></span>                | <span data-ttu-id="a506d-394">值</span><span class="sxs-lookup"><span data-stu-id="a506d-394">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="a506d-395">resourceId</span><span class="sxs-lookup"><span data-stu-id="a506d-395">resourceId</span></span>       | <span data-ttu-id="a506d-396">String</span><span class="sxs-lookup"><span data-stu-id="a506d-396">String</span></span>                                                   | <span data-ttu-id="a506d-397">是</span><span class="sxs-lookup"><span data-stu-id="a506d-397">Yes</span></span>                     | <span data-ttu-id="a506d-398">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a506d-398">\<resourceId\></span></span> |
| <span data-ttu-id="a506d-399">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a506d-399">roleDefinitionId</span></span> | <span data-ttu-id="a506d-400">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-400">String</span></span>                                                   | <span data-ttu-id="a506d-401">是</span><span class="sxs-lookup"><span data-stu-id="a506d-401">Yes</span></span>                     | <span data-ttu-id="a506d-402">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a506d-402">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="a506d-403">subjectId</span><span class="sxs-lookup"><span data-stu-id="a506d-403">subjectId</span></span>        | <span data-ttu-id="a506d-404">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-404">String</span></span>                                                   | <span data-ttu-id="a506d-405">是</span><span class="sxs-lookup"><span data-stu-id="a506d-405">Yes</span></span>                     | <span data-ttu-id="a506d-406">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a506d-406">\<subjectId\></span></span> |
| <span data-ttu-id="a506d-407">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a506d-407">assignmentState</span></span>  | <span data-ttu-id="a506d-408">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-408">String</span></span>                                                   | <span data-ttu-id="a506d-409">是</span><span class="sxs-lookup"><span data-stu-id="a506d-409">Yes</span></span>                     | <span data-ttu-id="a506d-410">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="a506d-410">Eligible / Active</span></span> |
| <span data-ttu-id="a506d-411">type</span><span class="sxs-lookup"><span data-stu-id="a506d-411">type</span></span>             | <span data-ttu-id="a506d-412">字符串</span><span class="sxs-lookup"><span data-stu-id="a506d-412">String</span></span>                                                   | <span data-ttu-id="a506d-413">是</span><span class="sxs-lookup"><span data-stu-id="a506d-413">Yes</span></span>                     | <span data-ttu-id="a506d-414">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="a506d-414">AdminExtend</span></span> |
| <span data-ttu-id="a506d-415">在于</span><span class="sxs-lookup"><span data-stu-id="a506d-415">reason</span></span>           | <span data-ttu-id="a506d-416">String</span><span class="sxs-lookup"><span data-stu-id="a506d-416">String</span></span>                                                   | <span data-ttu-id="a506d-417">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="a506d-417">depends on roleSettings</span></span> |   |
| <span data-ttu-id="a506d-418">schedule</span><span class="sxs-lookup"><span data-stu-id="a506d-418">schedule</span></span>         | [<span data-ttu-id="a506d-419">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a506d-419">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a506d-420">是</span><span class="sxs-lookup"><span data-stu-id="a506d-420">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="a506d-421">请求</span><span class="sxs-lookup"><span data-stu-id="a506d-421">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="a506d-422">响应</span><span class="sxs-lookup"><span data-stu-id="a506d-422">Response</span></span>

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
  ]
}
-->
