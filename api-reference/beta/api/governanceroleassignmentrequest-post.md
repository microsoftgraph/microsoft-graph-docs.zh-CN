---
title: 创建 governanceRoleAssignmentRequest
description: 创建一个角色分配请求，以代表在角色分配上所需的操作。 下表列出了这些操作。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: b038ca74eb8046e4ae77a8a31715a473a3518ba1
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218869"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="22557-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="22557-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="22557-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22557-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22557-106">创建一个角色分配请求，以代表在角色分配上所需的操作。</span><span class="sxs-lookup"><span data-stu-id="22557-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="22557-107">下表列出了这些操作。</span><span class="sxs-lookup"><span data-stu-id="22557-107">The following table lists the operations.</span></span>

| <span data-ttu-id="22557-108">Operation</span><span class="sxs-lookup"><span data-stu-id="22557-108">Operation</span></span>                                   | <span data-ttu-id="22557-109">类型</span><span class="sxs-lookup"><span data-stu-id="22557-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="22557-110">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="22557-110">Assign a role assignment</span></span>                    | <span data-ttu-id="22557-111">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="22557-111">AdminAdd</span></span>    |
| <span data-ttu-id="22557-112">激活符合条件的角色分配</span><span class="sxs-lookup"><span data-stu-id="22557-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="22557-113">UserAdd</span><span class="sxs-lookup"><span data-stu-id="22557-113">UserAdd</span></span>     |
| <span data-ttu-id="22557-114">停用已激活的角色分配</span><span class="sxs-lookup"><span data-stu-id="22557-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="22557-115">UserRemove</span><span class="sxs-lookup"><span data-stu-id="22557-115">UserRemove</span></span>  |
| <span data-ttu-id="22557-116">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="22557-116">Remove a role assignment</span></span>                    | <span data-ttu-id="22557-117">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="22557-117">AdminRemove</span></span> |
| <span data-ttu-id="22557-118">更新角色分配</span><span class="sxs-lookup"><span data-stu-id="22557-118">Update a role assignment</span></span>                    | <span data-ttu-id="22557-119">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="22557-119">AdminUpdate</span></span> |
| <span data-ttu-id="22557-120">请求扩展我的角色分配</span><span class="sxs-lookup"><span data-stu-id="22557-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="22557-121">UserExtend</span><span class="sxs-lookup"><span data-stu-id="22557-121">UserExtend</span></span>  |
| <span data-ttu-id="22557-122">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="22557-122">Extend a role assignment</span></span>                    | <span data-ttu-id="22557-123">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="22557-123">AdminExtend</span></span> |
| <span data-ttu-id="22557-124">续订我的过期角色分配的请求</span><span class="sxs-lookup"><span data-stu-id="22557-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="22557-125">UserRenew</span><span class="sxs-lookup"><span data-stu-id="22557-125">UserRenew</span></span>   |
| <span data-ttu-id="22557-126">续订过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="22557-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="22557-127">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="22557-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="22557-128">Permissions</span><span class="sxs-lookup"><span data-stu-id="22557-128">Permissions</span></span>

<span data-ttu-id="22557-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22557-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22557-131">权限类型</span><span class="sxs-lookup"><span data-stu-id="22557-131">Permission type</span></span>                        | <span data-ttu-id="22557-132">Permissions</span><span class="sxs-lookup"><span data-stu-id="22557-132">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="22557-133">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22557-133">Delegated (work or school account)</span></span>     | <span data-ttu-id="22557-134">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="22557-134">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="22557-135">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22557-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22557-136">不支持。</span><span class="sxs-lookup"><span data-stu-id="22557-136">Not supported.</span></span>                            |
| <span data-ttu-id="22557-137">应用程序</span><span class="sxs-lookup"><span data-stu-id="22557-137">Application</span></span>                            | <span data-ttu-id="22557-138">不支持。</span><span class="sxs-lookup"><span data-stu-id="22557-138">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22557-139">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22557-139">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="22557-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="22557-140">Request headers</span></span>

| <span data-ttu-id="22557-141">名称</span><span class="sxs-lookup"><span data-stu-id="22557-141">Name</span></span>          | <span data-ttu-id="22557-142">说明</span><span class="sxs-lookup"><span data-stu-id="22557-142">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="22557-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="22557-143">Authorization</span></span> | <span data-ttu-id="22557-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="22557-144">Bearer {code}</span></span>    |
| <span data-ttu-id="22557-145">Content-type</span><span class="sxs-lookup"><span data-stu-id="22557-145">Content-type</span></span>  | <span data-ttu-id="22557-146">application/json</span><span class="sxs-lookup"><span data-stu-id="22557-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="22557-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="22557-147">Request body</span></span>

