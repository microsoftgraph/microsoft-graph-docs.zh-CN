---
title: 创建 governanceRoleAssignmentRequest
description: 创建一个角色分配请求, 以代表在角色分配上所需的操作。 下表列出了这些操作。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: a49bd528ffe97e33402ab8aef51f86a07b33e5fa
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420313"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="7580b-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="7580b-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7580b-105">创建一个角色分配请求, 以代表在角色分配上所需的操作。</span><span class="sxs-lookup"><span data-stu-id="7580b-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="7580b-106">下表列出了这些操作。</span><span class="sxs-lookup"><span data-stu-id="7580b-106">The following table lists the operations.</span></span>

| <span data-ttu-id="7580b-107">Operation</span><span class="sxs-lookup"><span data-stu-id="7580b-107">Operation</span></span>                                   | <span data-ttu-id="7580b-108">类型</span><span class="sxs-lookup"><span data-stu-id="7580b-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="7580b-109">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="7580b-109">Assign a role assignment</span></span>                    | <span data-ttu-id="7580b-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="7580b-110">AdminAdd</span></span>    |
| <span data-ttu-id="7580b-111">激活符合条件的角色分配</span><span class="sxs-lookup"><span data-stu-id="7580b-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="7580b-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="7580b-112">UserAdd</span></span>     |
| <span data-ttu-id="7580b-113">停用已激活的角色分配</span><span class="sxs-lookup"><span data-stu-id="7580b-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="7580b-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="7580b-114">UserRemove</span></span>  |
| <span data-ttu-id="7580b-115">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="7580b-115">Remove a role assignment</span></span>                    | <span data-ttu-id="7580b-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="7580b-116">AdminRemove</span></span> |
| <span data-ttu-id="7580b-117">更新角色分配</span><span class="sxs-lookup"><span data-stu-id="7580b-117">Update a role assignment</span></span>                    | <span data-ttu-id="7580b-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="7580b-118">AdminUpdate</span></span> |
| <span data-ttu-id="7580b-119">请求扩展我的角色分配</span><span class="sxs-lookup"><span data-stu-id="7580b-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="7580b-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="7580b-120">UserExtend</span></span>  |
| <span data-ttu-id="7580b-121">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="7580b-121">Extend a role assignment</span></span>                    | <span data-ttu-id="7580b-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="7580b-122">AdminExtend</span></span> |
| <span data-ttu-id="7580b-123">续订我的过期角色分配的请求</span><span class="sxs-lookup"><span data-stu-id="7580b-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="7580b-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="7580b-124">UserRenew</span></span>   |
| <span data-ttu-id="7580b-125">续订过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="7580b-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="7580b-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="7580b-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="7580b-127">权限</span><span class="sxs-lookup"><span data-stu-id="7580b-127">Permissions</span></span>

<span data-ttu-id="7580b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7580b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7580b-130">权限类型</span><span class="sxs-lookup"><span data-stu-id="7580b-130">Permission type</span></span>                        | <span data-ttu-id="7580b-131">权限</span><span class="sxs-lookup"><span data-stu-id="7580b-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="7580b-132">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7580b-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="7580b-133">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="7580b-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="7580b-134">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7580b-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7580b-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="7580b-135">Not supported.</span></span>                            |
| <span data-ttu-id="7580b-136">应用程序</span><span class="sxs-lookup"><span data-stu-id="7580b-136">Application</span></span>                            | <span data-ttu-id="7580b-137">不支持。</span><span class="sxs-lookup"><span data-stu-id="7580b-137">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7580b-138">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7580b-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="7580b-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="7580b-139">Request headers</span></span>

| <span data-ttu-id="7580b-140">名称</span><span class="sxs-lookup"><span data-stu-id="7580b-140">Name</span></span>          | <span data-ttu-id="7580b-141">说明</span><span class="sxs-lookup"><span data-stu-id="7580b-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="7580b-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="7580b-142">Authorization</span></span> | <span data-ttu-id="7580b-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7580b-143">Bearer {code}</span></span>    |
| <span data-ttu-id="7580b-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="7580b-144">Content-type</span></span>  | <span data-ttu-id="7580b-145">application/json</span><span class="sxs-lookup"><span data-stu-id="7580b-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7580b-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="7580b-146">Request body</span></span>

