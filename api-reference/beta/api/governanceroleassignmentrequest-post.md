---
title: 创建 governanceRoleAssignmentRequest
description: 创建一个角色分配请求, 以代表在角色分配上所需的操作。 下表列出了这些操作。
localization_priority: Normal
ms.openlocfilehash: b9b5f701f3f8ad283f589d07b250ce8ea63aa479
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329611"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="5f03d-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="5f03d-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f03d-105">创建一个角色分配请求, 以代表在角色分配上所需的操作。</span><span class="sxs-lookup"><span data-stu-id="5f03d-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="5f03d-106">下表列出了这些操作。</span><span class="sxs-lookup"><span data-stu-id="5f03d-106">The following table lists the operations.</span></span>

| <span data-ttu-id="5f03d-107">操作</span><span class="sxs-lookup"><span data-stu-id="5f03d-107">Operation</span></span>                                   | <span data-ttu-id="5f03d-108">类型</span><span class="sxs-lookup"><span data-stu-id="5f03d-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="5f03d-109">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="5f03d-109">Assign a role assignment</span></span>                    | <span data-ttu-id="5f03d-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="5f03d-110">AdminAdd</span></span>    |
| <span data-ttu-id="5f03d-111">激活符合条件的角色分配</span><span class="sxs-lookup"><span data-stu-id="5f03d-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="5f03d-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="5f03d-112">UserAdd</span></span>     |
| <span data-ttu-id="5f03d-113">停用已激活的角色分配</span><span class="sxs-lookup"><span data-stu-id="5f03d-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="5f03d-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="5f03d-114">UserRemove</span></span>  |
| <span data-ttu-id="5f03d-115">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="5f03d-115">Remove a role assignment</span></span>                    | <span data-ttu-id="5f03d-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="5f03d-116">AdminRemove</span></span> |
| <span data-ttu-id="5f03d-117">更新角色分配</span><span class="sxs-lookup"><span data-stu-id="5f03d-117">Update a role assignment</span></span>                    | <span data-ttu-id="5f03d-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="5f03d-118">AdminUpdate</span></span> |
| <span data-ttu-id="5f03d-119">请求扩展我的角色分配</span><span class="sxs-lookup"><span data-stu-id="5f03d-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="5f03d-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="5f03d-120">UserExtend</span></span>  |
| <span data-ttu-id="5f03d-121">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="5f03d-121">Extend a role assignment</span></span>                    | <span data-ttu-id="5f03d-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="5f03d-122">AdminExtend</span></span> |
| <span data-ttu-id="5f03d-123">续订我的过期角色分配的请求</span><span class="sxs-lookup"><span data-stu-id="5f03d-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="5f03d-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="5f03d-124">UserRenew</span></span>   |
| <span data-ttu-id="5f03d-125">续订过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="5f03d-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="5f03d-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="5f03d-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="5f03d-127">权限</span><span class="sxs-lookup"><span data-stu-id="5f03d-127">Permissions</span></span>

<span data-ttu-id="5f03d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f03d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5f03d-130">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f03d-130">Permission type</span></span>                        | <span data-ttu-id="5f03d-131">权限</span><span class="sxs-lookup"><span data-stu-id="5f03d-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="5f03d-132">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f03d-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f03d-133">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="5f03d-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="5f03d-134">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f03d-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f03d-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f03d-135">Not supported.</span></span>                            |
| <span data-ttu-id="5f03d-136">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f03d-136">Application</span></span>                            | <span data-ttu-id="5f03d-137">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="5f03d-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f03d-138">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f03d-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="5f03d-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f03d-139">Request headers</span></span>

| <span data-ttu-id="5f03d-140">名称</span><span class="sxs-lookup"><span data-stu-id="5f03d-140">Name</span></span>          | <span data-ttu-id="5f03d-141">说明</span><span class="sxs-lookup"><span data-stu-id="5f03d-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="5f03d-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f03d-142">Authorization</span></span> | <span data-ttu-id="5f03d-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5f03d-143">Bearer {code}</span></span>    |
| <span data-ttu-id="5f03d-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="5f03d-144">Content-type</span></span>  | <span data-ttu-id="5f03d-145">application/json</span><span class="sxs-lookup"><span data-stu-id="5f03d-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f03d-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f03d-146">Request body</span></span>