<span data-ttu-id="22557-148">在请求正文中，提供[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22557-148">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="22557-149">属性</span><span class="sxs-lookup"><span data-stu-id="22557-149">Property</span></span>         | <span data-ttu-id="22557-150">类型</span><span class="sxs-lookup"><span data-stu-id="22557-150">Type</span></span>                                                     | <span data-ttu-id="22557-151">说明</span><span class="sxs-lookup"><span data-stu-id="22557-151">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="22557-152">resourceId</span><span class="sxs-lookup"><span data-stu-id="22557-152">resourceId</span></span>       | <span data-ttu-id="22557-153">String</span><span class="sxs-lookup"><span data-stu-id="22557-153">String</span></span>                                                   | <span data-ttu-id="22557-154">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="22557-154">The ID of the resource.</span></span> <span data-ttu-id="22557-155">必需。</span><span class="sxs-lookup"><span data-stu-id="22557-155">Required.</span></span> |
| <span data-ttu-id="22557-156">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="22557-156">roleDefinitionId</span></span> | <span data-ttu-id="22557-157">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-157">String</span></span>                                                   | <span data-ttu-id="22557-158">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="22557-158">The ID of the role definition.</span></span> <span data-ttu-id="22557-159">必需。</span><span class="sxs-lookup"><span data-stu-id="22557-159">Required.</span></span> |
| <span data-ttu-id="22557-160">subjectId</span><span class="sxs-lookup"><span data-stu-id="22557-160">subjectId</span></span>        | <span data-ttu-id="22557-161">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-161">String</span></span>                                                   | <span data-ttu-id="22557-162">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="22557-162">The ID of the subject.</span></span> <span data-ttu-id="22557-163">必需。</span><span class="sxs-lookup"><span data-stu-id="22557-163">Required.</span></span> |
| <span data-ttu-id="22557-164">assignmentState</span><span class="sxs-lookup"><span data-stu-id="22557-164">assignmentState</span></span>  | <span data-ttu-id="22557-165">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-165">String</span></span>                                                   | <span data-ttu-id="22557-166">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="22557-166">The state of assignment.</span></span> <span data-ttu-id="22557-167">值可以是`Eligible`和`Active`。</span><span class="sxs-lookup"><span data-stu-id="22557-167">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="22557-168">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="22557-168">Required.</span></span> |
| <span data-ttu-id="22557-169">type</span><span class="sxs-lookup"><span data-stu-id="22557-169">type</span></span>             | <span data-ttu-id="22557-170">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-170">String</span></span>                                                   | <span data-ttu-id="22557-171">请求类型。</span><span class="sxs-lookup"><span data-stu-id="22557-171">The request type.</span></span> <span data-ttu-id="22557-172">值可以是`AdminAdd` `UserAdd`、、 `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `AdminRenew` `AdminExtend`、、、、和。 `UserRenew`</span><span class="sxs-lookup"><span data-stu-id="22557-172">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="22557-173">必需。</span><span class="sxs-lookup"><span data-stu-id="22557-173">Required.</span></span> |
| <span data-ttu-id="22557-174">reason</span><span class="sxs-lookup"><span data-stu-id="22557-174">reason</span></span>           | <span data-ttu-id="22557-175">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-175">String</span></span>                                                   | <span data-ttu-id="22557-176">需要为角色分配请求提供审核和审阅目的的原因。</span><span class="sxs-lookup"><span data-stu-id="22557-176">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="22557-177">schedule</span><span class="sxs-lookup"><span data-stu-id="22557-177">schedule</span></span>         | [<span data-ttu-id="22557-178">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="22557-178">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="22557-179">角色分配请求的日程安排。</span><span class="sxs-lookup"><span data-stu-id="22557-179">The schedule of the role assignment request.</span></span> <span data-ttu-id="22557-180">对于的请求类型`UserAdd`， `AdminAdd` `AdminUpdate`、和`AdminExtend`，它是必需的。</span><span class="sxs-lookup"><span data-stu-id="22557-180">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="22557-181">响应</span><span class="sxs-lookup"><span data-stu-id="22557-181">Response</span></span>

<span data-ttu-id="22557-182">如果成功，此方法在响应`201 Created`正文中返回响应代码和[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="22557-182">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="22557-183">错误代码</span><span class="sxs-lookup"><span data-stu-id="22557-183">Error codes</span></span>

<span data-ttu-id="22557-184">此 API 返回标准的 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="22557-184">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="22557-185">此外，它还返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="22557-185">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="22557-186">错误代码</span><span class="sxs-lookup"><span data-stu-id="22557-186">Error code</span></span>     | <span data-ttu-id="22557-187">错误消息</span><span class="sxs-lookup"><span data-stu-id="22557-187">Error message</span></span>                               | <span data-ttu-id="22557-188">详细信息</span><span class="sxs-lookup"><span data-stu-id="22557-188">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="22557-189">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22557-189">400 BadRequest</span></span> | <span data-ttu-id="22557-190">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="22557-190">RoleNotFound</span></span>                                | <span data-ttu-id="22557-191">找`roleDefinitionId`不到请求正文中提供的。</span><span class="sxs-lookup"><span data-stu-id="22557-191">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="22557-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22557-192">400 BadRequest</span></span> | <span data-ttu-id="22557-193">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="22557-193">ResourceIsLocked</span></span>                            | <span data-ttu-id="22557-194">请求正文中提供的资源处于状态`Locked` ，并且无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="22557-194">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="22557-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22557-195">400 BadRequest</span></span> | <span data-ttu-id="22557-196">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="22557-196">SubjectNotFound</span></span>                             | <span data-ttu-id="22557-197">找`subjectId`不到请求正文中提供的。</span><span class="sxs-lookup"><span data-stu-id="22557-197">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="22557-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22557-198">400 BadRequest</span></span> | <span data-ttu-id="22557-199">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="22557-199">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="22557-200">系统中已存在一个挂起的[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 。</span><span class="sxs-lookup"><span data-stu-id="22557-200">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="22557-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22557-201">400 BadRequest</span></span> | <span data-ttu-id="22557-202">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="22557-202">RoleAssignmentExists</span></span>                        | <span data-ttu-id="22557-203">系统中已存在请求创建的[governanceRoleAssignment](../resources/governanceroleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="22557-203">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="22557-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22557-204">400 BadRequest</span></span> | <span data-ttu-id="22557-205">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="22557-205">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="22557-206">系统中不存在请求进行更新/扩展的[governanceRoleAssignment](../resources/governanceroleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="22557-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="22557-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="22557-207">400 BadRequest</span></span> | <span data-ttu-id="22557-208">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="22557-208">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="22557-209">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部策略，因此无法创建。</span><span class="sxs-lookup"><span data-stu-id="22557-209">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="22557-210">示例</span><span class="sxs-lookup"><span data-stu-id="22557-210">Examples</span></span>

<span data-ttu-id="22557-211">下面的示例演示如何使用此 API。</span><span class="sxs-lookup"><span data-stu-id="22557-211">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="22557-212">示例1：管理员为用户分配角色</span><span class="sxs-lookup"><span data-stu-id="22557-212">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="22557-213">在此示例中，管理员向计费读者角色分配用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="22557-213">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="22557-214">**注意：** 除了权限之外，此示例还要求请求者在资源上至少有一个`Active`管理员角色分配（`owner`或`user access administrator`）。</span><span class="sxs-lookup"><span data-stu-id="22557-214">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="22557-215">属性</span><span class="sxs-lookup"><span data-stu-id="22557-215">Property</span></span>         | <span data-ttu-id="22557-216">类型</span><span class="sxs-lookup"><span data-stu-id="22557-216">Type</span></span>                                                     | <span data-ttu-id="22557-217">必需</span><span class="sxs-lookup"><span data-stu-id="22557-217">Required</span></span>                 | <span data-ttu-id="22557-218">值</span><span class="sxs-lookup"><span data-stu-id="22557-218">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="22557-219">resourceId</span><span class="sxs-lookup"><span data-stu-id="22557-219">resourceId</span></span>       | <span data-ttu-id="22557-220">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-220">String</span></span>                                                   | <span data-ttu-id="22557-221">是</span><span class="sxs-lookup"><span data-stu-id="22557-221">Yes</span></span>                      | <span data-ttu-id="22557-222">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="22557-222">\<resourceId\></span></span> |
| <span data-ttu-id="22557-223">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="22557-223">roleDefinitionId</span></span> | <span data-ttu-id="22557-224">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-224">String</span></span>                                                   | <span data-ttu-id="22557-225">是</span><span class="sxs-lookup"><span data-stu-id="22557-225">Yes</span></span>                      | <span data-ttu-id="22557-226">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="22557-226">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="22557-227">subjectId</span><span class="sxs-lookup"><span data-stu-id="22557-227">subjectId</span></span>        | <span data-ttu-id="22557-228">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-228">String</span></span>                                                   | <span data-ttu-id="22557-229">是</span><span class="sxs-lookup"><span data-stu-id="22557-229">Yes</span></span>                      | <span data-ttu-id="22557-230">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="22557-230">\<subjectId\></span></span> |
| <span data-ttu-id="22557-231">assignmentState</span><span class="sxs-lookup"><span data-stu-id="22557-231">assignmentState</span></span>  | <span data-ttu-id="22557-232">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-232">String</span></span>                                                   | <span data-ttu-id="22557-233">是</span><span class="sxs-lookup"><span data-stu-id="22557-233">Yes</span></span>                      | <span data-ttu-id="22557-234">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="22557-234">Eligible / Active</span></span> |
| <span data-ttu-id="22557-235">type</span><span class="sxs-lookup"><span data-stu-id="22557-235">type</span></span>             | <span data-ttu-id="22557-236">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-236">String</span></span>                                                   | <span data-ttu-id="22557-237">是</span><span class="sxs-lookup"><span data-stu-id="22557-237">Yes</span></span>                      | <span data-ttu-id="22557-238">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="22557-238">AdminAdd</span></span> |
| <span data-ttu-id="22557-239">reason</span><span class="sxs-lookup"><span data-stu-id="22557-239">reason</span></span>           | <span data-ttu-id="22557-240">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-240">String</span></span>                                                   | <span data-ttu-id="22557-241">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="22557-241">depends on role Settings</span></span> |   |
| <span data-ttu-id="22557-242">schedule</span><span class="sxs-lookup"><span data-stu-id="22557-242">schedule</span></span>         | [<span data-ttu-id="22557-243">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="22557-243">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="22557-244">是</span><span class="sxs-lookup"><span data-stu-id="22557-244">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="22557-245">请求</span><span class="sxs-lookup"><span data-stu-id="22557-245">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="22557-246">HTTP</span><span class="sxs-lookup"><span data-stu-id="22557-246">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="22557-247">C#</span><span class="sxs-lookup"><span data-stu-id="22557-247">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22557-248">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22557-248">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22557-249">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22557-249">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="22557-250">响应</span><span class="sxs-lookup"><span data-stu-id="22557-250">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="22557-251">示例2：用户激活符合条件的角色</span><span class="sxs-lookup"><span data-stu-id="22557-251">Example 2: User activates eligible role</span></span>

<span data-ttu-id="22557-252">在此示例中，用户 nawu@fimdev.net 激活符合条件的计费阅读者角色。</span><span class="sxs-lookup"><span data-stu-id="22557-252">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="22557-253">属性</span><span class="sxs-lookup"><span data-stu-id="22557-253">Property</span></span>         | <span data-ttu-id="22557-254">类型</span><span class="sxs-lookup"><span data-stu-id="22557-254">Type</span></span>                                                     | <span data-ttu-id="22557-255">必需</span><span class="sxs-lookup"><span data-stu-id="22557-255">Required</span></span>                 | <span data-ttu-id="22557-256">值</span><span class="sxs-lookup"><span data-stu-id="22557-256">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="22557-257">resourceId</span><span class="sxs-lookup"><span data-stu-id="22557-257">resourceId</span></span>       | <span data-ttu-id="22557-258">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-258">String</span></span>                                                   | <span data-ttu-id="22557-259">是</span><span class="sxs-lookup"><span data-stu-id="22557-259">Yes</span></span>                      | <span data-ttu-id="22557-260">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="22557-260">\<resourceId\></span></span> |
| <span data-ttu-id="22557-261">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="22557-261">roleDefinitionId</span></span> | <span data-ttu-id="22557-262">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-262">String</span></span>                                                   | <span data-ttu-id="22557-263">是</span><span class="sxs-lookup"><span data-stu-id="22557-263">Yes</span></span>                      | <span data-ttu-id="22557-264">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="22557-264">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="22557-265">subjectId</span><span class="sxs-lookup"><span data-stu-id="22557-265">subjectId</span></span>        | <span data-ttu-id="22557-266">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-266">String</span></span>                                                   | <span data-ttu-id="22557-267">是</span><span class="sxs-lookup"><span data-stu-id="22557-267">Yes</span></span>                      | <span data-ttu-id="22557-268">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="22557-268">\<subjectId\></span></span> |
| <span data-ttu-id="22557-269">assignmentState</span><span class="sxs-lookup"><span data-stu-id="22557-269">assignmentState</span></span>  | <span data-ttu-id="22557-270">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-270">String</span></span>                                                   | <span data-ttu-id="22557-271">是</span><span class="sxs-lookup"><span data-stu-id="22557-271">Yes</span></span>                      | <span data-ttu-id="22557-272">活动</span><span class="sxs-lookup"><span data-stu-id="22557-272">Active</span></span> |
| <span data-ttu-id="22557-273">type</span><span class="sxs-lookup"><span data-stu-id="22557-273">type</span></span>             | <span data-ttu-id="22557-274">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-274">String</span></span>                                                   | <span data-ttu-id="22557-275">是</span><span class="sxs-lookup"><span data-stu-id="22557-275">Yes</span></span>                      | <span data-ttu-id="22557-276">UserAdd</span><span class="sxs-lookup"><span data-stu-id="22557-276">UserAdd</span></span> |
| <span data-ttu-id="22557-277">reason</span><span class="sxs-lookup"><span data-stu-id="22557-277">reason</span></span>           | <span data-ttu-id="22557-278">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-278">String</span></span>                                                   | <span data-ttu-id="22557-279">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="22557-279">depends on role Settings</span></span> |   |
| <span data-ttu-id="22557-280">schedule</span><span class="sxs-lookup"><span data-stu-id="22557-280">schedule</span></span>         | [<span data-ttu-id="22557-281">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="22557-281">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="22557-282">是</span><span class="sxs-lookup"><span data-stu-id="22557-282">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="22557-283">请求</span><span class="sxs-lookup"><span data-stu-id="22557-283">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="22557-284">响应</span><span class="sxs-lookup"><span data-stu-id="22557-284">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="22557-285">示例3：用户停用分配的角色</span><span class="sxs-lookup"><span data-stu-id="22557-285">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="22557-286">在此示例中，用户 nawu@fimdev.net 停用活动的帐单阅读者角色。</span><span class="sxs-lookup"><span data-stu-id="22557-286">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="22557-287">属性</span><span class="sxs-lookup"><span data-stu-id="22557-287">Property</span></span>         | <span data-ttu-id="22557-288">类型</span><span class="sxs-lookup"><span data-stu-id="22557-288">Type</span></span>                                                     | <span data-ttu-id="22557-289">必需</span><span class="sxs-lookup"><span data-stu-id="22557-289">Required</span></span> | <span data-ttu-id="22557-290">值</span><span class="sxs-lookup"><span data-stu-id="22557-290">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="22557-291">resourceId</span><span class="sxs-lookup"><span data-stu-id="22557-291">resourceId</span></span>       | <span data-ttu-id="22557-292">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-292">String</span></span>                                                   | <span data-ttu-id="22557-293">是</span><span class="sxs-lookup"><span data-stu-id="22557-293">Yes</span></span>      | <span data-ttu-id="22557-294">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="22557-294">\<resourceId\></span></span> |
| <span data-ttu-id="22557-295">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="22557-295">roleDefinitionId</span></span> | <span data-ttu-id="22557-296">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-296">String</span></span>                                                   | <span data-ttu-id="22557-297">是</span><span class="sxs-lookup"><span data-stu-id="22557-297">Yes</span></span>      | <span data-ttu-id="22557-298">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="22557-298">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="22557-299">subjectId</span><span class="sxs-lookup"><span data-stu-id="22557-299">subjectId</span></span>        | <span data-ttu-id="22557-300">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-300">String</span></span>                                                   | <span data-ttu-id="22557-301">是</span><span class="sxs-lookup"><span data-stu-id="22557-301">Yes</span></span>      | <span data-ttu-id="22557-302">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="22557-302">\<subjectId\></span></span> |
| <span data-ttu-id="22557-303">assignmentState</span><span class="sxs-lookup"><span data-stu-id="22557-303">assignmentState</span></span>  | <span data-ttu-id="22557-304">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-304">String</span></span>                                                   | <span data-ttu-id="22557-305">是</span><span class="sxs-lookup"><span data-stu-id="22557-305">Yes</span></span>      | <span data-ttu-id="22557-306">活动</span><span class="sxs-lookup"><span data-stu-id="22557-306">Active</span></span> |
| <span data-ttu-id="22557-307">type</span><span class="sxs-lookup"><span data-stu-id="22557-307">type</span></span>             | <span data-ttu-id="22557-308">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-308">String</span></span>                                                   | <span data-ttu-id="22557-309">是</span><span class="sxs-lookup"><span data-stu-id="22557-309">Yes</span></span>      | <span data-ttu-id="22557-310">UserRemove</span><span class="sxs-lookup"><span data-stu-id="22557-310">UserRemove</span></span> |
| <span data-ttu-id="22557-311">reason</span><span class="sxs-lookup"><span data-stu-id="22557-311">reason</span></span>           | <span data-ttu-id="22557-312">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-312">String</span></span>                                                   | <span data-ttu-id="22557-313">否</span><span class="sxs-lookup"><span data-stu-id="22557-313">No</span></span>       |   |
| <span data-ttu-id="22557-314">schedule</span><span class="sxs-lookup"><span data-stu-id="22557-314">schedule</span></span>         | [<span data-ttu-id="22557-315">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="22557-315">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="22557-316">否</span><span class="sxs-lookup"><span data-stu-id="22557-316">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="22557-317">请求</span><span class="sxs-lookup"><span data-stu-id="22557-317">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="22557-318">响应</span><span class="sxs-lookup"><span data-stu-id="22557-318">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="22557-319">示例4：管理员从角色中删除用户</span><span class="sxs-lookup"><span data-stu-id="22557-319">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="22557-320">在此示例中，管理员从 "计费读者" 角色中删除用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="22557-320">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="22557-321">**注意：** 除了权限之外，此示例还要求请求者在资源上至少有一个`Active`管理员角色分配（`owner`或`user access administrator`）。</span><span class="sxs-lookup"><span data-stu-id="22557-321">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="22557-322">属性</span><span class="sxs-lookup"><span data-stu-id="22557-322">Property</span></span>         | <span data-ttu-id="22557-323">类型</span><span class="sxs-lookup"><span data-stu-id="22557-323">Type</span></span>                                                     | <span data-ttu-id="22557-324">必需</span><span class="sxs-lookup"><span data-stu-id="22557-324">Required</span></span> | <span data-ttu-id="22557-325">值</span><span class="sxs-lookup"><span data-stu-id="22557-325">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="22557-326">resourceId</span><span class="sxs-lookup"><span data-stu-id="22557-326">resourceId</span></span>       | <span data-ttu-id="22557-327">String</span><span class="sxs-lookup"><span data-stu-id="22557-327">String</span></span>                                                   | <span data-ttu-id="22557-328">是</span><span class="sxs-lookup"><span data-stu-id="22557-328">Yes</span></span>      | <span data-ttu-id="22557-329">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="22557-329">\<resourceId\></span></span> |
| <span data-ttu-id="22557-330">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="22557-330">roleDefinitionId</span></span> | <span data-ttu-id="22557-331">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-331">String</span></span>                                                   | <span data-ttu-id="22557-332">是</span><span class="sxs-lookup"><span data-stu-id="22557-332">Yes</span></span>      | <span data-ttu-id="22557-333">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="22557-333">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="22557-334">subjectId</span><span class="sxs-lookup"><span data-stu-id="22557-334">subjectId</span></span>        | <span data-ttu-id="22557-335">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-335">String</span></span>                                                   | <span data-ttu-id="22557-336">是</span><span class="sxs-lookup"><span data-stu-id="22557-336">Yes</span></span>      | <span data-ttu-id="22557-337">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="22557-337">\<subjectId\></span></span> |
| <span data-ttu-id="22557-338">assignmentState</span><span class="sxs-lookup"><span data-stu-id="22557-338">assignmentState</span></span>  | <span data-ttu-id="22557-339">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-339">String</span></span>                                                   | <span data-ttu-id="22557-340">是</span><span class="sxs-lookup"><span data-stu-id="22557-340">Yes</span></span>      | <span data-ttu-id="22557-341">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="22557-341">Eligible / Active</span></span> |
| <span data-ttu-id="22557-342">type</span><span class="sxs-lookup"><span data-stu-id="22557-342">type</span></span>             | <span data-ttu-id="22557-343">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-343">String</span></span>                                                   | <span data-ttu-id="22557-344">是</span><span class="sxs-lookup"><span data-stu-id="22557-344">Yes</span></span>      | <span data-ttu-id="22557-345">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="22557-345">AdminRemove</span></span> |
| <span data-ttu-id="22557-346">reason</span><span class="sxs-lookup"><span data-stu-id="22557-346">reason</span></span>           | <span data-ttu-id="22557-347">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-347">String</span></span>                                                   | <span data-ttu-id="22557-348">否</span><span class="sxs-lookup"><span data-stu-id="22557-348">No</span></span>       |   |
| <span data-ttu-id="22557-349">schedule</span><span class="sxs-lookup"><span data-stu-id="22557-349">schedule</span></span>         | [<span data-ttu-id="22557-350">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="22557-350">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="22557-351">否</span><span class="sxs-lookup"><span data-stu-id="22557-351">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="22557-352">请求</span><span class="sxs-lookup"><span data-stu-id="22557-352">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="22557-353">响应</span><span class="sxs-lookup"><span data-stu-id="22557-353">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="22557-354">示例5：管理员更新角色分配</span><span class="sxs-lookup"><span data-stu-id="22557-354">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="22557-355">在此示例中，管理员将用户 nawu@fimdev.net 的角色分配更新为 "所有者"。</span><span class="sxs-lookup"><span data-stu-id="22557-355">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="22557-356">**注意：** 除了权限之外，此示例还要求请求者在资源上至少有一个`Active`管理员角色分配（`owner`或`user access administrator`）。</span><span class="sxs-lookup"><span data-stu-id="22557-356">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="22557-357">属性</span><span class="sxs-lookup"><span data-stu-id="22557-357">Property</span></span>         | <span data-ttu-id="22557-358">类型</span><span class="sxs-lookup"><span data-stu-id="22557-358">Type</span></span>                                                     | <span data-ttu-id="22557-359">必需</span><span class="sxs-lookup"><span data-stu-id="22557-359">Required</span></span>                | <span data-ttu-id="22557-360">值</span><span class="sxs-lookup"><span data-stu-id="22557-360">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="22557-361">resourceId</span><span class="sxs-lookup"><span data-stu-id="22557-361">resourceId</span></span>       | <span data-ttu-id="22557-362">String</span><span class="sxs-lookup"><span data-stu-id="22557-362">String</span></span>                                                   | <span data-ttu-id="22557-363">是</span><span class="sxs-lookup"><span data-stu-id="22557-363">Yes</span></span>                     | <span data-ttu-id="22557-364">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="22557-364">\<resourceId\></span></span> |
| <span data-ttu-id="22557-365">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="22557-365">roleDefinitionId</span></span> | <span data-ttu-id="22557-366">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-366">String</span></span>                                                   | <span data-ttu-id="22557-367">是</span><span class="sxs-lookup"><span data-stu-id="22557-367">Yes</span></span>                     | <span data-ttu-id="22557-368">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="22557-368">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="22557-369">subjectId</span><span class="sxs-lookup"><span data-stu-id="22557-369">subjectId</span></span>        | <span data-ttu-id="22557-370">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-370">String</span></span>                                                   | <span data-ttu-id="22557-371">是</span><span class="sxs-lookup"><span data-stu-id="22557-371">Yes</span></span>                     | <span data-ttu-id="22557-372">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="22557-372">\<subjectId\></span></span> |
| <span data-ttu-id="22557-373">assignmentState</span><span class="sxs-lookup"><span data-stu-id="22557-373">assignmentState</span></span>  | <span data-ttu-id="22557-374">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-374">String</span></span>                                                   | <span data-ttu-id="22557-375">是</span><span class="sxs-lookup"><span data-stu-id="22557-375">Yes</span></span>                     | <span data-ttu-id="22557-376">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="22557-376">Eligible / Active</span></span> |
| <span data-ttu-id="22557-377">type</span><span class="sxs-lookup"><span data-stu-id="22557-377">type</span></span>             | <span data-ttu-id="22557-378">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-378">String</span></span>                                                   | <span data-ttu-id="22557-379">是</span><span class="sxs-lookup"><span data-stu-id="22557-379">Yes</span></span>                     | <span data-ttu-id="22557-380">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="22557-380">AdminUpdate</span></span> |
| <span data-ttu-id="22557-381">reason</span><span class="sxs-lookup"><span data-stu-id="22557-381">reason</span></span>           | <span data-ttu-id="22557-382">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-382">String</span></span>                                                   | <span data-ttu-id="22557-383">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="22557-383">depends on roleSettings</span></span> |   |
| <span data-ttu-id="22557-384">schedule</span><span class="sxs-lookup"><span data-stu-id="22557-384">schedule</span></span>         | [<span data-ttu-id="22557-385">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="22557-385">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="22557-386">是</span><span class="sxs-lookup"><span data-stu-id="22557-386">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="22557-387">请求</span><span class="sxs-lookup"><span data-stu-id="22557-387">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="22557-388">响应</span><span class="sxs-lookup"><span data-stu-id="22557-388">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="22557-389">示例6：管理员扩展了即将过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="22557-389">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="22557-390">此示例将用户 ANUJCUSER 的过期角色分配扩展到 API Management Service 参与者。</span><span class="sxs-lookup"><span data-stu-id="22557-390">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="22557-391">**注意：** 除了权限之外，此示例还要求请求者在资源上至少有一个`Active`管理员角色分配（`owner`或`user access administrator`）。</span><span class="sxs-lookup"><span data-stu-id="22557-391">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="22557-392">属性</span><span class="sxs-lookup"><span data-stu-id="22557-392">Property</span></span>         | <span data-ttu-id="22557-393">类型</span><span class="sxs-lookup"><span data-stu-id="22557-393">Type</span></span>                                                     | <span data-ttu-id="22557-394">必需</span><span class="sxs-lookup"><span data-stu-id="22557-394">Required</span></span>                | <span data-ttu-id="22557-395">值</span><span class="sxs-lookup"><span data-stu-id="22557-395">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="22557-396">resourceId</span><span class="sxs-lookup"><span data-stu-id="22557-396">resourceId</span></span>       | <span data-ttu-id="22557-397">String</span><span class="sxs-lookup"><span data-stu-id="22557-397">String</span></span>                                                   | <span data-ttu-id="22557-398">是</span><span class="sxs-lookup"><span data-stu-id="22557-398">Yes</span></span>                     | <span data-ttu-id="22557-399">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="22557-399">\<resourceId\></span></span> |
| <span data-ttu-id="22557-400">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="22557-400">roleDefinitionId</span></span> | <span data-ttu-id="22557-401">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-401">String</span></span>                                                   | <span data-ttu-id="22557-402">是</span><span class="sxs-lookup"><span data-stu-id="22557-402">Yes</span></span>                     | <span data-ttu-id="22557-403">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="22557-403">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="22557-404">subjectId</span><span class="sxs-lookup"><span data-stu-id="22557-404">subjectId</span></span>        | <span data-ttu-id="22557-405">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-405">String</span></span>                                                   | <span data-ttu-id="22557-406">是</span><span class="sxs-lookup"><span data-stu-id="22557-406">Yes</span></span>                     | <span data-ttu-id="22557-407">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="22557-407">\<subjectId\></span></span> |
| <span data-ttu-id="22557-408">assignmentState</span><span class="sxs-lookup"><span data-stu-id="22557-408">assignmentState</span></span>  | <span data-ttu-id="22557-409">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-409">String</span></span>                                                   | <span data-ttu-id="22557-410">是</span><span class="sxs-lookup"><span data-stu-id="22557-410">Yes</span></span>                     | <span data-ttu-id="22557-411">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="22557-411">Eligible / Active</span></span> |
| <span data-ttu-id="22557-412">type</span><span class="sxs-lookup"><span data-stu-id="22557-412">type</span></span>             | <span data-ttu-id="22557-413">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-413">String</span></span>                                                   | <span data-ttu-id="22557-414">是</span><span class="sxs-lookup"><span data-stu-id="22557-414">Yes</span></span>                     | <span data-ttu-id="22557-415">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="22557-415">AdminExtend</span></span> |
| <span data-ttu-id="22557-416">reason</span><span class="sxs-lookup"><span data-stu-id="22557-416">reason</span></span>           | <span data-ttu-id="22557-417">字符串</span><span class="sxs-lookup"><span data-stu-id="22557-417">String</span></span>                                                   | <span data-ttu-id="22557-418">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="22557-418">depends on roleSettings</span></span> |   |
| <span data-ttu-id="22557-419">schedule</span><span class="sxs-lookup"><span data-stu-id="22557-419">schedule</span></span>         | [<span data-ttu-id="22557-420">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="22557-420">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="22557-421">是</span><span class="sxs-lookup"><span data-stu-id="22557-421">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="22557-422">请求</span><span class="sxs-lookup"><span data-stu-id="22557-422">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="22557-423">响应</span><span class="sxs-lookup"><span data-stu-id="22557-423">Response</span></span>

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
