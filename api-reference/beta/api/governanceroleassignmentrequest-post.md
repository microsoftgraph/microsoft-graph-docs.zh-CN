---
title: 创建 governanceRoleAssignmentRequest
description: 创建一个角色分配请求, 以代表在角色分配上所需的操作。 下表列出了这些操作。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 7a97d5455da11db666bbd7a53f2453ed10610735
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323584"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="2e89f-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="2e89f-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e89f-105">创建一个角色分配请求, 以代表在角色分配上所需的操作。</span><span class="sxs-lookup"><span data-stu-id="2e89f-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="2e89f-106">下表列出了这些操作。</span><span class="sxs-lookup"><span data-stu-id="2e89f-106">The following table lists the operations.</span></span>

| <span data-ttu-id="2e89f-107">Operation</span><span class="sxs-lookup"><span data-stu-id="2e89f-107">Operation</span></span>                                   | <span data-ttu-id="2e89f-108">类型</span><span class="sxs-lookup"><span data-stu-id="2e89f-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="2e89f-109">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="2e89f-109">Assign a role assignment</span></span>                    | <span data-ttu-id="2e89f-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="2e89f-110">AdminAdd</span></span>    |
| <span data-ttu-id="2e89f-111">激活符合条件的角色分配</span><span class="sxs-lookup"><span data-stu-id="2e89f-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="2e89f-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="2e89f-112">UserAdd</span></span>     |
| <span data-ttu-id="2e89f-113">停用已激活的角色分配</span><span class="sxs-lookup"><span data-stu-id="2e89f-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="2e89f-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="2e89f-114">UserRemove</span></span>  |
| <span data-ttu-id="2e89f-115">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="2e89f-115">Remove a role assignment</span></span>                    | <span data-ttu-id="2e89f-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="2e89f-116">AdminRemove</span></span> |
| <span data-ttu-id="2e89f-117">更新角色分配</span><span class="sxs-lookup"><span data-stu-id="2e89f-117">Update a role assignment</span></span>                    | <span data-ttu-id="2e89f-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="2e89f-118">AdminUpdate</span></span> |
| <span data-ttu-id="2e89f-119">请求扩展我的角色分配</span><span class="sxs-lookup"><span data-stu-id="2e89f-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="2e89f-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="2e89f-120">UserExtend</span></span>  |
| <span data-ttu-id="2e89f-121">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="2e89f-121">Extend a role assignment</span></span>                    | <span data-ttu-id="2e89f-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="2e89f-122">AdminExtend</span></span> |
| <span data-ttu-id="2e89f-123">续订我的过期角色分配的请求</span><span class="sxs-lookup"><span data-stu-id="2e89f-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="2e89f-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="2e89f-124">UserRenew</span></span>   |
| <span data-ttu-id="2e89f-125">续订过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="2e89f-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="2e89f-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="2e89f-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="2e89f-127">权限</span><span class="sxs-lookup"><span data-stu-id="2e89f-127">Permissions</span></span>

<span data-ttu-id="2e89f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e89f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e89f-130">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e89f-130">Permission type</span></span>                        | <span data-ttu-id="2e89f-131">权限</span><span class="sxs-lookup"><span data-stu-id="2e89f-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="2e89f-132">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e89f-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="2e89f-133">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="2e89f-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="2e89f-134">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e89f-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e89f-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e89f-135">Not supported.</span></span>                            |
| <span data-ttu-id="2e89f-136">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e89f-136">Application</span></span>                            | <span data-ttu-id="2e89f-137">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e89f-137">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e89f-138">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e89f-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="2e89f-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e89f-139">Request headers</span></span>

| <span data-ttu-id="2e89f-140">名称</span><span class="sxs-lookup"><span data-stu-id="2e89f-140">Name</span></span>          | <span data-ttu-id="2e89f-141">说明</span><span class="sxs-lookup"><span data-stu-id="2e89f-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="2e89f-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e89f-142">Authorization</span></span> | <span data-ttu-id="2e89f-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2e89f-143">Bearer {code}</span></span>    |
| <span data-ttu-id="2e89f-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="2e89f-144">Content-type</span></span>  | <span data-ttu-id="2e89f-145">application/json</span><span class="sxs-lookup"><span data-stu-id="2e89f-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e89f-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e89f-146">Request body</span></span>