<span data-ttu-id="5f03d-147">在请求正文中, 提供[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f03d-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="5f03d-148">属性</span><span class="sxs-lookup"><span data-stu-id="5f03d-148">Property</span></span>         | <span data-ttu-id="5f03d-149">类型</span><span class="sxs-lookup"><span data-stu-id="5f03d-149">Type</span></span>                                                     | <span data-ttu-id="5f03d-150">说明</span><span class="sxs-lookup"><span data-stu-id="5f03d-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="5f03d-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="5f03d-151">resourceId</span></span>       | <span data-ttu-id="5f03d-152">String</span><span class="sxs-lookup"><span data-stu-id="5f03d-152">String</span></span>                                                   | <span data-ttu-id="5f03d-153">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="5f03d-153">The ID of the resource.</span></span> <span data-ttu-id="5f03d-154">必填。</span><span class="sxs-lookup"><span data-stu-id="5f03d-154">Required.</span></span> |
| <span data-ttu-id="5f03d-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5f03d-155">roleDefinitionId</span></span> | <span data-ttu-id="5f03d-156">String</span><span class="sxs-lookup"><span data-stu-id="5f03d-156">String</span></span>                                                   | <span data-ttu-id="5f03d-157">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="5f03d-157">The ID of the role definition.</span></span> <span data-ttu-id="5f03d-158">必填。</span><span class="sxs-lookup"><span data-stu-id="5f03d-158">Required.</span></span> |
| <span data-ttu-id="5f03d-159">subjectId</span><span class="sxs-lookup"><span data-stu-id="5f03d-159">subjectId</span></span>        | <span data-ttu-id="5f03d-160">String</span><span class="sxs-lookup"><span data-stu-id="5f03d-160">String</span></span>                                                   | <span data-ttu-id="5f03d-161">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="5f03d-161">The ID of the subject.</span></span> <span data-ttu-id="5f03d-162">必填。</span><span class="sxs-lookup"><span data-stu-id="5f03d-162">Required.</span></span> |
| <span data-ttu-id="5f03d-163">assignmentState</span><span class="sxs-lookup"><span data-stu-id="5f03d-163">assignmentState</span></span>  | <span data-ttu-id="5f03d-164">String</span><span class="sxs-lookup"><span data-stu-id="5f03d-164">String</span></span>                                                   | <span data-ttu-id="5f03d-165">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="5f03d-165">The state of assignment.</span></span> <span data-ttu-id="5f03d-166">值可以是`Eligible`和`Active`。</span><span class="sxs-lookup"><span data-stu-id="5f03d-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="5f03d-167">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="5f03d-167">Required.</span></span> |
| <span data-ttu-id="5f03d-168">type</span><span class="sxs-lookup"><span data-stu-id="5f03d-168">type</span></span>             | <span data-ttu-id="5f03d-169">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-169">String</span></span>                                                   | <span data-ttu-id="5f03d-170">请求类型。</span><span class="sxs-lookup"><span data-stu-id="5f03d-170">The request type.</span></span> <span data-ttu-id="5f03d-171">值可以是`AdminAdd` `UserAdd`、、 `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `AdminRenew` `AdminExtend`、、、、和。 `UserRenew`</span><span class="sxs-lookup"><span data-stu-id="5f03d-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="5f03d-172">必填。</span><span class="sxs-lookup"><span data-stu-id="5f03d-172">Required.</span></span> |
| <span data-ttu-id="5f03d-173">在于</span><span class="sxs-lookup"><span data-stu-id="5f03d-173">reason</span></span>           | <span data-ttu-id="5f03d-174">String</span><span class="sxs-lookup"><span data-stu-id="5f03d-174">String</span></span>                                                   | <span data-ttu-id="5f03d-175">需要为角色分配请求提供审核和审阅目的的原因。</span><span class="sxs-lookup"><span data-stu-id="5f03d-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="5f03d-176">设定</span><span class="sxs-lookup"><span data-stu-id="5f03d-176">schedule</span></span>         | [<span data-ttu-id="5f03d-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="5f03d-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="5f03d-178">角色分配请求的日程安排。</span><span class="sxs-lookup"><span data-stu-id="5f03d-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="5f03d-179">对于的请求类型`UserAdd`, `AdminAdd` `AdminUpdate`、和`AdminExtend`, 它是必需的。</span><span class="sxs-lookup"><span data-stu-id="5f03d-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="5f03d-180">响应</span><span class="sxs-lookup"><span data-stu-id="5f03d-180">Response</span></span>

<span data-ttu-id="5f03d-181">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5f03d-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="5f03d-182">错误代码</span><span class="sxs-lookup"><span data-stu-id="5f03d-182">Error codes</span></span>

<span data-ttu-id="5f03d-183">此 API 返回标准的 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="5f03d-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="5f03d-184">此外, 它还返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="5f03d-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="5f03d-185">错误代码</span><span class="sxs-lookup"><span data-stu-id="5f03d-185">Error code</span></span>     | <span data-ttu-id="5f03d-186">错误消息</span><span class="sxs-lookup"><span data-stu-id="5f03d-186">Error message</span></span>                               | <span data-ttu-id="5f03d-187">详细信息</span><span class="sxs-lookup"><span data-stu-id="5f03d-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="5f03d-188">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="5f03d-188">400 BadRequest</span></span> | <span data-ttu-id="5f03d-189">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="5f03d-189">RoleNotFound</span></span>                                | <span data-ttu-id="5f03d-190">找`roleDefinitionId`不到请求正文中提供的。</span><span class="sxs-lookup"><span data-stu-id="5f03d-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="5f03d-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="5f03d-191">400 BadRequest</span></span> | <span data-ttu-id="5f03d-192">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="5f03d-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="5f03d-193">请求正文中提供的资源处于状态`Locked` , 并且无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="5f03d-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="5f03d-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="5f03d-194">400 BadRequest</span></span> | <span data-ttu-id="5f03d-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="5f03d-195">SubjectNotFound</span></span>                             | <span data-ttu-id="5f03d-196">找`subjectId`不到请求正文中提供的。</span><span class="sxs-lookup"><span data-stu-id="5f03d-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="5f03d-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="5f03d-197">400 BadRequest</span></span> | <span data-ttu-id="5f03d-198">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="5f03d-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="5f03d-199">系统中已存在一个挂起的[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 。</span><span class="sxs-lookup"><span data-stu-id="5f03d-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="5f03d-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="5f03d-200">400 BadRequest</span></span> | <span data-ttu-id="5f03d-201">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="5f03d-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="5f03d-202">系统中已存在请求创建的[governanceRoleAssignment](../resources/governanceroleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="5f03d-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="5f03d-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="5f03d-203">400 BadRequest</span></span> | <span data-ttu-id="5f03d-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="5f03d-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="5f03d-205">系统中不存在请求进行更新/扩展的[governanceRoleAssignment](../resources/governanceroleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="5f03d-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="5f03d-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="5f03d-206">400 BadRequest</span></span> | <span data-ttu-id="5f03d-207">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="5f03d-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="5f03d-208">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部策略, 因此无法创建。</span><span class="sxs-lookup"><span data-stu-id="5f03d-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="5f03d-209">示例</span><span class="sxs-lookup"><span data-stu-id="5f03d-209">Examples</span></span>

<span data-ttu-id="5f03d-210">下面的示例演示如何使用此 API。</span><span class="sxs-lookup"><span data-stu-id="5f03d-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="5f03d-211">示例 1: 管理员为用户分配角色</span><span class="sxs-lookup"><span data-stu-id="5f03d-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="5f03d-212">在此示例中, 管理员向计费读者角色分配用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="5f03d-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="5f03d-213">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="5f03d-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="5f03d-214">属性</span><span class="sxs-lookup"><span data-stu-id="5f03d-214">Property</span></span>         | <span data-ttu-id="5f03d-215">类型</span><span class="sxs-lookup"><span data-stu-id="5f03d-215">Type</span></span>                                                     | <span data-ttu-id="5f03d-216">必需</span><span class="sxs-lookup"><span data-stu-id="5f03d-216">Required</span></span>                 | <span data-ttu-id="5f03d-217">值</span><span class="sxs-lookup"><span data-stu-id="5f03d-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="5f03d-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="5f03d-218">resourceId</span></span>       | <span data-ttu-id="5f03d-219">String</span><span class="sxs-lookup"><span data-stu-id="5f03d-219">String</span></span>                                                   | <span data-ttu-id="5f03d-220">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-220">Yes</span></span>                      | <span data-ttu-id="5f03d-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="5f03d-221">\<resourceId\></span></span> |
| <span data-ttu-id="5f03d-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5f03d-222">roleDefinitionId</span></span> | <span data-ttu-id="5f03d-223">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-223">String</span></span>                                                   | <span data-ttu-id="5f03d-224">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-224">Yes</span></span>                      | <span data-ttu-id="5f03d-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="5f03d-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="5f03d-226">subjectId</span><span class="sxs-lookup"><span data-stu-id="5f03d-226">subjectId</span></span>        | <span data-ttu-id="5f03d-227">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-227">String</span></span>                                                   | <span data-ttu-id="5f03d-228">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-228">Yes</span></span>                      | <span data-ttu-id="5f03d-229">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="5f03d-229">\<subjectId\></span></span> |
| <span data-ttu-id="5f03d-230">assignmentState</span><span class="sxs-lookup"><span data-stu-id="5f03d-230">assignmentState</span></span>  | <span data-ttu-id="5f03d-231">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-231">String</span></span>                                                   | <span data-ttu-id="5f03d-232">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-232">Yes</span></span>                      | <span data-ttu-id="5f03d-233">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="5f03d-233">Eligible / Active</span></span> |
| <span data-ttu-id="5f03d-234">type</span><span class="sxs-lookup"><span data-stu-id="5f03d-234">type</span></span>             | <span data-ttu-id="5f03d-235">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-235">String</span></span>                                                   | <span data-ttu-id="5f03d-236">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-236">Yes</span></span>                      | <span data-ttu-id="5f03d-237">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="5f03d-237">AdminAdd</span></span> |
| <span data-ttu-id="5f03d-238">在于</span><span class="sxs-lookup"><span data-stu-id="5f03d-238">reason</span></span>           | <span data-ttu-id="5f03d-239">String</span><span class="sxs-lookup"><span data-stu-id="5f03d-239">String</span></span>                                                   | <span data-ttu-id="5f03d-240">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="5f03d-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="5f03d-241">设定</span><span class="sxs-lookup"><span data-stu-id="5f03d-241">schedule</span></span>         | [<span data-ttu-id="5f03d-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="5f03d-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="5f03d-243">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="5f03d-244">请求</span><span class="sxs-lookup"><span data-stu-id="5f03d-244">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="5f03d-245">响应</span><span class="sxs-lookup"><span data-stu-id="5f03d-245">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="5f03d-246">示例 2: 用户激活符合条件的角色</span><span class="sxs-lookup"><span data-stu-id="5f03d-246">Example 2: User activates eligible role</span></span>

<span data-ttu-id="5f03d-247">在此示例中, 用户 nawu@fimdev.net 激活符合条件的计费阅读者角色。</span><span class="sxs-lookup"><span data-stu-id="5f03d-247">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="5f03d-248">属性</span><span class="sxs-lookup"><span data-stu-id="5f03d-248">Property</span></span>         | <span data-ttu-id="5f03d-249">类型</span><span class="sxs-lookup"><span data-stu-id="5f03d-249">Type</span></span>                                                     | <span data-ttu-id="5f03d-250">必需</span><span class="sxs-lookup"><span data-stu-id="5f03d-250">Required</span></span>                 | <span data-ttu-id="5f03d-251">值</span><span class="sxs-lookup"><span data-stu-id="5f03d-251">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="5f03d-252">resourceId</span><span class="sxs-lookup"><span data-stu-id="5f03d-252">resourceId</span></span>       | <span data-ttu-id="5f03d-253">String</span><span class="sxs-lookup"><span data-stu-id="5f03d-253">String</span></span>                                                   | <span data-ttu-id="5f03d-254">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-254">Yes</span></span>                      | <span data-ttu-id="5f03d-255">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="5f03d-255">\<resourceId\></span></span> |
| <span data-ttu-id="5f03d-256">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5f03d-256">roleDefinitionId</span></span> | <span data-ttu-id="5f03d-257">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-257">String</span></span>                                                   | <span data-ttu-id="5f03d-258">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-258">Yes</span></span>                      | <span data-ttu-id="5f03d-259">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="5f03d-259">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="5f03d-260">subjectId</span><span class="sxs-lookup"><span data-stu-id="5f03d-260">subjectId</span></span>        | <span data-ttu-id="5f03d-261">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-261">String</span></span>                                                   | <span data-ttu-id="5f03d-262">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-262">Yes</span></span>                      | <span data-ttu-id="5f03d-263">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="5f03d-263">\<subjectId\></span></span> |
| <span data-ttu-id="5f03d-264">assignmentState</span><span class="sxs-lookup"><span data-stu-id="5f03d-264">assignmentState</span></span>  | <span data-ttu-id="5f03d-265">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-265">String</span></span>                                                   | <span data-ttu-id="5f03d-266">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-266">Yes</span></span>                      | <span data-ttu-id="5f03d-267">可用</span><span class="sxs-lookup"><span data-stu-id="5f03d-267">Active</span></span> |
| <span data-ttu-id="5f03d-268">type</span><span class="sxs-lookup"><span data-stu-id="5f03d-268">type</span></span>             | <span data-ttu-id="5f03d-269">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-269">String</span></span>                                                   | <span data-ttu-id="5f03d-270">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-270">Yes</span></span>                      | <span data-ttu-id="5f03d-271">UserAdd</span><span class="sxs-lookup"><span data-stu-id="5f03d-271">UserAdd</span></span> |
| <span data-ttu-id="5f03d-272">在于</span><span class="sxs-lookup"><span data-stu-id="5f03d-272">reason</span></span>           | <span data-ttu-id="5f03d-273">String</span><span class="sxs-lookup"><span data-stu-id="5f03d-273">String</span></span>                                                   | <span data-ttu-id="5f03d-274">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="5f03d-274">depends on role Settings</span></span> |   |
| <span data-ttu-id="5f03d-275">设定</span><span class="sxs-lookup"><span data-stu-id="5f03d-275">schedule</span></span>         | [<span data-ttu-id="5f03d-276">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="5f03d-276">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="5f03d-277">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-277">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="5f03d-278">请求</span><span class="sxs-lookup"><span data-stu-id="5f03d-278">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="5f03d-279">响应</span><span class="sxs-lookup"><span data-stu-id="5f03d-279">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="5f03d-280">示例 3: 用户停用分配的角色</span><span class="sxs-lookup"><span data-stu-id="5f03d-280">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="5f03d-281">在此示例中, 用户 nawu@fimdev.net 停用活动的帐单阅读者角色。</span><span class="sxs-lookup"><span data-stu-id="5f03d-281">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="5f03d-282">属性</span><span class="sxs-lookup"><span data-stu-id="5f03d-282">Property</span></span>         | <span data-ttu-id="5f03d-283">类型</span><span class="sxs-lookup"><span data-stu-id="5f03d-283">Type</span></span>                                                     | <span data-ttu-id="5f03d-284">必需</span><span class="sxs-lookup"><span data-stu-id="5f03d-284">Required</span></span> | <span data-ttu-id="5f03d-285">值</span><span class="sxs-lookup"><span data-stu-id="5f03d-285">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="5f03d-286">resourceId</span><span class="sxs-lookup"><span data-stu-id="5f03d-286">resourceId</span></span>       | <span data-ttu-id="5f03d-287">String</span><span class="sxs-lookup"><span data-stu-id="5f03d-287">String</span></span>                                                   | <span data-ttu-id="5f03d-288">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-288">Yes</span></span>      | <span data-ttu-id="5f03d-289">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="5f03d-289">\<resourceId\></span></span> |
| <span data-ttu-id="5f03d-290">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5f03d-290">roleDefinitionId</span></span> | <span data-ttu-id="5f03d-291">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-291">String</span></span>                                                   | <span data-ttu-id="5f03d-292">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-292">Yes</span></span>      | <span data-ttu-id="5f03d-293">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="5f03d-293">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="5f03d-294">subjectId</span><span class="sxs-lookup"><span data-stu-id="5f03d-294">subjectId</span></span>        | <span data-ttu-id="5f03d-295">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-295">String</span></span>                                                   | <span data-ttu-id="5f03d-296">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-296">Yes</span></span>      | <span data-ttu-id="5f03d-297">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="5f03d-297">\<subjectId\></span></span> |
| <span data-ttu-id="5f03d-298">assignmentState</span><span class="sxs-lookup"><span data-stu-id="5f03d-298">assignmentState</span></span>  | <span data-ttu-id="5f03d-299">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-299">String</span></span>                                                   | <span data-ttu-id="5f03d-300">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-300">Yes</span></span>      | <span data-ttu-id="5f03d-301">可用</span><span class="sxs-lookup"><span data-stu-id="5f03d-301">Active</span></span> |
| <span data-ttu-id="5f03d-302">type</span><span class="sxs-lookup"><span data-stu-id="5f03d-302">type</span></span>             | <span data-ttu-id="5f03d-303">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-303">String</span></span>                                                   | <span data-ttu-id="5f03d-304">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-304">Yes</span></span>      | <span data-ttu-id="5f03d-305">UserRemove</span><span class="sxs-lookup"><span data-stu-id="5f03d-305">UserRemove</span></span> |
| <span data-ttu-id="5f03d-306">在于</span><span class="sxs-lookup"><span data-stu-id="5f03d-306">reason</span></span>           | <span data-ttu-id="5f03d-307">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-307">String</span></span>                                                   | <span data-ttu-id="5f03d-308">否</span><span class="sxs-lookup"><span data-stu-id="5f03d-308">No</span></span>       |   |
| <span data-ttu-id="5f03d-309">设定</span><span class="sxs-lookup"><span data-stu-id="5f03d-309">schedule</span></span>         | [<span data-ttu-id="5f03d-310">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="5f03d-310">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="5f03d-311">否</span><span class="sxs-lookup"><span data-stu-id="5f03d-311">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="5f03d-312">请求</span><span class="sxs-lookup"><span data-stu-id="5f03d-312">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="5f03d-313">响应</span><span class="sxs-lookup"><span data-stu-id="5f03d-313">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="5f03d-314">示例 4: 管理员从角色中删除用户</span><span class="sxs-lookup"><span data-stu-id="5f03d-314">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="5f03d-315">在此示例中, 管理员从 "计费读者" 角色中删除用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="5f03d-315">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="5f03d-316">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="5f03d-316">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="5f03d-317">属性</span><span class="sxs-lookup"><span data-stu-id="5f03d-317">Property</span></span>         | <span data-ttu-id="5f03d-318">类型</span><span class="sxs-lookup"><span data-stu-id="5f03d-318">Type</span></span>                                                     | <span data-ttu-id="5f03d-319">必需</span><span class="sxs-lookup"><span data-stu-id="5f03d-319">Required</span></span> | <span data-ttu-id="5f03d-320">值</span><span class="sxs-lookup"><span data-stu-id="5f03d-320">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="5f03d-321">resourceId</span><span class="sxs-lookup"><span data-stu-id="5f03d-321">resourceId</span></span>       | <span data-ttu-id="5f03d-322">String</span><span class="sxs-lookup"><span data-stu-id="5f03d-322">String</span></span>                                                   | <span data-ttu-id="5f03d-323">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-323">Yes</span></span>      | <span data-ttu-id="5f03d-324">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="5f03d-324">\<resourceId\></span></span> |
| <span data-ttu-id="5f03d-325">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5f03d-325">roleDefinitionId</span></span> | <span data-ttu-id="5f03d-326">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-326">String</span></span>                                                   | <span data-ttu-id="5f03d-327">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-327">Yes</span></span>      | <span data-ttu-id="5f03d-328">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="5f03d-328">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="5f03d-329">subjectId</span><span class="sxs-lookup"><span data-stu-id="5f03d-329">subjectId</span></span>        | <span data-ttu-id="5f03d-330">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-330">String</span></span>                                                   | <span data-ttu-id="5f03d-331">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-331">Yes</span></span>      | <span data-ttu-id="5f03d-332">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="5f03d-332">\<subjectId\></span></span> |
| <span data-ttu-id="5f03d-333">assignmentState</span><span class="sxs-lookup"><span data-stu-id="5f03d-333">assignmentState</span></span>  | <span data-ttu-id="5f03d-334">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-334">String</span></span>                                                   | <span data-ttu-id="5f03d-335">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-335">Yes</span></span>      | <span data-ttu-id="5f03d-336">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="5f03d-336">Eligible / Active</span></span> |
| <span data-ttu-id="5f03d-337">type</span><span class="sxs-lookup"><span data-stu-id="5f03d-337">type</span></span>             | <span data-ttu-id="5f03d-338">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-338">String</span></span>                                                   | <span data-ttu-id="5f03d-339">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-339">Yes</span></span>      | <span data-ttu-id="5f03d-340">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="5f03d-340">AdminRemove</span></span> |
| <span data-ttu-id="5f03d-341">在于</span><span class="sxs-lookup"><span data-stu-id="5f03d-341">reason</span></span>           | <span data-ttu-id="5f03d-342">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-342">String</span></span>                                                   | <span data-ttu-id="5f03d-343">否</span><span class="sxs-lookup"><span data-stu-id="5f03d-343">No</span></span>       |   |
| <span data-ttu-id="5f03d-344">设定</span><span class="sxs-lookup"><span data-stu-id="5f03d-344">schedule</span></span>         | [<span data-ttu-id="5f03d-345">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="5f03d-345">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="5f03d-346">否</span><span class="sxs-lookup"><span data-stu-id="5f03d-346">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="5f03d-347">请求</span><span class="sxs-lookup"><span data-stu-id="5f03d-347">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="5f03d-348">响应</span><span class="sxs-lookup"><span data-stu-id="5f03d-348">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="5f03d-349">示例 5: 管理员更新角色分配</span><span class="sxs-lookup"><span data-stu-id="5f03d-349">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="5f03d-350">在此示例中, 管理员将用户 nawu@fimdev.net 的角色分配更新为 "所有者"。</span><span class="sxs-lookup"><span data-stu-id="5f03d-350">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="5f03d-351">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="5f03d-351">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="5f03d-352">属性</span><span class="sxs-lookup"><span data-stu-id="5f03d-352">Property</span></span>         | <span data-ttu-id="5f03d-353">类型</span><span class="sxs-lookup"><span data-stu-id="5f03d-353">Type</span></span>                                                     | <span data-ttu-id="5f03d-354">必需</span><span class="sxs-lookup"><span data-stu-id="5f03d-354">Required</span></span>                | <span data-ttu-id="5f03d-355">值</span><span class="sxs-lookup"><span data-stu-id="5f03d-355">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="5f03d-356">resourceId</span><span class="sxs-lookup"><span data-stu-id="5f03d-356">resourceId</span></span>       | <span data-ttu-id="5f03d-357">String</span><span class="sxs-lookup"><span data-stu-id="5f03d-357">String</span></span>                                                   | <span data-ttu-id="5f03d-358">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-358">Yes</span></span>                     | <span data-ttu-id="5f03d-359">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="5f03d-359">\<resourceId\></span></span> |
| <span data-ttu-id="5f03d-360">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5f03d-360">roleDefinitionId</span></span> | <span data-ttu-id="5f03d-361">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-361">String</span></span>                                                   | <span data-ttu-id="5f03d-362">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-362">Yes</span></span>                     | <span data-ttu-id="5f03d-363">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="5f03d-363">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="5f03d-364">subjectId</span><span class="sxs-lookup"><span data-stu-id="5f03d-364">subjectId</span></span>        | <span data-ttu-id="5f03d-365">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-365">String</span></span>                                                   | <span data-ttu-id="5f03d-366">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-366">Yes</span></span>                     | <span data-ttu-id="5f03d-367">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="5f03d-367">\<subjectId\></span></span> |
| <span data-ttu-id="5f03d-368">assignmentState</span><span class="sxs-lookup"><span data-stu-id="5f03d-368">assignmentState</span></span>  | <span data-ttu-id="5f03d-369">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-369">String</span></span>                                                   | <span data-ttu-id="5f03d-370">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-370">Yes</span></span>                     | <span data-ttu-id="5f03d-371">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="5f03d-371">Eligible / Active</span></span> |
| <span data-ttu-id="5f03d-372">type</span><span class="sxs-lookup"><span data-stu-id="5f03d-372">type</span></span>             | <span data-ttu-id="5f03d-373">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-373">String</span></span>                                                   | <span data-ttu-id="5f03d-374">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-374">Yes</span></span>                     | <span data-ttu-id="5f03d-375">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="5f03d-375">AdminUpdate</span></span> |
| <span data-ttu-id="5f03d-376">在于</span><span class="sxs-lookup"><span data-stu-id="5f03d-376">reason</span></span>           | <span data-ttu-id="5f03d-377">String</span><span class="sxs-lookup"><span data-stu-id="5f03d-377">String</span></span>                                                   | <span data-ttu-id="5f03d-378">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="5f03d-378">depends on roleSettings</span></span> |   |
| <span data-ttu-id="5f03d-379">设定</span><span class="sxs-lookup"><span data-stu-id="5f03d-379">schedule</span></span>         | [<span data-ttu-id="5f03d-380">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="5f03d-380">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="5f03d-381">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-381">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="5f03d-382">请求</span><span class="sxs-lookup"><span data-stu-id="5f03d-382">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="5f03d-383">响应</span><span class="sxs-lookup"><span data-stu-id="5f03d-383">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="5f03d-384">示例 6: 管理员扩展了即将过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="5f03d-384">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="5f03d-385">此示例将用户 ANUJCUSER 的过期角色分配扩展到 API Management Service 参与者。</span><span class="sxs-lookup"><span data-stu-id="5f03d-385">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="5f03d-386">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="5f03d-386">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="5f03d-387">属性</span><span class="sxs-lookup"><span data-stu-id="5f03d-387">Property</span></span>         | <span data-ttu-id="5f03d-388">类型</span><span class="sxs-lookup"><span data-stu-id="5f03d-388">Type</span></span>                                                     | <span data-ttu-id="5f03d-389">必需</span><span class="sxs-lookup"><span data-stu-id="5f03d-389">Required</span></span>                | <span data-ttu-id="5f03d-390">值</span><span class="sxs-lookup"><span data-stu-id="5f03d-390">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="5f03d-391">resourceId</span><span class="sxs-lookup"><span data-stu-id="5f03d-391">resourceId</span></span>       | <span data-ttu-id="5f03d-392">String</span><span class="sxs-lookup"><span data-stu-id="5f03d-392">String</span></span>                                                   | <span data-ttu-id="5f03d-393">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-393">Yes</span></span>                     | <span data-ttu-id="5f03d-394">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="5f03d-394">\<resourceId\></span></span> |
| <span data-ttu-id="5f03d-395">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5f03d-395">roleDefinitionId</span></span> | <span data-ttu-id="5f03d-396">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-396">String</span></span>                                                   | <span data-ttu-id="5f03d-397">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-397">Yes</span></span>                     | <span data-ttu-id="5f03d-398">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="5f03d-398">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="5f03d-399">subjectId</span><span class="sxs-lookup"><span data-stu-id="5f03d-399">subjectId</span></span>        | <span data-ttu-id="5f03d-400">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-400">String</span></span>                                                   | <span data-ttu-id="5f03d-401">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-401">Yes</span></span>                     | <span data-ttu-id="5f03d-402">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="5f03d-402">\<subjectId\></span></span> |
| <span data-ttu-id="5f03d-403">assignmentState</span><span class="sxs-lookup"><span data-stu-id="5f03d-403">assignmentState</span></span>  | <span data-ttu-id="5f03d-404">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-404">String</span></span>                                                   | <span data-ttu-id="5f03d-405">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-405">Yes</span></span>                     | <span data-ttu-id="5f03d-406">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="5f03d-406">Eligible / Active</span></span> |
| <span data-ttu-id="5f03d-407">type</span><span class="sxs-lookup"><span data-stu-id="5f03d-407">type</span></span>             | <span data-ttu-id="5f03d-408">字符串</span><span class="sxs-lookup"><span data-stu-id="5f03d-408">String</span></span>                                                   | <span data-ttu-id="5f03d-409">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-409">Yes</span></span>                     | <span data-ttu-id="5f03d-410">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="5f03d-410">AdminExtend</span></span> |
| <span data-ttu-id="5f03d-411">在于</span><span class="sxs-lookup"><span data-stu-id="5f03d-411">reason</span></span>           | <span data-ttu-id="5f03d-412">String</span><span class="sxs-lookup"><span data-stu-id="5f03d-412">String</span></span>                                                   | <span data-ttu-id="5f03d-413">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="5f03d-413">depends on roleSettings</span></span> |   |
| <span data-ttu-id="5f03d-414">设定</span><span class="sxs-lookup"><span data-stu-id="5f03d-414">schedule</span></span>         | [<span data-ttu-id="5f03d-415">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="5f03d-415">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="5f03d-416">是</span><span class="sxs-lookup"><span data-stu-id="5f03d-416">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="5f03d-417">请求</span><span class="sxs-lookup"><span data-stu-id="5f03d-417">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="5f03d-418">响应</span><span class="sxs-lookup"><span data-stu-id="5f03d-418">Response</span></span>

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
  "suppressions": []
}
-->