<span data-ttu-id="7580b-147">在请求正文中, 提供[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7580b-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="7580b-148">属性</span><span class="sxs-lookup"><span data-stu-id="7580b-148">Property</span></span>         | <span data-ttu-id="7580b-149">类型</span><span class="sxs-lookup"><span data-stu-id="7580b-149">Type</span></span>                                                     | <span data-ttu-id="7580b-150">说明</span><span class="sxs-lookup"><span data-stu-id="7580b-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="7580b-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="7580b-151">resourceId</span></span>       | <span data-ttu-id="7580b-152">String</span><span class="sxs-lookup"><span data-stu-id="7580b-152">String</span></span>                                                   | <span data-ttu-id="7580b-153">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="7580b-153">The ID of the resource.</span></span> <span data-ttu-id="7580b-154">必需。</span><span class="sxs-lookup"><span data-stu-id="7580b-154">Required.</span></span> |
| <span data-ttu-id="7580b-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7580b-155">roleDefinitionId</span></span> | <span data-ttu-id="7580b-156">String</span><span class="sxs-lookup"><span data-stu-id="7580b-156">String</span></span>                                                   | <span data-ttu-id="7580b-157">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="7580b-157">The ID of the role definition.</span></span> <span data-ttu-id="7580b-158">必需。</span><span class="sxs-lookup"><span data-stu-id="7580b-158">Required.</span></span> |
| <span data-ttu-id="7580b-159">subjectId</span><span class="sxs-lookup"><span data-stu-id="7580b-159">subjectId</span></span>        | <span data-ttu-id="7580b-160">String</span><span class="sxs-lookup"><span data-stu-id="7580b-160">String</span></span>                                                   | <span data-ttu-id="7580b-161">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="7580b-161">The ID of the subject.</span></span> <span data-ttu-id="7580b-162">必需。</span><span class="sxs-lookup"><span data-stu-id="7580b-162">Required.</span></span> |
| <span data-ttu-id="7580b-163">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7580b-163">assignmentState</span></span>  | <span data-ttu-id="7580b-164">String</span><span class="sxs-lookup"><span data-stu-id="7580b-164">String</span></span>                                                   | <span data-ttu-id="7580b-165">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="7580b-165">The state of assignment.</span></span> <span data-ttu-id="7580b-166">值可以是`Eligible`和`Active`。</span><span class="sxs-lookup"><span data-stu-id="7580b-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="7580b-167">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="7580b-167">Required.</span></span> |
| <span data-ttu-id="7580b-168">type</span><span class="sxs-lookup"><span data-stu-id="7580b-168">type</span></span>             | <span data-ttu-id="7580b-169">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-169">String</span></span>                                                   | <span data-ttu-id="7580b-170">请求类型。</span><span class="sxs-lookup"><span data-stu-id="7580b-170">The request type.</span></span> <span data-ttu-id="7580b-171">值可以是`AdminAdd` `UserAdd`、、 `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `AdminRenew` `AdminExtend`、、、、和。 `UserRenew`</span><span class="sxs-lookup"><span data-stu-id="7580b-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="7580b-172">必需。</span><span class="sxs-lookup"><span data-stu-id="7580b-172">Required.</span></span> |
| <span data-ttu-id="7580b-173">在于</span><span class="sxs-lookup"><span data-stu-id="7580b-173">reason</span></span>           | <span data-ttu-id="7580b-174">String</span><span class="sxs-lookup"><span data-stu-id="7580b-174">String</span></span>                                                   | <span data-ttu-id="7580b-175">需要为角色分配请求提供审核和审阅目的的原因。</span><span class="sxs-lookup"><span data-stu-id="7580b-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="7580b-176">schedule</span><span class="sxs-lookup"><span data-stu-id="7580b-176">schedule</span></span>         | [<span data-ttu-id="7580b-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7580b-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7580b-178">角色分配请求的日程安排。</span><span class="sxs-lookup"><span data-stu-id="7580b-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="7580b-179">对于的请求类型`UserAdd`, `AdminAdd` `AdminUpdate`、和`AdminExtend`, 它是必需的。</span><span class="sxs-lookup"><span data-stu-id="7580b-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="7580b-180">响应</span><span class="sxs-lookup"><span data-stu-id="7580b-180">Response</span></span>

<span data-ttu-id="7580b-181">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7580b-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="7580b-182">错误代码</span><span class="sxs-lookup"><span data-stu-id="7580b-182">Error codes</span></span>

<span data-ttu-id="7580b-183">此 API 返回标准的 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="7580b-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="7580b-184">此外, 它还返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="7580b-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="7580b-185">错误代码</span><span class="sxs-lookup"><span data-stu-id="7580b-185">Error code</span></span>     | <span data-ttu-id="7580b-186">错误消息</span><span class="sxs-lookup"><span data-stu-id="7580b-186">Error message</span></span>                               | <span data-ttu-id="7580b-187">详细信息</span><span class="sxs-lookup"><span data-stu-id="7580b-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="7580b-188">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7580b-188">400 BadRequest</span></span> | <span data-ttu-id="7580b-189">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="7580b-189">RoleNotFound</span></span>                                | <span data-ttu-id="7580b-190">找`roleDefinitionId`不到请求正文中提供的。</span><span class="sxs-lookup"><span data-stu-id="7580b-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="7580b-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7580b-191">400 BadRequest</span></span> | <span data-ttu-id="7580b-192">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="7580b-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="7580b-193">请求正文中提供的资源处于状态`Locked` , 并且无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="7580b-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="7580b-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7580b-194">400 BadRequest</span></span> | <span data-ttu-id="7580b-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="7580b-195">SubjectNotFound</span></span>                             | <span data-ttu-id="7580b-196">找`subjectId`不到请求正文中提供的。</span><span class="sxs-lookup"><span data-stu-id="7580b-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="7580b-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7580b-197">400 BadRequest</span></span> | <span data-ttu-id="7580b-198">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="7580b-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="7580b-199">系统中已存在一个挂起的[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 。</span><span class="sxs-lookup"><span data-stu-id="7580b-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="7580b-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7580b-200">400 BadRequest</span></span> | <span data-ttu-id="7580b-201">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="7580b-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="7580b-202">系统中已存在请求创建的[governanceRoleAssignment](../resources/governanceroleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="7580b-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="7580b-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7580b-203">400 BadRequest</span></span> | <span data-ttu-id="7580b-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="7580b-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="7580b-205">系统中不存在请求进行更新/扩展的[governanceRoleAssignment](../resources/governanceroleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="7580b-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="7580b-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7580b-206">400 BadRequest</span></span> | <span data-ttu-id="7580b-207">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="7580b-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="7580b-208">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部策略, 因此无法创建。</span><span class="sxs-lookup"><span data-stu-id="7580b-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="7580b-209">示例</span><span class="sxs-lookup"><span data-stu-id="7580b-209">Examples</span></span>

<span data-ttu-id="7580b-210">下面的示例演示如何使用此 API。</span><span class="sxs-lookup"><span data-stu-id="7580b-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="7580b-211">示例 1: 管理员为用户分配角色</span><span class="sxs-lookup"><span data-stu-id="7580b-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="7580b-212">在此示例中, 管理员向计费读者角色分配用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="7580b-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="7580b-213">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="7580b-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="7580b-214">属性</span><span class="sxs-lookup"><span data-stu-id="7580b-214">Property</span></span>         | <span data-ttu-id="7580b-215">类型</span><span class="sxs-lookup"><span data-stu-id="7580b-215">Type</span></span>                                                     | <span data-ttu-id="7580b-216">必需</span><span class="sxs-lookup"><span data-stu-id="7580b-216">Required</span></span>                 | <span data-ttu-id="7580b-217">值</span><span class="sxs-lookup"><span data-stu-id="7580b-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="7580b-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="7580b-218">resourceId</span></span>       | <span data-ttu-id="7580b-219">String</span><span class="sxs-lookup"><span data-stu-id="7580b-219">String</span></span>                                                   | <span data-ttu-id="7580b-220">是</span><span class="sxs-lookup"><span data-stu-id="7580b-220">Yes</span></span>                      | <span data-ttu-id="7580b-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="7580b-221">\<resourceId\></span></span> |
| <span data-ttu-id="7580b-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7580b-222">roleDefinitionId</span></span> | <span data-ttu-id="7580b-223">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-223">String</span></span>                                                   | <span data-ttu-id="7580b-224">是</span><span class="sxs-lookup"><span data-stu-id="7580b-224">Yes</span></span>                      | <span data-ttu-id="7580b-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="7580b-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="7580b-226">subjectId</span><span class="sxs-lookup"><span data-stu-id="7580b-226">subjectId</span></span>        | <span data-ttu-id="7580b-227">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-227">String</span></span>                                                   | <span data-ttu-id="7580b-228">是</span><span class="sxs-lookup"><span data-stu-id="7580b-228">Yes</span></span>                      | <span data-ttu-id="7580b-229">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="7580b-229">\<subjectId\></span></span> |
| <span data-ttu-id="7580b-230">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7580b-230">assignmentState</span></span>  | <span data-ttu-id="7580b-231">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-231">String</span></span>                                                   | <span data-ttu-id="7580b-232">是</span><span class="sxs-lookup"><span data-stu-id="7580b-232">Yes</span></span>                      | <span data-ttu-id="7580b-233">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="7580b-233">Eligible / Active</span></span> |
| <span data-ttu-id="7580b-234">type</span><span class="sxs-lookup"><span data-stu-id="7580b-234">type</span></span>             | <span data-ttu-id="7580b-235">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-235">String</span></span>                                                   | <span data-ttu-id="7580b-236">是</span><span class="sxs-lookup"><span data-stu-id="7580b-236">Yes</span></span>                      | <span data-ttu-id="7580b-237">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="7580b-237">AdminAdd</span></span> |
| <span data-ttu-id="7580b-238">在于</span><span class="sxs-lookup"><span data-stu-id="7580b-238">reason</span></span>           | <span data-ttu-id="7580b-239">String</span><span class="sxs-lookup"><span data-stu-id="7580b-239">String</span></span>                                                   | <span data-ttu-id="7580b-240">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="7580b-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="7580b-241">schedule</span><span class="sxs-lookup"><span data-stu-id="7580b-241">schedule</span></span>         | [<span data-ttu-id="7580b-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7580b-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7580b-243">是</span><span class="sxs-lookup"><span data-stu-id="7580b-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="7580b-244">请求</span><span class="sxs-lookup"><span data-stu-id="7580b-244">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7580b-245">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="7580b-245">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7580b-246">C#</span><span class="sxs-lookup"><span data-stu-id="7580b-246">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7580b-247">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7580b-247">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7580b-248">目标-C</span><span class="sxs-lookup"><span data-stu-id="7580b-248">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="7580b-249">响应</span><span class="sxs-lookup"><span data-stu-id="7580b-249">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="7580b-250">示例 2: 用户激活符合条件的角色</span><span class="sxs-lookup"><span data-stu-id="7580b-250">Example 2: User activates eligible role</span></span>

<span data-ttu-id="7580b-251">在此示例中, 用户 nawu@fimdev.net 激活符合条件的计费阅读者角色。</span><span class="sxs-lookup"><span data-stu-id="7580b-251">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="7580b-252">属性</span><span class="sxs-lookup"><span data-stu-id="7580b-252">Property</span></span>         | <span data-ttu-id="7580b-253">类型</span><span class="sxs-lookup"><span data-stu-id="7580b-253">Type</span></span>                                                     | <span data-ttu-id="7580b-254">必需</span><span class="sxs-lookup"><span data-stu-id="7580b-254">Required</span></span>                 | <span data-ttu-id="7580b-255">值</span><span class="sxs-lookup"><span data-stu-id="7580b-255">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="7580b-256">resourceId</span><span class="sxs-lookup"><span data-stu-id="7580b-256">resourceId</span></span>       | <span data-ttu-id="7580b-257">String</span><span class="sxs-lookup"><span data-stu-id="7580b-257">String</span></span>                                                   | <span data-ttu-id="7580b-258">是</span><span class="sxs-lookup"><span data-stu-id="7580b-258">Yes</span></span>                      | <span data-ttu-id="7580b-259">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="7580b-259">\<resourceId\></span></span> |
| <span data-ttu-id="7580b-260">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7580b-260">roleDefinitionId</span></span> | <span data-ttu-id="7580b-261">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-261">String</span></span>                                                   | <span data-ttu-id="7580b-262">是</span><span class="sxs-lookup"><span data-stu-id="7580b-262">Yes</span></span>                      | <span data-ttu-id="7580b-263">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="7580b-263">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="7580b-264">subjectId</span><span class="sxs-lookup"><span data-stu-id="7580b-264">subjectId</span></span>        | <span data-ttu-id="7580b-265">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-265">String</span></span>                                                   | <span data-ttu-id="7580b-266">是</span><span class="sxs-lookup"><span data-stu-id="7580b-266">Yes</span></span>                      | <span data-ttu-id="7580b-267">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="7580b-267">\<subjectId\></span></span> |
| <span data-ttu-id="7580b-268">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7580b-268">assignmentState</span></span>  | <span data-ttu-id="7580b-269">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-269">String</span></span>                                                   | <span data-ttu-id="7580b-270">是</span><span class="sxs-lookup"><span data-stu-id="7580b-270">Yes</span></span>                      | <span data-ttu-id="7580b-271">活动</span><span class="sxs-lookup"><span data-stu-id="7580b-271">Active</span></span> |
| <span data-ttu-id="7580b-272">type</span><span class="sxs-lookup"><span data-stu-id="7580b-272">type</span></span>             | <span data-ttu-id="7580b-273">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-273">String</span></span>                                                   | <span data-ttu-id="7580b-274">是</span><span class="sxs-lookup"><span data-stu-id="7580b-274">Yes</span></span>                      | <span data-ttu-id="7580b-275">UserAdd</span><span class="sxs-lookup"><span data-stu-id="7580b-275">UserAdd</span></span> |
| <span data-ttu-id="7580b-276">在于</span><span class="sxs-lookup"><span data-stu-id="7580b-276">reason</span></span>           | <span data-ttu-id="7580b-277">String</span><span class="sxs-lookup"><span data-stu-id="7580b-277">String</span></span>                                                   | <span data-ttu-id="7580b-278">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="7580b-278">depends on role Settings</span></span> |   |
| <span data-ttu-id="7580b-279">schedule</span><span class="sxs-lookup"><span data-stu-id="7580b-279">schedule</span></span>         | [<span data-ttu-id="7580b-280">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7580b-280">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7580b-281">是</span><span class="sxs-lookup"><span data-stu-id="7580b-281">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="7580b-282">请求</span><span class="sxs-lookup"><span data-stu-id="7580b-282">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="7580b-283">响应</span><span class="sxs-lookup"><span data-stu-id="7580b-283">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="7580b-284">示例 3: 用户停用分配的角色</span><span class="sxs-lookup"><span data-stu-id="7580b-284">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="7580b-285">在此示例中, 用户 nawu@fimdev.net 停用活动的帐单阅读者角色。</span><span class="sxs-lookup"><span data-stu-id="7580b-285">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="7580b-286">属性</span><span class="sxs-lookup"><span data-stu-id="7580b-286">Property</span></span>         | <span data-ttu-id="7580b-287">类型</span><span class="sxs-lookup"><span data-stu-id="7580b-287">Type</span></span>                                                     | <span data-ttu-id="7580b-288">必需</span><span class="sxs-lookup"><span data-stu-id="7580b-288">Required</span></span> | <span data-ttu-id="7580b-289">值</span><span class="sxs-lookup"><span data-stu-id="7580b-289">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="7580b-290">resourceId</span><span class="sxs-lookup"><span data-stu-id="7580b-290">resourceId</span></span>       | <span data-ttu-id="7580b-291">String</span><span class="sxs-lookup"><span data-stu-id="7580b-291">String</span></span>                                                   | <span data-ttu-id="7580b-292">是</span><span class="sxs-lookup"><span data-stu-id="7580b-292">Yes</span></span>      | <span data-ttu-id="7580b-293">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="7580b-293">\<resourceId\></span></span> |
| <span data-ttu-id="7580b-294">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7580b-294">roleDefinitionId</span></span> | <span data-ttu-id="7580b-295">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-295">String</span></span>                                                   | <span data-ttu-id="7580b-296">是</span><span class="sxs-lookup"><span data-stu-id="7580b-296">Yes</span></span>      | <span data-ttu-id="7580b-297">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="7580b-297">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="7580b-298">subjectId</span><span class="sxs-lookup"><span data-stu-id="7580b-298">subjectId</span></span>        | <span data-ttu-id="7580b-299">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-299">String</span></span>                                                   | <span data-ttu-id="7580b-300">是</span><span class="sxs-lookup"><span data-stu-id="7580b-300">Yes</span></span>      | <span data-ttu-id="7580b-301">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="7580b-301">\<subjectId\></span></span> |
| <span data-ttu-id="7580b-302">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7580b-302">assignmentState</span></span>  | <span data-ttu-id="7580b-303">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-303">String</span></span>                                                   | <span data-ttu-id="7580b-304">是</span><span class="sxs-lookup"><span data-stu-id="7580b-304">Yes</span></span>      | <span data-ttu-id="7580b-305">活动</span><span class="sxs-lookup"><span data-stu-id="7580b-305">Active</span></span> |
| <span data-ttu-id="7580b-306">type</span><span class="sxs-lookup"><span data-stu-id="7580b-306">type</span></span>             | <span data-ttu-id="7580b-307">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-307">String</span></span>                                                   | <span data-ttu-id="7580b-308">是</span><span class="sxs-lookup"><span data-stu-id="7580b-308">Yes</span></span>      | <span data-ttu-id="7580b-309">UserRemove</span><span class="sxs-lookup"><span data-stu-id="7580b-309">UserRemove</span></span> |
| <span data-ttu-id="7580b-310">在于</span><span class="sxs-lookup"><span data-stu-id="7580b-310">reason</span></span>           | <span data-ttu-id="7580b-311">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-311">String</span></span>                                                   | <span data-ttu-id="7580b-312">否</span><span class="sxs-lookup"><span data-stu-id="7580b-312">No</span></span>       |   |
| <span data-ttu-id="7580b-313">schedule</span><span class="sxs-lookup"><span data-stu-id="7580b-313">schedule</span></span>         | [<span data-ttu-id="7580b-314">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7580b-314">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7580b-315">否</span><span class="sxs-lookup"><span data-stu-id="7580b-315">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="7580b-316">请求</span><span class="sxs-lookup"><span data-stu-id="7580b-316">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="7580b-317">响应</span><span class="sxs-lookup"><span data-stu-id="7580b-317">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="7580b-318">示例 4: 管理员从角色中删除用户</span><span class="sxs-lookup"><span data-stu-id="7580b-318">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="7580b-319">在此示例中, 管理员从 "计费读者" 角色中删除用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="7580b-319">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="7580b-320">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="7580b-320">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="7580b-321">属性</span><span class="sxs-lookup"><span data-stu-id="7580b-321">Property</span></span>         | <span data-ttu-id="7580b-322">类型</span><span class="sxs-lookup"><span data-stu-id="7580b-322">Type</span></span>                                                     | <span data-ttu-id="7580b-323">必需</span><span class="sxs-lookup"><span data-stu-id="7580b-323">Required</span></span> | <span data-ttu-id="7580b-324">值</span><span class="sxs-lookup"><span data-stu-id="7580b-324">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="7580b-325">resourceId</span><span class="sxs-lookup"><span data-stu-id="7580b-325">resourceId</span></span>       | <span data-ttu-id="7580b-326">String</span><span class="sxs-lookup"><span data-stu-id="7580b-326">String</span></span>                                                   | <span data-ttu-id="7580b-327">是</span><span class="sxs-lookup"><span data-stu-id="7580b-327">Yes</span></span>      | <span data-ttu-id="7580b-328">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="7580b-328">\<resourceId\></span></span> |
| <span data-ttu-id="7580b-329">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7580b-329">roleDefinitionId</span></span> | <span data-ttu-id="7580b-330">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-330">String</span></span>                                                   | <span data-ttu-id="7580b-331">是</span><span class="sxs-lookup"><span data-stu-id="7580b-331">Yes</span></span>      | <span data-ttu-id="7580b-332">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="7580b-332">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="7580b-333">subjectId</span><span class="sxs-lookup"><span data-stu-id="7580b-333">subjectId</span></span>        | <span data-ttu-id="7580b-334">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-334">String</span></span>                                                   | <span data-ttu-id="7580b-335">是</span><span class="sxs-lookup"><span data-stu-id="7580b-335">Yes</span></span>      | <span data-ttu-id="7580b-336">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="7580b-336">\<subjectId\></span></span> |
| <span data-ttu-id="7580b-337">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7580b-337">assignmentState</span></span>  | <span data-ttu-id="7580b-338">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-338">String</span></span>                                                   | <span data-ttu-id="7580b-339">是</span><span class="sxs-lookup"><span data-stu-id="7580b-339">Yes</span></span>      | <span data-ttu-id="7580b-340">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="7580b-340">Eligible / Active</span></span> |
| <span data-ttu-id="7580b-341">type</span><span class="sxs-lookup"><span data-stu-id="7580b-341">type</span></span>             | <span data-ttu-id="7580b-342">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-342">String</span></span>                                                   | <span data-ttu-id="7580b-343">是</span><span class="sxs-lookup"><span data-stu-id="7580b-343">Yes</span></span>      | <span data-ttu-id="7580b-344">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="7580b-344">AdminRemove</span></span> |
| <span data-ttu-id="7580b-345">在于</span><span class="sxs-lookup"><span data-stu-id="7580b-345">reason</span></span>           | <span data-ttu-id="7580b-346">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-346">String</span></span>                                                   | <span data-ttu-id="7580b-347">否</span><span class="sxs-lookup"><span data-stu-id="7580b-347">No</span></span>       |   |
| <span data-ttu-id="7580b-348">schedule</span><span class="sxs-lookup"><span data-stu-id="7580b-348">schedule</span></span>         | [<span data-ttu-id="7580b-349">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7580b-349">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7580b-350">否</span><span class="sxs-lookup"><span data-stu-id="7580b-350">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="7580b-351">请求</span><span class="sxs-lookup"><span data-stu-id="7580b-351">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="7580b-352">响应</span><span class="sxs-lookup"><span data-stu-id="7580b-352">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="7580b-353">示例 5: 管理员更新角色分配</span><span class="sxs-lookup"><span data-stu-id="7580b-353">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="7580b-354">在此示例中, 管理员将用户 nawu@fimdev.net 的角色分配更新为 "所有者"。</span><span class="sxs-lookup"><span data-stu-id="7580b-354">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="7580b-355">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="7580b-355">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="7580b-356">属性</span><span class="sxs-lookup"><span data-stu-id="7580b-356">Property</span></span>         | <span data-ttu-id="7580b-357">类型</span><span class="sxs-lookup"><span data-stu-id="7580b-357">Type</span></span>                                                     | <span data-ttu-id="7580b-358">必需</span><span class="sxs-lookup"><span data-stu-id="7580b-358">Required</span></span>                | <span data-ttu-id="7580b-359">值</span><span class="sxs-lookup"><span data-stu-id="7580b-359">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="7580b-360">resourceId</span><span class="sxs-lookup"><span data-stu-id="7580b-360">resourceId</span></span>       | <span data-ttu-id="7580b-361">String</span><span class="sxs-lookup"><span data-stu-id="7580b-361">String</span></span>                                                   | <span data-ttu-id="7580b-362">是</span><span class="sxs-lookup"><span data-stu-id="7580b-362">Yes</span></span>                     | <span data-ttu-id="7580b-363">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="7580b-363">\<resourceId\></span></span> |
| <span data-ttu-id="7580b-364">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7580b-364">roleDefinitionId</span></span> | <span data-ttu-id="7580b-365">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-365">String</span></span>                                                   | <span data-ttu-id="7580b-366">是</span><span class="sxs-lookup"><span data-stu-id="7580b-366">Yes</span></span>                     | <span data-ttu-id="7580b-367">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="7580b-367">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="7580b-368">subjectId</span><span class="sxs-lookup"><span data-stu-id="7580b-368">subjectId</span></span>        | <span data-ttu-id="7580b-369">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-369">String</span></span>                                                   | <span data-ttu-id="7580b-370">是</span><span class="sxs-lookup"><span data-stu-id="7580b-370">Yes</span></span>                     | <span data-ttu-id="7580b-371">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="7580b-371">\<subjectId\></span></span> |
| <span data-ttu-id="7580b-372">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7580b-372">assignmentState</span></span>  | <span data-ttu-id="7580b-373">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-373">String</span></span>                                                   | <span data-ttu-id="7580b-374">是</span><span class="sxs-lookup"><span data-stu-id="7580b-374">Yes</span></span>                     | <span data-ttu-id="7580b-375">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="7580b-375">Eligible / Active</span></span> |
| <span data-ttu-id="7580b-376">type</span><span class="sxs-lookup"><span data-stu-id="7580b-376">type</span></span>             | <span data-ttu-id="7580b-377">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-377">String</span></span>                                                   | <span data-ttu-id="7580b-378">是</span><span class="sxs-lookup"><span data-stu-id="7580b-378">Yes</span></span>                     | <span data-ttu-id="7580b-379">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="7580b-379">AdminUpdate</span></span> |
| <span data-ttu-id="7580b-380">在于</span><span class="sxs-lookup"><span data-stu-id="7580b-380">reason</span></span>           | <span data-ttu-id="7580b-381">String</span><span class="sxs-lookup"><span data-stu-id="7580b-381">String</span></span>                                                   | <span data-ttu-id="7580b-382">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="7580b-382">depends on roleSettings</span></span> |   |
| <span data-ttu-id="7580b-383">schedule</span><span class="sxs-lookup"><span data-stu-id="7580b-383">schedule</span></span>         | [<span data-ttu-id="7580b-384">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7580b-384">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7580b-385">是</span><span class="sxs-lookup"><span data-stu-id="7580b-385">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="7580b-386">请求</span><span class="sxs-lookup"><span data-stu-id="7580b-386">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="7580b-387">响应</span><span class="sxs-lookup"><span data-stu-id="7580b-387">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="7580b-388">示例 6: 管理员扩展了即将过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="7580b-388">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="7580b-389">此示例将用户 ANUJCUSER 的过期角色分配扩展到 API Management Service 参与者。</span><span class="sxs-lookup"><span data-stu-id="7580b-389">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="7580b-390">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="7580b-390">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="7580b-391">属性</span><span class="sxs-lookup"><span data-stu-id="7580b-391">Property</span></span>         | <span data-ttu-id="7580b-392">类型</span><span class="sxs-lookup"><span data-stu-id="7580b-392">Type</span></span>                                                     | <span data-ttu-id="7580b-393">必需</span><span class="sxs-lookup"><span data-stu-id="7580b-393">Required</span></span>                | <span data-ttu-id="7580b-394">值</span><span class="sxs-lookup"><span data-stu-id="7580b-394">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="7580b-395">resourceId</span><span class="sxs-lookup"><span data-stu-id="7580b-395">resourceId</span></span>       | <span data-ttu-id="7580b-396">String</span><span class="sxs-lookup"><span data-stu-id="7580b-396">String</span></span>                                                   | <span data-ttu-id="7580b-397">是</span><span class="sxs-lookup"><span data-stu-id="7580b-397">Yes</span></span>                     | <span data-ttu-id="7580b-398">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="7580b-398">\<resourceId\></span></span> |
| <span data-ttu-id="7580b-399">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7580b-399">roleDefinitionId</span></span> | <span data-ttu-id="7580b-400">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-400">String</span></span>                                                   | <span data-ttu-id="7580b-401">是</span><span class="sxs-lookup"><span data-stu-id="7580b-401">Yes</span></span>                     | <span data-ttu-id="7580b-402">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="7580b-402">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="7580b-403">subjectId</span><span class="sxs-lookup"><span data-stu-id="7580b-403">subjectId</span></span>        | <span data-ttu-id="7580b-404">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-404">String</span></span>                                                   | <span data-ttu-id="7580b-405">是</span><span class="sxs-lookup"><span data-stu-id="7580b-405">Yes</span></span>                     | <span data-ttu-id="7580b-406">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="7580b-406">\<subjectId\></span></span> |
| <span data-ttu-id="7580b-407">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7580b-407">assignmentState</span></span>  | <span data-ttu-id="7580b-408">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-408">String</span></span>                                                   | <span data-ttu-id="7580b-409">是</span><span class="sxs-lookup"><span data-stu-id="7580b-409">Yes</span></span>                     | <span data-ttu-id="7580b-410">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="7580b-410">Eligible / Active</span></span> |
| <span data-ttu-id="7580b-411">type</span><span class="sxs-lookup"><span data-stu-id="7580b-411">type</span></span>             | <span data-ttu-id="7580b-412">字符串</span><span class="sxs-lookup"><span data-stu-id="7580b-412">String</span></span>                                                   | <span data-ttu-id="7580b-413">是</span><span class="sxs-lookup"><span data-stu-id="7580b-413">Yes</span></span>                     | <span data-ttu-id="7580b-414">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="7580b-414">AdminExtend</span></span> |
| <span data-ttu-id="7580b-415">在于</span><span class="sxs-lookup"><span data-stu-id="7580b-415">reason</span></span>           | <span data-ttu-id="7580b-416">String</span><span class="sxs-lookup"><span data-stu-id="7580b-416">String</span></span>                                                   | <span data-ttu-id="7580b-417">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="7580b-417">depends on roleSettings</span></span> |   |
| <span data-ttu-id="7580b-418">schedule</span><span class="sxs-lookup"><span data-stu-id="7580b-418">schedule</span></span>         | [<span data-ttu-id="7580b-419">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7580b-419">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7580b-420">是</span><span class="sxs-lookup"><span data-stu-id="7580b-420">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="7580b-421">请求</span><span class="sxs-lookup"><span data-stu-id="7580b-421">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="7580b-422">响应</span><span class="sxs-lookup"><span data-stu-id="7580b-422">Response</span></span>

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
