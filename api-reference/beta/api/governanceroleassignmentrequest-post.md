---
title: 创建 governanceRoleAssignmentRequest
description: 创建一个角色分配请求, 以代表在角色分配上所需的操作。 下表列出了这些操作。
localization_priority: Normal
ms.openlocfilehash: be27c8e0bab24f6a83e970b9aae46d0742be7c10
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422365"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="de5b3-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="de5b3-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de5b3-105">创建一个角色分配请求, 以代表在角色分配上所需的操作。</span><span class="sxs-lookup"><span data-stu-id="de5b3-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="de5b3-106">下表列出了这些操作。</span><span class="sxs-lookup"><span data-stu-id="de5b3-106">The following table lists the operations.</span></span>

| <span data-ttu-id="de5b3-107">Operation</span><span class="sxs-lookup"><span data-stu-id="de5b3-107">Operation</span></span>                                   | <span data-ttu-id="de5b3-108">类型</span><span class="sxs-lookup"><span data-stu-id="de5b3-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="de5b3-109">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="de5b3-109">Assign a role assignment</span></span>                    | <span data-ttu-id="de5b3-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="de5b3-110">AdminAdd</span></span>    |
| <span data-ttu-id="de5b3-111">激活符合条件的角色分配</span><span class="sxs-lookup"><span data-stu-id="de5b3-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="de5b3-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="de5b3-112">UserAdd</span></span>     |
| <span data-ttu-id="de5b3-113">停用已激活的角色分配</span><span class="sxs-lookup"><span data-stu-id="de5b3-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="de5b3-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="de5b3-114">UserRemove</span></span>  |
| <span data-ttu-id="de5b3-115">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="de5b3-115">Remove a role assignment</span></span>                    | <span data-ttu-id="de5b3-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="de5b3-116">AdminRemove</span></span> |
| <span data-ttu-id="de5b3-117">更新角色分配</span><span class="sxs-lookup"><span data-stu-id="de5b3-117">Update a role assignment</span></span>                    | <span data-ttu-id="de5b3-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="de5b3-118">AdminUpdate</span></span> |
| <span data-ttu-id="de5b3-119">请求扩展我的角色分配</span><span class="sxs-lookup"><span data-stu-id="de5b3-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="de5b3-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="de5b3-120">UserExtend</span></span>  |
| <span data-ttu-id="de5b3-121">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="de5b3-121">Extend a role assignment</span></span>                    | <span data-ttu-id="de5b3-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="de5b3-122">AdminExtend</span></span> |
| <span data-ttu-id="de5b3-123">续订我的过期角色分配的请求</span><span class="sxs-lookup"><span data-stu-id="de5b3-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="de5b3-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="de5b3-124">UserRenew</span></span>   |
| <span data-ttu-id="de5b3-125">续订过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="de5b3-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="de5b3-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="de5b3-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="de5b3-127">权限</span><span class="sxs-lookup"><span data-stu-id="de5b3-127">Permissions</span></span>

<span data-ttu-id="de5b3-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de5b3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de5b3-130">权限类型</span><span class="sxs-lookup"><span data-stu-id="de5b3-130">Permission type</span></span>                        | <span data-ttu-id="de5b3-131">权限</span><span class="sxs-lookup"><span data-stu-id="de5b3-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="de5b3-132">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de5b3-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="de5b3-133">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="de5b3-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="de5b3-134">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de5b3-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de5b3-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="de5b3-135">Not supported.</span></span>                            |
| <span data-ttu-id="de5b3-136">应用程序</span><span class="sxs-lookup"><span data-stu-id="de5b3-136">Application</span></span>                            | <span data-ttu-id="de5b3-137">不支持。</span><span class="sxs-lookup"><span data-stu-id="de5b3-137">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de5b3-138">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de5b3-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="de5b3-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="de5b3-139">Request headers</span></span>

| <span data-ttu-id="de5b3-140">名称</span><span class="sxs-lookup"><span data-stu-id="de5b3-140">Name</span></span>          | <span data-ttu-id="de5b3-141">说明</span><span class="sxs-lookup"><span data-stu-id="de5b3-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="de5b3-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="de5b3-142">Authorization</span></span> | <span data-ttu-id="de5b3-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="de5b3-143">Bearer {code}</span></span>    |
| <span data-ttu-id="de5b3-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="de5b3-144">Content-type</span></span>  | <span data-ttu-id="de5b3-145">application/json</span><span class="sxs-lookup"><span data-stu-id="de5b3-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="de5b3-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="de5b3-146">Request body</span></span>