<span data-ttu-id="2e89f-147">在请求正文中, 提供[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e89f-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="2e89f-148">属性</span><span class="sxs-lookup"><span data-stu-id="2e89f-148">Property</span></span>         | <span data-ttu-id="2e89f-149">类型</span><span class="sxs-lookup"><span data-stu-id="2e89f-149">Type</span></span>                                                     | <span data-ttu-id="2e89f-150">说明</span><span class="sxs-lookup"><span data-stu-id="2e89f-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="2e89f-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="2e89f-151">resourceId</span></span>       | <span data-ttu-id="2e89f-152">String</span><span class="sxs-lookup"><span data-stu-id="2e89f-152">String</span></span>                                                   | <span data-ttu-id="2e89f-153">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="2e89f-153">The ID of the resource.</span></span> <span data-ttu-id="2e89f-154">必需。</span><span class="sxs-lookup"><span data-stu-id="2e89f-154">Required.</span></span> |
| <span data-ttu-id="2e89f-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2e89f-155">roleDefinitionId</span></span> | <span data-ttu-id="2e89f-156">String</span><span class="sxs-lookup"><span data-stu-id="2e89f-156">String</span></span>                                                   | <span data-ttu-id="2e89f-157">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="2e89f-157">The ID of the role definition.</span></span> <span data-ttu-id="2e89f-158">必需。</span><span class="sxs-lookup"><span data-stu-id="2e89f-158">Required.</span></span> |
| <span data-ttu-id="2e89f-159">subjectId</span><span class="sxs-lookup"><span data-stu-id="2e89f-159">subjectId</span></span>        | <span data-ttu-id="2e89f-160">String</span><span class="sxs-lookup"><span data-stu-id="2e89f-160">String</span></span>                                                   | <span data-ttu-id="2e89f-161">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="2e89f-161">The ID of the subject.</span></span> <span data-ttu-id="2e89f-162">必需。</span><span class="sxs-lookup"><span data-stu-id="2e89f-162">Required.</span></span> |
| <span data-ttu-id="2e89f-163">assignmentState</span><span class="sxs-lookup"><span data-stu-id="2e89f-163">assignmentState</span></span>  | <span data-ttu-id="2e89f-164">String</span><span class="sxs-lookup"><span data-stu-id="2e89f-164">String</span></span>                                                   | <span data-ttu-id="2e89f-165">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="2e89f-165">The state of assignment.</span></span> <span data-ttu-id="2e89f-166">值可以是`Eligible`和`Active`。</span><span class="sxs-lookup"><span data-stu-id="2e89f-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="2e89f-167">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="2e89f-167">Required.</span></span> |
| <span data-ttu-id="2e89f-168">type</span><span class="sxs-lookup"><span data-stu-id="2e89f-168">type</span></span>             | <span data-ttu-id="2e89f-169">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-169">String</span></span>                                                   | <span data-ttu-id="2e89f-170">请求类型。</span><span class="sxs-lookup"><span data-stu-id="2e89f-170">The request type.</span></span> <span data-ttu-id="2e89f-171">值可以是`AdminAdd` `UserAdd`、、 `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `AdminRenew` `AdminExtend`、、、、和。 `UserRenew`</span><span class="sxs-lookup"><span data-stu-id="2e89f-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="2e89f-172">必需。</span><span class="sxs-lookup"><span data-stu-id="2e89f-172">Required.</span></span> |
| <span data-ttu-id="2e89f-173">在于</span><span class="sxs-lookup"><span data-stu-id="2e89f-173">reason</span></span>           | <span data-ttu-id="2e89f-174">String</span><span class="sxs-lookup"><span data-stu-id="2e89f-174">String</span></span>                                                   | <span data-ttu-id="2e89f-175">需要为角色分配请求提供审核和审阅目的的原因。</span><span class="sxs-lookup"><span data-stu-id="2e89f-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="2e89f-176">schedule</span><span class="sxs-lookup"><span data-stu-id="2e89f-176">schedule</span></span>         | [<span data-ttu-id="2e89f-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2e89f-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="2e89f-178">角色分配请求的日程安排。</span><span class="sxs-lookup"><span data-stu-id="2e89f-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="2e89f-179">对于的请求类型`UserAdd`, `AdminAdd` `AdminUpdate`、和`AdminExtend`, 它是必需的。</span><span class="sxs-lookup"><span data-stu-id="2e89f-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="2e89f-180">响应</span><span class="sxs-lookup"><span data-stu-id="2e89f-180">Response</span></span>

<span data-ttu-id="2e89f-181">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2e89f-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="2e89f-182">错误代码</span><span class="sxs-lookup"><span data-stu-id="2e89f-182">Error codes</span></span>

<span data-ttu-id="2e89f-183">此 API 返回标准的 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="2e89f-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="2e89f-184">此外, 它还返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="2e89f-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="2e89f-185">错误代码</span><span class="sxs-lookup"><span data-stu-id="2e89f-185">Error code</span></span>     | <span data-ttu-id="2e89f-186">错误消息</span><span class="sxs-lookup"><span data-stu-id="2e89f-186">Error message</span></span>                               | <span data-ttu-id="2e89f-187">详细信息</span><span class="sxs-lookup"><span data-stu-id="2e89f-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="2e89f-188">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2e89f-188">400 BadRequest</span></span> | <span data-ttu-id="2e89f-189">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="2e89f-189">RoleNotFound</span></span>                                | <span data-ttu-id="2e89f-190">找`roleDefinitionId`不到请求正文中提供的。</span><span class="sxs-lookup"><span data-stu-id="2e89f-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="2e89f-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2e89f-191">400 BadRequest</span></span> | <span data-ttu-id="2e89f-192">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="2e89f-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="2e89f-193">请求正文中提供的资源处于状态`Locked` , 并且无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="2e89f-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="2e89f-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2e89f-194">400 BadRequest</span></span> | <span data-ttu-id="2e89f-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="2e89f-195">SubjectNotFound</span></span>                             | <span data-ttu-id="2e89f-196">找`subjectId`不到请求正文中提供的。</span><span class="sxs-lookup"><span data-stu-id="2e89f-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="2e89f-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2e89f-197">400 BadRequest</span></span> | <span data-ttu-id="2e89f-198">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="2e89f-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="2e89f-199">系统中已存在一个挂起的[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 。</span><span class="sxs-lookup"><span data-stu-id="2e89f-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="2e89f-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2e89f-200">400 BadRequest</span></span> | <span data-ttu-id="2e89f-201">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="2e89f-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="2e89f-202">系统中已存在请求创建的[governanceRoleAssignment](../resources/governanceroleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="2e89f-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="2e89f-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2e89f-203">400 BadRequest</span></span> | <span data-ttu-id="2e89f-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="2e89f-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="2e89f-205">系统中不存在请求进行更新/扩展的[governanceRoleAssignment](../resources/governanceroleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="2e89f-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="2e89f-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2e89f-206">400 BadRequest</span></span> | <span data-ttu-id="2e89f-207">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="2e89f-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="2e89f-208">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部策略, 因此无法创建。</span><span class="sxs-lookup"><span data-stu-id="2e89f-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="2e89f-209">示例</span><span class="sxs-lookup"><span data-stu-id="2e89f-209">Examples</span></span>

<span data-ttu-id="2e89f-210">下面的示例演示如何使用此 API。</span><span class="sxs-lookup"><span data-stu-id="2e89f-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="2e89f-211">示例 1: 管理员为用户分配角色</span><span class="sxs-lookup"><span data-stu-id="2e89f-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="2e89f-212">在此示例中, 管理员向计费读者角色分配用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="2e89f-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="2e89f-213">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="2e89f-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="2e89f-214">属性</span><span class="sxs-lookup"><span data-stu-id="2e89f-214">Property</span></span>         | <span data-ttu-id="2e89f-215">类型</span><span class="sxs-lookup"><span data-stu-id="2e89f-215">Type</span></span>                                                     | <span data-ttu-id="2e89f-216">必需</span><span class="sxs-lookup"><span data-stu-id="2e89f-216">Required</span></span>                 | <span data-ttu-id="2e89f-217">值</span><span class="sxs-lookup"><span data-stu-id="2e89f-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="2e89f-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="2e89f-218">resourceId</span></span>       | <span data-ttu-id="2e89f-219">String</span><span class="sxs-lookup"><span data-stu-id="2e89f-219">String</span></span>                                                   | <span data-ttu-id="2e89f-220">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-220">Yes</span></span>                      | <span data-ttu-id="2e89f-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="2e89f-221">\<resourceId\></span></span> |
| <span data-ttu-id="2e89f-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2e89f-222">roleDefinitionId</span></span> | <span data-ttu-id="2e89f-223">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-223">String</span></span>                                                   | <span data-ttu-id="2e89f-224">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-224">Yes</span></span>                      | <span data-ttu-id="2e89f-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="2e89f-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="2e89f-226">subjectId</span><span class="sxs-lookup"><span data-stu-id="2e89f-226">subjectId</span></span>        | <span data-ttu-id="2e89f-227">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-227">String</span></span>                                                   | <span data-ttu-id="2e89f-228">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-228">Yes</span></span>                      | <span data-ttu-id="2e89f-229">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="2e89f-229">\<subjectId\></span></span> |
| <span data-ttu-id="2e89f-230">assignmentState</span><span class="sxs-lookup"><span data-stu-id="2e89f-230">assignmentState</span></span>  | <span data-ttu-id="2e89f-231">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-231">String</span></span>                                                   | <span data-ttu-id="2e89f-232">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-232">Yes</span></span>                      | <span data-ttu-id="2e89f-233">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="2e89f-233">Eligible / Active</span></span> |
| <span data-ttu-id="2e89f-234">type</span><span class="sxs-lookup"><span data-stu-id="2e89f-234">type</span></span>             | <span data-ttu-id="2e89f-235">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-235">String</span></span>                                                   | <span data-ttu-id="2e89f-236">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-236">Yes</span></span>                      | <span data-ttu-id="2e89f-237">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="2e89f-237">AdminAdd</span></span> |
| <span data-ttu-id="2e89f-238">在于</span><span class="sxs-lookup"><span data-stu-id="2e89f-238">reason</span></span>           | <span data-ttu-id="2e89f-239">String</span><span class="sxs-lookup"><span data-stu-id="2e89f-239">String</span></span>                                                   | <span data-ttu-id="2e89f-240">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="2e89f-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="2e89f-241">schedule</span><span class="sxs-lookup"><span data-stu-id="2e89f-241">schedule</span></span>         | [<span data-ttu-id="2e89f-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2e89f-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="2e89f-243">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="2e89f-244">请求</span><span class="sxs-lookup"><span data-stu-id="2e89f-244">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2e89f-245">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2e89f-245">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2e89f-246">C#</span><span class="sxs-lookup"><span data-stu-id="2e89f-246">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2e89f-247">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e89f-247">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2e89f-248">目标-C</span><span class="sxs-lookup"><span data-stu-id="2e89f-248">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2e89f-249">Java</span><span class="sxs-lookup"><span data-stu-id="2e89f-249">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="2e89f-250">响应</span><span class="sxs-lookup"><span data-stu-id="2e89f-250">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="2e89f-251">示例 2: 用户激活符合条件的角色</span><span class="sxs-lookup"><span data-stu-id="2e89f-251">Example 2: User activates eligible role</span></span>

<span data-ttu-id="2e89f-252">在此示例中, 用户 nawu@fimdev.net 激活符合条件的计费阅读者角色。</span><span class="sxs-lookup"><span data-stu-id="2e89f-252">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="2e89f-253">属性</span><span class="sxs-lookup"><span data-stu-id="2e89f-253">Property</span></span>         | <span data-ttu-id="2e89f-254">类型</span><span class="sxs-lookup"><span data-stu-id="2e89f-254">Type</span></span>                                                     | <span data-ttu-id="2e89f-255">必需</span><span class="sxs-lookup"><span data-stu-id="2e89f-255">Required</span></span>                 | <span data-ttu-id="2e89f-256">值</span><span class="sxs-lookup"><span data-stu-id="2e89f-256">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="2e89f-257">resourceId</span><span class="sxs-lookup"><span data-stu-id="2e89f-257">resourceId</span></span>       | <span data-ttu-id="2e89f-258">String</span><span class="sxs-lookup"><span data-stu-id="2e89f-258">String</span></span>                                                   | <span data-ttu-id="2e89f-259">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-259">Yes</span></span>                      | <span data-ttu-id="2e89f-260">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="2e89f-260">\<resourceId\></span></span> |
| <span data-ttu-id="2e89f-261">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2e89f-261">roleDefinitionId</span></span> | <span data-ttu-id="2e89f-262">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-262">String</span></span>                                                   | <span data-ttu-id="2e89f-263">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-263">Yes</span></span>                      | <span data-ttu-id="2e89f-264">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="2e89f-264">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="2e89f-265">subjectId</span><span class="sxs-lookup"><span data-stu-id="2e89f-265">subjectId</span></span>        | <span data-ttu-id="2e89f-266">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-266">String</span></span>                                                   | <span data-ttu-id="2e89f-267">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-267">Yes</span></span>                      | <span data-ttu-id="2e89f-268">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="2e89f-268">\<subjectId\></span></span> |
| <span data-ttu-id="2e89f-269">assignmentState</span><span class="sxs-lookup"><span data-stu-id="2e89f-269">assignmentState</span></span>  | <span data-ttu-id="2e89f-270">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-270">String</span></span>                                                   | <span data-ttu-id="2e89f-271">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-271">Yes</span></span>                      | <span data-ttu-id="2e89f-272">活动</span><span class="sxs-lookup"><span data-stu-id="2e89f-272">Active</span></span> |
| <span data-ttu-id="2e89f-273">type</span><span class="sxs-lookup"><span data-stu-id="2e89f-273">type</span></span>             | <span data-ttu-id="2e89f-274">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-274">String</span></span>                                                   | <span data-ttu-id="2e89f-275">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-275">Yes</span></span>                      | <span data-ttu-id="2e89f-276">UserAdd</span><span class="sxs-lookup"><span data-stu-id="2e89f-276">UserAdd</span></span> |
| <span data-ttu-id="2e89f-277">在于</span><span class="sxs-lookup"><span data-stu-id="2e89f-277">reason</span></span>           | <span data-ttu-id="2e89f-278">String</span><span class="sxs-lookup"><span data-stu-id="2e89f-278">String</span></span>                                                   | <span data-ttu-id="2e89f-279">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="2e89f-279">depends on role Settings</span></span> |   |
| <span data-ttu-id="2e89f-280">schedule</span><span class="sxs-lookup"><span data-stu-id="2e89f-280">schedule</span></span>         | [<span data-ttu-id="2e89f-281">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2e89f-281">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="2e89f-282">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-282">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="2e89f-283">请求</span><span class="sxs-lookup"><span data-stu-id="2e89f-283">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="2e89f-284">响应</span><span class="sxs-lookup"><span data-stu-id="2e89f-284">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="2e89f-285">示例 3: 用户停用分配的角色</span><span class="sxs-lookup"><span data-stu-id="2e89f-285">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="2e89f-286">在此示例中, 用户 nawu@fimdev.net 停用活动的帐单阅读者角色。</span><span class="sxs-lookup"><span data-stu-id="2e89f-286">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="2e89f-287">属性</span><span class="sxs-lookup"><span data-stu-id="2e89f-287">Property</span></span>         | <span data-ttu-id="2e89f-288">类型</span><span class="sxs-lookup"><span data-stu-id="2e89f-288">Type</span></span>                                                     | <span data-ttu-id="2e89f-289">必需</span><span class="sxs-lookup"><span data-stu-id="2e89f-289">Required</span></span> | <span data-ttu-id="2e89f-290">值</span><span class="sxs-lookup"><span data-stu-id="2e89f-290">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="2e89f-291">resourceId</span><span class="sxs-lookup"><span data-stu-id="2e89f-291">resourceId</span></span>       | <span data-ttu-id="2e89f-292">String</span><span class="sxs-lookup"><span data-stu-id="2e89f-292">String</span></span>                                                   | <span data-ttu-id="2e89f-293">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-293">Yes</span></span>      | <span data-ttu-id="2e89f-294">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="2e89f-294">\<resourceId\></span></span> |
| <span data-ttu-id="2e89f-295">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2e89f-295">roleDefinitionId</span></span> | <span data-ttu-id="2e89f-296">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-296">String</span></span>                                                   | <span data-ttu-id="2e89f-297">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-297">Yes</span></span>      | <span data-ttu-id="2e89f-298">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="2e89f-298">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="2e89f-299">subjectId</span><span class="sxs-lookup"><span data-stu-id="2e89f-299">subjectId</span></span>        | <span data-ttu-id="2e89f-300">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-300">String</span></span>                                                   | <span data-ttu-id="2e89f-301">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-301">Yes</span></span>      | <span data-ttu-id="2e89f-302">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="2e89f-302">\<subjectId\></span></span> |
| <span data-ttu-id="2e89f-303">assignmentState</span><span class="sxs-lookup"><span data-stu-id="2e89f-303">assignmentState</span></span>  | <span data-ttu-id="2e89f-304">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-304">String</span></span>                                                   | <span data-ttu-id="2e89f-305">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-305">Yes</span></span>      | <span data-ttu-id="2e89f-306">活动</span><span class="sxs-lookup"><span data-stu-id="2e89f-306">Active</span></span> |
| <span data-ttu-id="2e89f-307">type</span><span class="sxs-lookup"><span data-stu-id="2e89f-307">type</span></span>             | <span data-ttu-id="2e89f-308">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-308">String</span></span>                                                   | <span data-ttu-id="2e89f-309">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-309">Yes</span></span>      | <span data-ttu-id="2e89f-310">UserRemove</span><span class="sxs-lookup"><span data-stu-id="2e89f-310">UserRemove</span></span> |
| <span data-ttu-id="2e89f-311">在于</span><span class="sxs-lookup"><span data-stu-id="2e89f-311">reason</span></span>           | <span data-ttu-id="2e89f-312">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-312">String</span></span>                                                   | <span data-ttu-id="2e89f-313">否</span><span class="sxs-lookup"><span data-stu-id="2e89f-313">No</span></span>       |   |
| <span data-ttu-id="2e89f-314">schedule</span><span class="sxs-lookup"><span data-stu-id="2e89f-314">schedule</span></span>         | [<span data-ttu-id="2e89f-315">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2e89f-315">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="2e89f-316">否</span><span class="sxs-lookup"><span data-stu-id="2e89f-316">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="2e89f-317">请求</span><span class="sxs-lookup"><span data-stu-id="2e89f-317">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="2e89f-318">响应</span><span class="sxs-lookup"><span data-stu-id="2e89f-318">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="2e89f-319">示例 4: 管理员从角色中删除用户</span><span class="sxs-lookup"><span data-stu-id="2e89f-319">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="2e89f-320">在此示例中, 管理员从 "计费读者" 角色中删除用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="2e89f-320">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="2e89f-321">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="2e89f-321">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="2e89f-322">属性</span><span class="sxs-lookup"><span data-stu-id="2e89f-322">Property</span></span>         | <span data-ttu-id="2e89f-323">类型</span><span class="sxs-lookup"><span data-stu-id="2e89f-323">Type</span></span>                                                     | <span data-ttu-id="2e89f-324">必需</span><span class="sxs-lookup"><span data-stu-id="2e89f-324">Required</span></span> | <span data-ttu-id="2e89f-325">值</span><span class="sxs-lookup"><span data-stu-id="2e89f-325">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="2e89f-326">resourceId</span><span class="sxs-lookup"><span data-stu-id="2e89f-326">resourceId</span></span>       | <span data-ttu-id="2e89f-327">String</span><span class="sxs-lookup"><span data-stu-id="2e89f-327">String</span></span>                                                   | <span data-ttu-id="2e89f-328">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-328">Yes</span></span>      | <span data-ttu-id="2e89f-329">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="2e89f-329">\<resourceId\></span></span> |
| <span data-ttu-id="2e89f-330">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2e89f-330">roleDefinitionId</span></span> | <span data-ttu-id="2e89f-331">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-331">String</span></span>                                                   | <span data-ttu-id="2e89f-332">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-332">Yes</span></span>      | <span data-ttu-id="2e89f-333">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="2e89f-333">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="2e89f-334">subjectId</span><span class="sxs-lookup"><span data-stu-id="2e89f-334">subjectId</span></span>        | <span data-ttu-id="2e89f-335">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-335">String</span></span>                                                   | <span data-ttu-id="2e89f-336">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-336">Yes</span></span>      | <span data-ttu-id="2e89f-337">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="2e89f-337">\<subjectId\></span></span> |
| <span data-ttu-id="2e89f-338">assignmentState</span><span class="sxs-lookup"><span data-stu-id="2e89f-338">assignmentState</span></span>  | <span data-ttu-id="2e89f-339">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-339">String</span></span>                                                   | <span data-ttu-id="2e89f-340">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-340">Yes</span></span>      | <span data-ttu-id="2e89f-341">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="2e89f-341">Eligible / Active</span></span> |
| <span data-ttu-id="2e89f-342">type</span><span class="sxs-lookup"><span data-stu-id="2e89f-342">type</span></span>             | <span data-ttu-id="2e89f-343">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-343">String</span></span>                                                   | <span data-ttu-id="2e89f-344">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-344">Yes</span></span>      | <span data-ttu-id="2e89f-345">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="2e89f-345">AdminRemove</span></span> |
| <span data-ttu-id="2e89f-346">在于</span><span class="sxs-lookup"><span data-stu-id="2e89f-346">reason</span></span>           | <span data-ttu-id="2e89f-347">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-347">String</span></span>                                                   | <span data-ttu-id="2e89f-348">否</span><span class="sxs-lookup"><span data-stu-id="2e89f-348">No</span></span>       |   |
| <span data-ttu-id="2e89f-349">schedule</span><span class="sxs-lookup"><span data-stu-id="2e89f-349">schedule</span></span>         | [<span data-ttu-id="2e89f-350">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2e89f-350">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="2e89f-351">否</span><span class="sxs-lookup"><span data-stu-id="2e89f-351">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="2e89f-352">请求</span><span class="sxs-lookup"><span data-stu-id="2e89f-352">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="2e89f-353">响应</span><span class="sxs-lookup"><span data-stu-id="2e89f-353">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="2e89f-354">示例 5: 管理员更新角色分配</span><span class="sxs-lookup"><span data-stu-id="2e89f-354">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="2e89f-355">在此示例中, 管理员将用户 nawu@fimdev.net 的角色分配更新为 "所有者"。</span><span class="sxs-lookup"><span data-stu-id="2e89f-355">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="2e89f-356">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="2e89f-356">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="2e89f-357">属性</span><span class="sxs-lookup"><span data-stu-id="2e89f-357">Property</span></span>         | <span data-ttu-id="2e89f-358">类型</span><span class="sxs-lookup"><span data-stu-id="2e89f-358">Type</span></span>                                                     | <span data-ttu-id="2e89f-359">必需</span><span class="sxs-lookup"><span data-stu-id="2e89f-359">Required</span></span>                | <span data-ttu-id="2e89f-360">值</span><span class="sxs-lookup"><span data-stu-id="2e89f-360">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="2e89f-361">resourceId</span><span class="sxs-lookup"><span data-stu-id="2e89f-361">resourceId</span></span>       | <span data-ttu-id="2e89f-362">String</span><span class="sxs-lookup"><span data-stu-id="2e89f-362">String</span></span>                                                   | <span data-ttu-id="2e89f-363">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-363">Yes</span></span>                     | <span data-ttu-id="2e89f-364">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="2e89f-364">\<resourceId\></span></span> |
| <span data-ttu-id="2e89f-365">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2e89f-365">roleDefinitionId</span></span> | <span data-ttu-id="2e89f-366">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-366">String</span></span>                                                   | <span data-ttu-id="2e89f-367">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-367">Yes</span></span>                     | <span data-ttu-id="2e89f-368">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="2e89f-368">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="2e89f-369">subjectId</span><span class="sxs-lookup"><span data-stu-id="2e89f-369">subjectId</span></span>        | <span data-ttu-id="2e89f-370">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-370">String</span></span>                                                   | <span data-ttu-id="2e89f-371">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-371">Yes</span></span>                     | <span data-ttu-id="2e89f-372">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="2e89f-372">\<subjectId\></span></span> |
| <span data-ttu-id="2e89f-373">assignmentState</span><span class="sxs-lookup"><span data-stu-id="2e89f-373">assignmentState</span></span>  | <span data-ttu-id="2e89f-374">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-374">String</span></span>                                                   | <span data-ttu-id="2e89f-375">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-375">Yes</span></span>                     | <span data-ttu-id="2e89f-376">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="2e89f-376">Eligible / Active</span></span> |
| <span data-ttu-id="2e89f-377">type</span><span class="sxs-lookup"><span data-stu-id="2e89f-377">type</span></span>             | <span data-ttu-id="2e89f-378">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-378">String</span></span>                                                   | <span data-ttu-id="2e89f-379">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-379">Yes</span></span>                     | <span data-ttu-id="2e89f-380">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="2e89f-380">AdminUpdate</span></span> |
| <span data-ttu-id="2e89f-381">在于</span><span class="sxs-lookup"><span data-stu-id="2e89f-381">reason</span></span>           | <span data-ttu-id="2e89f-382">String</span><span class="sxs-lookup"><span data-stu-id="2e89f-382">String</span></span>                                                   | <span data-ttu-id="2e89f-383">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="2e89f-383">depends on roleSettings</span></span> |   |
| <span data-ttu-id="2e89f-384">schedule</span><span class="sxs-lookup"><span data-stu-id="2e89f-384">schedule</span></span>         | [<span data-ttu-id="2e89f-385">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2e89f-385">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="2e89f-386">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-386">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="2e89f-387">请求</span><span class="sxs-lookup"><span data-stu-id="2e89f-387">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="2e89f-388">响应</span><span class="sxs-lookup"><span data-stu-id="2e89f-388">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="2e89f-389">示例 6: 管理员扩展了即将过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="2e89f-389">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="2e89f-390">此示例将用户 ANUJCUSER 的过期角色分配扩展到 API Management Service 参与者。</span><span class="sxs-lookup"><span data-stu-id="2e89f-390">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="2e89f-391">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="2e89f-391">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="2e89f-392">属性</span><span class="sxs-lookup"><span data-stu-id="2e89f-392">Property</span></span>         | <span data-ttu-id="2e89f-393">类型</span><span class="sxs-lookup"><span data-stu-id="2e89f-393">Type</span></span>                                                     | <span data-ttu-id="2e89f-394">必需</span><span class="sxs-lookup"><span data-stu-id="2e89f-394">Required</span></span>                | <span data-ttu-id="2e89f-395">值</span><span class="sxs-lookup"><span data-stu-id="2e89f-395">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="2e89f-396">resourceId</span><span class="sxs-lookup"><span data-stu-id="2e89f-396">resourceId</span></span>       | <span data-ttu-id="2e89f-397">String</span><span class="sxs-lookup"><span data-stu-id="2e89f-397">String</span></span>                                                   | <span data-ttu-id="2e89f-398">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-398">Yes</span></span>                     | <span data-ttu-id="2e89f-399">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="2e89f-399">\<resourceId\></span></span> |
| <span data-ttu-id="2e89f-400">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2e89f-400">roleDefinitionId</span></span> | <span data-ttu-id="2e89f-401">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-401">String</span></span>                                                   | <span data-ttu-id="2e89f-402">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-402">Yes</span></span>                     | <span data-ttu-id="2e89f-403">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="2e89f-403">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="2e89f-404">subjectId</span><span class="sxs-lookup"><span data-stu-id="2e89f-404">subjectId</span></span>        | <span data-ttu-id="2e89f-405">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-405">String</span></span>                                                   | <span data-ttu-id="2e89f-406">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-406">Yes</span></span>                     | <span data-ttu-id="2e89f-407">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="2e89f-407">\<subjectId\></span></span> |
| <span data-ttu-id="2e89f-408">assignmentState</span><span class="sxs-lookup"><span data-stu-id="2e89f-408">assignmentState</span></span>  | <span data-ttu-id="2e89f-409">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-409">String</span></span>                                                   | <span data-ttu-id="2e89f-410">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-410">Yes</span></span>                     | <span data-ttu-id="2e89f-411">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="2e89f-411">Eligible / Active</span></span> |
| <span data-ttu-id="2e89f-412">type</span><span class="sxs-lookup"><span data-stu-id="2e89f-412">type</span></span>             | <span data-ttu-id="2e89f-413">字符串</span><span class="sxs-lookup"><span data-stu-id="2e89f-413">String</span></span>                                                   | <span data-ttu-id="2e89f-414">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-414">Yes</span></span>                     | <span data-ttu-id="2e89f-415">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="2e89f-415">AdminExtend</span></span> |
| <span data-ttu-id="2e89f-416">在于</span><span class="sxs-lookup"><span data-stu-id="2e89f-416">reason</span></span>           | <span data-ttu-id="2e89f-417">String</span><span class="sxs-lookup"><span data-stu-id="2e89f-417">String</span></span>                                                   | <span data-ttu-id="2e89f-418">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="2e89f-418">depends on roleSettings</span></span> |   |
| <span data-ttu-id="2e89f-419">schedule</span><span class="sxs-lookup"><span data-stu-id="2e89f-419">schedule</span></span>         | [<span data-ttu-id="2e89f-420">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2e89f-420">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="2e89f-421">是</span><span class="sxs-lookup"><span data-stu-id="2e89f-421">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="2e89f-422">请求</span><span class="sxs-lookup"><span data-stu-id="2e89f-422">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="2e89f-423">响应</span><span class="sxs-lookup"><span data-stu-id="2e89f-423">Response</span></span>

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