<span data-ttu-id="de5b3-147">在请求正文中, 提供[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de5b3-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="de5b3-148">属性</span><span class="sxs-lookup"><span data-stu-id="de5b3-148">Property</span></span>         | <span data-ttu-id="de5b3-149">类型</span><span class="sxs-lookup"><span data-stu-id="de5b3-149">Type</span></span>                                                     | <span data-ttu-id="de5b3-150">说明</span><span class="sxs-lookup"><span data-stu-id="de5b3-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="de5b3-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="de5b3-151">resourceId</span></span>       | <span data-ttu-id="de5b3-152">String</span><span class="sxs-lookup"><span data-stu-id="de5b3-152">String</span></span>                                                   | <span data-ttu-id="de5b3-153">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="de5b3-153">The ID of the resource.</span></span> <span data-ttu-id="de5b3-154">必需。</span><span class="sxs-lookup"><span data-stu-id="de5b3-154">Required.</span></span> |
| <span data-ttu-id="de5b3-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="de5b3-155">roleDefinitionId</span></span> | <span data-ttu-id="de5b3-156">String</span><span class="sxs-lookup"><span data-stu-id="de5b3-156">String</span></span>                                                   | <span data-ttu-id="de5b3-157">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="de5b3-157">The ID of the role definition.</span></span> <span data-ttu-id="de5b3-158">必需。</span><span class="sxs-lookup"><span data-stu-id="de5b3-158">Required.</span></span> |
| <span data-ttu-id="de5b3-159">subjectId</span><span class="sxs-lookup"><span data-stu-id="de5b3-159">subjectId</span></span>        | <span data-ttu-id="de5b3-160">String</span><span class="sxs-lookup"><span data-stu-id="de5b3-160">String</span></span>                                                   | <span data-ttu-id="de5b3-161">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="de5b3-161">The ID of the subject.</span></span> <span data-ttu-id="de5b3-162">必需。</span><span class="sxs-lookup"><span data-stu-id="de5b3-162">Required.</span></span> |
| <span data-ttu-id="de5b3-163">assignmentState</span><span class="sxs-lookup"><span data-stu-id="de5b3-163">assignmentState</span></span>  | <span data-ttu-id="de5b3-164">String</span><span class="sxs-lookup"><span data-stu-id="de5b3-164">String</span></span>                                                   | <span data-ttu-id="de5b3-165">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="de5b3-165">The state of assignment.</span></span> <span data-ttu-id="de5b3-166">值可以是`Eligible`和`Active`。</span><span class="sxs-lookup"><span data-stu-id="de5b3-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="de5b3-167">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="de5b3-167">Required.</span></span> |
| <span data-ttu-id="de5b3-168">type</span><span class="sxs-lookup"><span data-stu-id="de5b3-168">type</span></span>             | <span data-ttu-id="de5b3-169">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-169">String</span></span>                                                   | <span data-ttu-id="de5b3-170">请求类型。</span><span class="sxs-lookup"><span data-stu-id="de5b3-170">The request type.</span></span> <span data-ttu-id="de5b3-171">值可以是`AdminAdd` `UserAdd`、、 `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `AdminRenew` `AdminExtend`、、、、和。 `UserRenew`</span><span class="sxs-lookup"><span data-stu-id="de5b3-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="de5b3-172">必需。</span><span class="sxs-lookup"><span data-stu-id="de5b3-172">Required.</span></span> |
| <span data-ttu-id="de5b3-173">在于</span><span class="sxs-lookup"><span data-stu-id="de5b3-173">reason</span></span>           | <span data-ttu-id="de5b3-174">String</span><span class="sxs-lookup"><span data-stu-id="de5b3-174">String</span></span>                                                   | <span data-ttu-id="de5b3-175">需要为角色分配请求提供审核和审阅目的的原因。</span><span class="sxs-lookup"><span data-stu-id="de5b3-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="de5b3-176">schedule</span><span class="sxs-lookup"><span data-stu-id="de5b3-176">schedule</span></span>         | [<span data-ttu-id="de5b3-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="de5b3-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="de5b3-178">角色分配请求的日程安排。</span><span class="sxs-lookup"><span data-stu-id="de5b3-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="de5b3-179">对于的请求类型`UserAdd`, `AdminAdd` `AdminUpdate`、和`AdminExtend`, 它是必需的。</span><span class="sxs-lookup"><span data-stu-id="de5b3-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="de5b3-180">响应</span><span class="sxs-lookup"><span data-stu-id="de5b3-180">Response</span></span>

<span data-ttu-id="de5b3-181">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="de5b3-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="de5b3-182">错误代码</span><span class="sxs-lookup"><span data-stu-id="de5b3-182">Error codes</span></span>

<span data-ttu-id="de5b3-183">此 API 返回标准的 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="de5b3-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="de5b3-184">此外, 它还返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="de5b3-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="de5b3-185">错误代码</span><span class="sxs-lookup"><span data-stu-id="de5b3-185">Error code</span></span>     | <span data-ttu-id="de5b3-186">错误消息</span><span class="sxs-lookup"><span data-stu-id="de5b3-186">Error message</span></span>                               | <span data-ttu-id="de5b3-187">详细信息</span><span class="sxs-lookup"><span data-stu-id="de5b3-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="de5b3-188">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="de5b3-188">400 BadRequest</span></span> | <span data-ttu-id="de5b3-189">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="de5b3-189">RoleNotFound</span></span>                                | <span data-ttu-id="de5b3-190">找`roleDefinitionId`不到请求正文中提供的。</span><span class="sxs-lookup"><span data-stu-id="de5b3-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="de5b3-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="de5b3-191">400 BadRequest</span></span> | <span data-ttu-id="de5b3-192">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="de5b3-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="de5b3-193">请求正文中提供的资源处于状态`Locked` , 并且无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="de5b3-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="de5b3-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="de5b3-194">400 BadRequest</span></span> | <span data-ttu-id="de5b3-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="de5b3-195">SubjectNotFound</span></span>                             | <span data-ttu-id="de5b3-196">找`subjectId`不到请求正文中提供的。</span><span class="sxs-lookup"><span data-stu-id="de5b3-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="de5b3-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="de5b3-197">400 BadRequest</span></span> | <span data-ttu-id="de5b3-198">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="de5b3-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="de5b3-199">系统中已存在一个挂起的[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 。</span><span class="sxs-lookup"><span data-stu-id="de5b3-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="de5b3-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="de5b3-200">400 BadRequest</span></span> | <span data-ttu-id="de5b3-201">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="de5b3-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="de5b3-202">系统中已存在请求创建的[governanceRoleAssignment](../resources/governanceroleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="de5b3-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="de5b3-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="de5b3-203">400 BadRequest</span></span> | <span data-ttu-id="de5b3-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="de5b3-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="de5b3-205">系统中不存在请求进行更新/扩展的[governanceRoleAssignment](../resources/governanceroleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="de5b3-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="de5b3-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="de5b3-206">400 BadRequest</span></span> | <span data-ttu-id="de5b3-207">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="de5b3-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="de5b3-208">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部策略, 因此无法创建。</span><span class="sxs-lookup"><span data-stu-id="de5b3-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="de5b3-209">示例</span><span class="sxs-lookup"><span data-stu-id="de5b3-209">Examples</span></span>

<span data-ttu-id="de5b3-210">下面的示例演示如何使用此 API。</span><span class="sxs-lookup"><span data-stu-id="de5b3-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="de5b3-211">示例 1: 管理员为用户分配角色</span><span class="sxs-lookup"><span data-stu-id="de5b3-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="de5b3-212">在此示例中, 管理员向计费读者角色分配用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="de5b3-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="de5b3-213">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="de5b3-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="de5b3-214">属性</span><span class="sxs-lookup"><span data-stu-id="de5b3-214">Property</span></span>         | <span data-ttu-id="de5b3-215">类型</span><span class="sxs-lookup"><span data-stu-id="de5b3-215">Type</span></span>                                                     | <span data-ttu-id="de5b3-216">必需</span><span class="sxs-lookup"><span data-stu-id="de5b3-216">Required</span></span>                 | <span data-ttu-id="de5b3-217">值</span><span class="sxs-lookup"><span data-stu-id="de5b3-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="de5b3-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="de5b3-218">resourceId</span></span>       | <span data-ttu-id="de5b3-219">String</span><span class="sxs-lookup"><span data-stu-id="de5b3-219">String</span></span>                                                   | <span data-ttu-id="de5b3-220">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-220">Yes</span></span>                      | <span data-ttu-id="de5b3-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="de5b3-221">\<resourceId\></span></span> |
| <span data-ttu-id="de5b3-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="de5b3-222">roleDefinitionId</span></span> | <span data-ttu-id="de5b3-223">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-223">String</span></span>                                                   | <span data-ttu-id="de5b3-224">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-224">Yes</span></span>                      | <span data-ttu-id="de5b3-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="de5b3-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="de5b3-226">subjectId</span><span class="sxs-lookup"><span data-stu-id="de5b3-226">subjectId</span></span>        | <span data-ttu-id="de5b3-227">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-227">String</span></span>                                                   | <span data-ttu-id="de5b3-228">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-228">Yes</span></span>                      | <span data-ttu-id="de5b3-229">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="de5b3-229">\<subjectId\></span></span> |
| <span data-ttu-id="de5b3-230">assignmentState</span><span class="sxs-lookup"><span data-stu-id="de5b3-230">assignmentState</span></span>  | <span data-ttu-id="de5b3-231">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-231">String</span></span>                                                   | <span data-ttu-id="de5b3-232">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-232">Yes</span></span>                      | <span data-ttu-id="de5b3-233">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="de5b3-233">Eligible / Active</span></span> |
| <span data-ttu-id="de5b3-234">type</span><span class="sxs-lookup"><span data-stu-id="de5b3-234">type</span></span>             | <span data-ttu-id="de5b3-235">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-235">String</span></span>                                                   | <span data-ttu-id="de5b3-236">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-236">Yes</span></span>                      | <span data-ttu-id="de5b3-237">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="de5b3-237">AdminAdd</span></span> |
| <span data-ttu-id="de5b3-238">在于</span><span class="sxs-lookup"><span data-stu-id="de5b3-238">reason</span></span>           | <span data-ttu-id="de5b3-239">String</span><span class="sxs-lookup"><span data-stu-id="de5b3-239">String</span></span>                                                   | <span data-ttu-id="de5b3-240">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="de5b3-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="de5b3-241">schedule</span><span class="sxs-lookup"><span data-stu-id="de5b3-241">schedule</span></span>         | [<span data-ttu-id="de5b3-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="de5b3-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="de5b3-243">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="de5b3-244">请求</span><span class="sxs-lookup"><span data-stu-id="de5b3-244">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="de5b3-245">响应</span><span class="sxs-lookup"><span data-stu-id="de5b3-245">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="de5b3-246">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="de5b3-246">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="de5b3-247">C#</span><span class="sxs-lookup"><span data-stu-id="de5b3-247">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/governanceroleassignmentrequest_post-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de5b3-248">Javascript</span><span class="sxs-lookup"><span data-stu-id="de5b3-248">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/governanceroleassignmentrequest_post-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="de5b3-249">示例 2: 用户激活符合条件的角色</span><span class="sxs-lookup"><span data-stu-id="de5b3-249">Example 2: User activates eligible role</span></span>

<span data-ttu-id="de5b3-250">在此示例中, 用户 nawu@fimdev.net 激活符合条件的计费阅读者角色。</span><span class="sxs-lookup"><span data-stu-id="de5b3-250">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="de5b3-251">属性</span><span class="sxs-lookup"><span data-stu-id="de5b3-251">Property</span></span>         | <span data-ttu-id="de5b3-252">类型</span><span class="sxs-lookup"><span data-stu-id="de5b3-252">Type</span></span>                                                     | <span data-ttu-id="de5b3-253">必需</span><span class="sxs-lookup"><span data-stu-id="de5b3-253">Required</span></span>                 | <span data-ttu-id="de5b3-254">值</span><span class="sxs-lookup"><span data-stu-id="de5b3-254">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="de5b3-255">resourceId</span><span class="sxs-lookup"><span data-stu-id="de5b3-255">resourceId</span></span>       | <span data-ttu-id="de5b3-256">String</span><span class="sxs-lookup"><span data-stu-id="de5b3-256">String</span></span>                                                   | <span data-ttu-id="de5b3-257">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-257">Yes</span></span>                      | <span data-ttu-id="de5b3-258">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="de5b3-258">\<resourceId\></span></span> |
| <span data-ttu-id="de5b3-259">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="de5b3-259">roleDefinitionId</span></span> | <span data-ttu-id="de5b3-260">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-260">String</span></span>                                                   | <span data-ttu-id="de5b3-261">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-261">Yes</span></span>                      | <span data-ttu-id="de5b3-262">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="de5b3-262">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="de5b3-263">subjectId</span><span class="sxs-lookup"><span data-stu-id="de5b3-263">subjectId</span></span>        | <span data-ttu-id="de5b3-264">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-264">String</span></span>                                                   | <span data-ttu-id="de5b3-265">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-265">Yes</span></span>                      | <span data-ttu-id="de5b3-266">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="de5b3-266">\<subjectId\></span></span> |
| <span data-ttu-id="de5b3-267">assignmentState</span><span class="sxs-lookup"><span data-stu-id="de5b3-267">assignmentState</span></span>  | <span data-ttu-id="de5b3-268">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-268">String</span></span>                                                   | <span data-ttu-id="de5b3-269">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-269">Yes</span></span>                      | <span data-ttu-id="de5b3-270">活动</span><span class="sxs-lookup"><span data-stu-id="de5b3-270">Active</span></span> |
| <span data-ttu-id="de5b3-271">type</span><span class="sxs-lookup"><span data-stu-id="de5b3-271">type</span></span>             | <span data-ttu-id="de5b3-272">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-272">String</span></span>                                                   | <span data-ttu-id="de5b3-273">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-273">Yes</span></span>                      | <span data-ttu-id="de5b3-274">UserAdd</span><span class="sxs-lookup"><span data-stu-id="de5b3-274">UserAdd</span></span> |
| <span data-ttu-id="de5b3-275">在于</span><span class="sxs-lookup"><span data-stu-id="de5b3-275">reason</span></span>           | <span data-ttu-id="de5b3-276">String</span><span class="sxs-lookup"><span data-stu-id="de5b3-276">String</span></span>                                                   | <span data-ttu-id="de5b3-277">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="de5b3-277">depends on role Settings</span></span> |   |
| <span data-ttu-id="de5b3-278">schedule</span><span class="sxs-lookup"><span data-stu-id="de5b3-278">schedule</span></span>         | [<span data-ttu-id="de5b3-279">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="de5b3-279">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="de5b3-280">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-280">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="de5b3-281">请求</span><span class="sxs-lookup"><span data-stu-id="de5b3-281">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="de5b3-282">响应</span><span class="sxs-lookup"><span data-stu-id="de5b3-282">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="de5b3-283">示例 3: 用户停用分配的角色</span><span class="sxs-lookup"><span data-stu-id="de5b3-283">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="de5b3-284">在此示例中, 用户 nawu@fimdev.net 停用活动的帐单阅读者角色。</span><span class="sxs-lookup"><span data-stu-id="de5b3-284">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="de5b3-285">属性</span><span class="sxs-lookup"><span data-stu-id="de5b3-285">Property</span></span>         | <span data-ttu-id="de5b3-286">类型</span><span class="sxs-lookup"><span data-stu-id="de5b3-286">Type</span></span>                                                     | <span data-ttu-id="de5b3-287">必需</span><span class="sxs-lookup"><span data-stu-id="de5b3-287">Required</span></span> | <span data-ttu-id="de5b3-288">值</span><span class="sxs-lookup"><span data-stu-id="de5b3-288">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="de5b3-289">resourceId</span><span class="sxs-lookup"><span data-stu-id="de5b3-289">resourceId</span></span>       | <span data-ttu-id="de5b3-290">String</span><span class="sxs-lookup"><span data-stu-id="de5b3-290">String</span></span>                                                   | <span data-ttu-id="de5b3-291">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-291">Yes</span></span>      | <span data-ttu-id="de5b3-292">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="de5b3-292">\<resourceId\></span></span> |
| <span data-ttu-id="de5b3-293">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="de5b3-293">roleDefinitionId</span></span> | <span data-ttu-id="de5b3-294">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-294">String</span></span>                                                   | <span data-ttu-id="de5b3-295">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-295">Yes</span></span>      | <span data-ttu-id="de5b3-296">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="de5b3-296">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="de5b3-297">subjectId</span><span class="sxs-lookup"><span data-stu-id="de5b3-297">subjectId</span></span>        | <span data-ttu-id="de5b3-298">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-298">String</span></span>                                                   | <span data-ttu-id="de5b3-299">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-299">Yes</span></span>      | <span data-ttu-id="de5b3-300">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="de5b3-300">\<subjectId\></span></span> |
| <span data-ttu-id="de5b3-301">assignmentState</span><span class="sxs-lookup"><span data-stu-id="de5b3-301">assignmentState</span></span>  | <span data-ttu-id="de5b3-302">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-302">String</span></span>                                                   | <span data-ttu-id="de5b3-303">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-303">Yes</span></span>      | <span data-ttu-id="de5b3-304">活动</span><span class="sxs-lookup"><span data-stu-id="de5b3-304">Active</span></span> |
| <span data-ttu-id="de5b3-305">type</span><span class="sxs-lookup"><span data-stu-id="de5b3-305">type</span></span>             | <span data-ttu-id="de5b3-306">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-306">String</span></span>                                                   | <span data-ttu-id="de5b3-307">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-307">Yes</span></span>      | <span data-ttu-id="de5b3-308">UserRemove</span><span class="sxs-lookup"><span data-stu-id="de5b3-308">UserRemove</span></span> |
| <span data-ttu-id="de5b3-309">在于</span><span class="sxs-lookup"><span data-stu-id="de5b3-309">reason</span></span>           | <span data-ttu-id="de5b3-310">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-310">String</span></span>                                                   | <span data-ttu-id="de5b3-311">否</span><span class="sxs-lookup"><span data-stu-id="de5b3-311">No</span></span>       |   |
| <span data-ttu-id="de5b3-312">schedule</span><span class="sxs-lookup"><span data-stu-id="de5b3-312">schedule</span></span>         | [<span data-ttu-id="de5b3-313">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="de5b3-313">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="de5b3-314">否</span><span class="sxs-lookup"><span data-stu-id="de5b3-314">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="de5b3-315">请求</span><span class="sxs-lookup"><span data-stu-id="de5b3-315">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="de5b3-316">响应</span><span class="sxs-lookup"><span data-stu-id="de5b3-316">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="de5b3-317">示例 4: 管理员从角色中删除用户</span><span class="sxs-lookup"><span data-stu-id="de5b3-317">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="de5b3-318">在此示例中, 管理员从 "计费读者" 角色中删除用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="de5b3-318">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="de5b3-319">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="de5b3-319">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="de5b3-320">属性</span><span class="sxs-lookup"><span data-stu-id="de5b3-320">Property</span></span>         | <span data-ttu-id="de5b3-321">类型</span><span class="sxs-lookup"><span data-stu-id="de5b3-321">Type</span></span>                                                     | <span data-ttu-id="de5b3-322">必需</span><span class="sxs-lookup"><span data-stu-id="de5b3-322">Required</span></span> | <span data-ttu-id="de5b3-323">值</span><span class="sxs-lookup"><span data-stu-id="de5b3-323">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="de5b3-324">resourceId</span><span class="sxs-lookup"><span data-stu-id="de5b3-324">resourceId</span></span>       | <span data-ttu-id="de5b3-325">String</span><span class="sxs-lookup"><span data-stu-id="de5b3-325">String</span></span>                                                   | <span data-ttu-id="de5b3-326">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-326">Yes</span></span>      | <span data-ttu-id="de5b3-327">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="de5b3-327">\<resourceId\></span></span> |
| <span data-ttu-id="de5b3-328">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="de5b3-328">roleDefinitionId</span></span> | <span data-ttu-id="de5b3-329">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-329">String</span></span>                                                   | <span data-ttu-id="de5b3-330">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-330">Yes</span></span>      | <span data-ttu-id="de5b3-331">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="de5b3-331">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="de5b3-332">subjectId</span><span class="sxs-lookup"><span data-stu-id="de5b3-332">subjectId</span></span>        | <span data-ttu-id="de5b3-333">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-333">String</span></span>                                                   | <span data-ttu-id="de5b3-334">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-334">Yes</span></span>      | <span data-ttu-id="de5b3-335">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="de5b3-335">\<subjectId\></span></span> |
| <span data-ttu-id="de5b3-336">assignmentState</span><span class="sxs-lookup"><span data-stu-id="de5b3-336">assignmentState</span></span>  | <span data-ttu-id="de5b3-337">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-337">String</span></span>                                                   | <span data-ttu-id="de5b3-338">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-338">Yes</span></span>      | <span data-ttu-id="de5b3-339">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="de5b3-339">Eligible / Active</span></span> |
| <span data-ttu-id="de5b3-340">type</span><span class="sxs-lookup"><span data-stu-id="de5b3-340">type</span></span>             | <span data-ttu-id="de5b3-341">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-341">String</span></span>                                                   | <span data-ttu-id="de5b3-342">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-342">Yes</span></span>      | <span data-ttu-id="de5b3-343">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="de5b3-343">AdminRemove</span></span> |
| <span data-ttu-id="de5b3-344">在于</span><span class="sxs-lookup"><span data-stu-id="de5b3-344">reason</span></span>           | <span data-ttu-id="de5b3-345">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-345">String</span></span>                                                   | <span data-ttu-id="de5b3-346">否</span><span class="sxs-lookup"><span data-stu-id="de5b3-346">No</span></span>       |   |
| <span data-ttu-id="de5b3-347">schedule</span><span class="sxs-lookup"><span data-stu-id="de5b3-347">schedule</span></span>         | [<span data-ttu-id="de5b3-348">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="de5b3-348">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="de5b3-349">否</span><span class="sxs-lookup"><span data-stu-id="de5b3-349">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="de5b3-350">请求</span><span class="sxs-lookup"><span data-stu-id="de5b3-350">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="de5b3-351">响应</span><span class="sxs-lookup"><span data-stu-id="de5b3-351">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="de5b3-352">示例 5: 管理员更新角色分配</span><span class="sxs-lookup"><span data-stu-id="de5b3-352">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="de5b3-353">在此示例中, 管理员将用户 nawu@fimdev.net 的角色分配更新为 "所有者"。</span><span class="sxs-lookup"><span data-stu-id="de5b3-353">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="de5b3-354">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="de5b3-354">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="de5b3-355">属性</span><span class="sxs-lookup"><span data-stu-id="de5b3-355">Property</span></span>         | <span data-ttu-id="de5b3-356">类型</span><span class="sxs-lookup"><span data-stu-id="de5b3-356">Type</span></span>                                                     | <span data-ttu-id="de5b3-357">必需</span><span class="sxs-lookup"><span data-stu-id="de5b3-357">Required</span></span>                | <span data-ttu-id="de5b3-358">值</span><span class="sxs-lookup"><span data-stu-id="de5b3-358">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="de5b3-359">resourceId</span><span class="sxs-lookup"><span data-stu-id="de5b3-359">resourceId</span></span>       | <span data-ttu-id="de5b3-360">String</span><span class="sxs-lookup"><span data-stu-id="de5b3-360">String</span></span>                                                   | <span data-ttu-id="de5b3-361">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-361">Yes</span></span>                     | <span data-ttu-id="de5b3-362">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="de5b3-362">\<resourceId\></span></span> |
| <span data-ttu-id="de5b3-363">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="de5b3-363">roleDefinitionId</span></span> | <span data-ttu-id="de5b3-364">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-364">String</span></span>                                                   | <span data-ttu-id="de5b3-365">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-365">Yes</span></span>                     | <span data-ttu-id="de5b3-366">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="de5b3-366">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="de5b3-367">subjectId</span><span class="sxs-lookup"><span data-stu-id="de5b3-367">subjectId</span></span>        | <span data-ttu-id="de5b3-368">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-368">String</span></span>                                                   | <span data-ttu-id="de5b3-369">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-369">Yes</span></span>                     | <span data-ttu-id="de5b3-370">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="de5b3-370">\<subjectId\></span></span> |
| <span data-ttu-id="de5b3-371">assignmentState</span><span class="sxs-lookup"><span data-stu-id="de5b3-371">assignmentState</span></span>  | <span data-ttu-id="de5b3-372">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-372">String</span></span>                                                   | <span data-ttu-id="de5b3-373">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-373">Yes</span></span>                     | <span data-ttu-id="de5b3-374">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="de5b3-374">Eligible / Active</span></span> |
| <span data-ttu-id="de5b3-375">type</span><span class="sxs-lookup"><span data-stu-id="de5b3-375">type</span></span>             | <span data-ttu-id="de5b3-376">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-376">String</span></span>                                                   | <span data-ttu-id="de5b3-377">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-377">Yes</span></span>                     | <span data-ttu-id="de5b3-378">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="de5b3-378">AdminUpdate</span></span> |
| <span data-ttu-id="de5b3-379">在于</span><span class="sxs-lookup"><span data-stu-id="de5b3-379">reason</span></span>           | <span data-ttu-id="de5b3-380">String</span><span class="sxs-lookup"><span data-stu-id="de5b3-380">String</span></span>                                                   | <span data-ttu-id="de5b3-381">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="de5b3-381">depends on roleSettings</span></span> |   |
| <span data-ttu-id="de5b3-382">schedule</span><span class="sxs-lookup"><span data-stu-id="de5b3-382">schedule</span></span>         | [<span data-ttu-id="de5b3-383">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="de5b3-383">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="de5b3-384">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-384">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="de5b3-385">请求</span><span class="sxs-lookup"><span data-stu-id="de5b3-385">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="de5b3-386">响应</span><span class="sxs-lookup"><span data-stu-id="de5b3-386">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="de5b3-387">示例 6: 管理员扩展了即将过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="de5b3-387">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="de5b3-388">此示例将用户 ANUJCUSER 的过期角色分配扩展到 API Management Service 参与者。</span><span class="sxs-lookup"><span data-stu-id="de5b3-388">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="de5b3-389">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="de5b3-389">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="de5b3-390">属性</span><span class="sxs-lookup"><span data-stu-id="de5b3-390">Property</span></span>         | <span data-ttu-id="de5b3-391">类型</span><span class="sxs-lookup"><span data-stu-id="de5b3-391">Type</span></span>                                                     | <span data-ttu-id="de5b3-392">必需</span><span class="sxs-lookup"><span data-stu-id="de5b3-392">Required</span></span>                | <span data-ttu-id="de5b3-393">值</span><span class="sxs-lookup"><span data-stu-id="de5b3-393">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="de5b3-394">resourceId</span><span class="sxs-lookup"><span data-stu-id="de5b3-394">resourceId</span></span>       | <span data-ttu-id="de5b3-395">String</span><span class="sxs-lookup"><span data-stu-id="de5b3-395">String</span></span>                                                   | <span data-ttu-id="de5b3-396">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-396">Yes</span></span>                     | <span data-ttu-id="de5b3-397">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="de5b3-397">\<resourceId\></span></span> |
| <span data-ttu-id="de5b3-398">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="de5b3-398">roleDefinitionId</span></span> | <span data-ttu-id="de5b3-399">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-399">String</span></span>                                                   | <span data-ttu-id="de5b3-400">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-400">Yes</span></span>                     | <span data-ttu-id="de5b3-401">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="de5b3-401">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="de5b3-402">subjectId</span><span class="sxs-lookup"><span data-stu-id="de5b3-402">subjectId</span></span>        | <span data-ttu-id="de5b3-403">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-403">String</span></span>                                                   | <span data-ttu-id="de5b3-404">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-404">Yes</span></span>                     | <span data-ttu-id="de5b3-405">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="de5b3-405">\<subjectId\></span></span> |
| <span data-ttu-id="de5b3-406">assignmentState</span><span class="sxs-lookup"><span data-stu-id="de5b3-406">assignmentState</span></span>  | <span data-ttu-id="de5b3-407">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-407">String</span></span>                                                   | <span data-ttu-id="de5b3-408">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-408">Yes</span></span>                     | <span data-ttu-id="de5b3-409">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="de5b3-409">Eligible / Active</span></span> |
| <span data-ttu-id="de5b3-410">type</span><span class="sxs-lookup"><span data-stu-id="de5b3-410">type</span></span>             | <span data-ttu-id="de5b3-411">字符串</span><span class="sxs-lookup"><span data-stu-id="de5b3-411">String</span></span>                                                   | <span data-ttu-id="de5b3-412">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-412">Yes</span></span>                     | <span data-ttu-id="de5b3-413">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="de5b3-413">AdminExtend</span></span> |
| <span data-ttu-id="de5b3-414">在于</span><span class="sxs-lookup"><span data-stu-id="de5b3-414">reason</span></span>           | <span data-ttu-id="de5b3-415">String</span><span class="sxs-lookup"><span data-stu-id="de5b3-415">String</span></span>                                                   | <span data-ttu-id="de5b3-416">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="de5b3-416">depends on roleSettings</span></span> |   |
| <span data-ttu-id="de5b3-417">schedule</span><span class="sxs-lookup"><span data-stu-id="de5b3-417">schedule</span></span>         | [<span data-ttu-id="de5b3-418">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="de5b3-418">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="de5b3-419">是</span><span class="sxs-lookup"><span data-stu-id="de5b3-419">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="de5b3-420">请求</span><span class="sxs-lookup"><span data-stu-id="de5b3-420">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="de5b3-421">响应</span><span class="sxs-lookup"><span data-stu-id="de5b3-421">Response</span></span>

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
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
