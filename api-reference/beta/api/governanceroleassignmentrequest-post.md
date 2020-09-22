---
title: 创建 governanceRoleAssignmentRequest
description: 创建一个角色分配请求，以代表在角色分配上所需的操作。 下表列出了这些操作。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 7bff2d2ae8e6a122621e3d17de7f7acc3f4e24df
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991108"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="942d6-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="942d6-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="942d6-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="942d6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="942d6-106">创建一个角色分配请求，以代表在角色分配上所需的操作。</span><span class="sxs-lookup"><span data-stu-id="942d6-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="942d6-107">下表列出了这些操作。</span><span class="sxs-lookup"><span data-stu-id="942d6-107">The following table lists the operations.</span></span>

| <span data-ttu-id="942d6-108">操作</span><span class="sxs-lookup"><span data-stu-id="942d6-108">Operation</span></span>                                   | <span data-ttu-id="942d6-109">类型</span><span class="sxs-lookup"><span data-stu-id="942d6-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="942d6-110">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="942d6-110">Assign a role assignment</span></span>                    | <span data-ttu-id="942d6-111">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="942d6-111">AdminAdd</span></span>    |
| <span data-ttu-id="942d6-112">激活符合条件的角色分配</span><span class="sxs-lookup"><span data-stu-id="942d6-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="942d6-113">UserAdd</span><span class="sxs-lookup"><span data-stu-id="942d6-113">UserAdd</span></span>     |
| <span data-ttu-id="942d6-114">停用已激活的角色分配</span><span class="sxs-lookup"><span data-stu-id="942d6-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="942d6-115">UserRemove</span><span class="sxs-lookup"><span data-stu-id="942d6-115">UserRemove</span></span>  |
| <span data-ttu-id="942d6-116">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="942d6-116">Remove a role assignment</span></span>                    | <span data-ttu-id="942d6-117">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="942d6-117">AdminRemove</span></span> |
| <span data-ttu-id="942d6-118">更新角色分配</span><span class="sxs-lookup"><span data-stu-id="942d6-118">Update a role assignment</span></span>                    | <span data-ttu-id="942d6-119">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="942d6-119">AdminUpdate</span></span> |
| <span data-ttu-id="942d6-120">请求扩展我的角色分配</span><span class="sxs-lookup"><span data-stu-id="942d6-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="942d6-121">UserExtend</span><span class="sxs-lookup"><span data-stu-id="942d6-121">UserExtend</span></span>  |
| <span data-ttu-id="942d6-122">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="942d6-122">Extend a role assignment</span></span>                    | <span data-ttu-id="942d6-123">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="942d6-123">AdminExtend</span></span> |
| <span data-ttu-id="942d6-124">续订我的过期角色分配的请求</span><span class="sxs-lookup"><span data-stu-id="942d6-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="942d6-125">UserRenew</span><span class="sxs-lookup"><span data-stu-id="942d6-125">UserRenew</span></span>   |
| <span data-ttu-id="942d6-126">续订过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="942d6-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="942d6-127">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="942d6-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="942d6-128">权限</span><span class="sxs-lookup"><span data-stu-id="942d6-128">Permissions</span></span>

<span data-ttu-id="942d6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="942d6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="942d6-131">权限类型</span><span class="sxs-lookup"><span data-stu-id="942d6-131">Permission type</span></span>                        | <span data-ttu-id="942d6-132">权限</span><span class="sxs-lookup"><span data-stu-id="942d6-132">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="942d6-133">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="942d6-133">Delegated (work or school account)</span></span>     | <span data-ttu-id="942d6-134">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="942d6-134">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="942d6-135">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="942d6-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="942d6-136">不支持。</span><span class="sxs-lookup"><span data-stu-id="942d6-136">Not supported.</span></span>                            |
| <span data-ttu-id="942d6-137">应用程序</span><span class="sxs-lookup"><span data-stu-id="942d6-137">Application</span></span>                            | <span data-ttu-id="942d6-138">不支持。</span><span class="sxs-lookup"><span data-stu-id="942d6-138">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="942d6-139">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="942d6-139">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="942d6-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="942d6-140">Request headers</span></span>

| <span data-ttu-id="942d6-141">名称</span><span class="sxs-lookup"><span data-stu-id="942d6-141">Name</span></span>          | <span data-ttu-id="942d6-142">说明</span><span class="sxs-lookup"><span data-stu-id="942d6-142">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="942d6-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="942d6-143">Authorization</span></span> | <span data-ttu-id="942d6-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="942d6-144">Bearer {code}</span></span>    |
| <span data-ttu-id="942d6-145">Content-type</span><span class="sxs-lookup"><span data-stu-id="942d6-145">Content-type</span></span>  | <span data-ttu-id="942d6-146">application/json</span><span class="sxs-lookup"><span data-stu-id="942d6-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="942d6-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="942d6-147">Request body</span></span>

<span data-ttu-id="942d6-148">在请求正文中，提供 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="942d6-148">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="942d6-149">属性</span><span class="sxs-lookup"><span data-stu-id="942d6-149">Property</span></span>         | <span data-ttu-id="942d6-150">类型</span><span class="sxs-lookup"><span data-stu-id="942d6-150">Type</span></span>                                                     | <span data-ttu-id="942d6-151">说明</span><span class="sxs-lookup"><span data-stu-id="942d6-151">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="942d6-152">resourceId</span><span class="sxs-lookup"><span data-stu-id="942d6-152">resourceId</span></span>       | <span data-ttu-id="942d6-153">String</span><span class="sxs-lookup"><span data-stu-id="942d6-153">String</span></span>                                                   | <span data-ttu-id="942d6-154">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="942d6-154">The ID of the resource.</span></span> <span data-ttu-id="942d6-155">必需。</span><span class="sxs-lookup"><span data-stu-id="942d6-155">Required.</span></span> |
| <span data-ttu-id="942d6-156">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="942d6-156">roleDefinitionId</span></span> | <span data-ttu-id="942d6-157">String</span><span class="sxs-lookup"><span data-stu-id="942d6-157">String</span></span>                                                   | <span data-ttu-id="942d6-158">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="942d6-158">The ID of the role definition.</span></span> <span data-ttu-id="942d6-159">必需。</span><span class="sxs-lookup"><span data-stu-id="942d6-159">Required.</span></span> |
| <span data-ttu-id="942d6-160">subjectId</span><span class="sxs-lookup"><span data-stu-id="942d6-160">subjectId</span></span>        | <span data-ttu-id="942d6-161">String</span><span class="sxs-lookup"><span data-stu-id="942d6-161">String</span></span>                                                   | <span data-ttu-id="942d6-162">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="942d6-162">The ID of the subject.</span></span> <span data-ttu-id="942d6-163">必需。</span><span class="sxs-lookup"><span data-stu-id="942d6-163">Required.</span></span> |
| <span data-ttu-id="942d6-164">assignmentState</span><span class="sxs-lookup"><span data-stu-id="942d6-164">assignmentState</span></span>  | <span data-ttu-id="942d6-165">String</span><span class="sxs-lookup"><span data-stu-id="942d6-165">String</span></span>                                                   | <span data-ttu-id="942d6-166">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="942d6-166">The state of assignment.</span></span> <span data-ttu-id="942d6-167">值可以是 `Eligible` 和 `Active` 。</span><span class="sxs-lookup"><span data-stu-id="942d6-167">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="942d6-168">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="942d6-168">Required.</span></span> |
| <span data-ttu-id="942d6-169">type</span><span class="sxs-lookup"><span data-stu-id="942d6-169">type</span></span>             | <span data-ttu-id="942d6-170">String</span><span class="sxs-lookup"><span data-stu-id="942d6-170">String</span></span>                                                   | <span data-ttu-id="942d6-171">请求类型。</span><span class="sxs-lookup"><span data-stu-id="942d6-171">The request type.</span></span> <span data-ttu-id="942d6-172">值可以是、、、、、、 `AdminAdd` `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew` `AdminRenew` 和 `AdminExtend` 。</span><span class="sxs-lookup"><span data-stu-id="942d6-172">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="942d6-173">必需。</span><span class="sxs-lookup"><span data-stu-id="942d6-173">Required.</span></span> |
| <span data-ttu-id="942d6-174">reason</span><span class="sxs-lookup"><span data-stu-id="942d6-174">reason</span></span>           | <span data-ttu-id="942d6-175">String</span><span class="sxs-lookup"><span data-stu-id="942d6-175">String</span></span>                                                   | <span data-ttu-id="942d6-176">需要为角色分配请求提供审核和审阅目的的原因。</span><span class="sxs-lookup"><span data-stu-id="942d6-176">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="942d6-177">schedule</span><span class="sxs-lookup"><span data-stu-id="942d6-177">schedule</span></span>         | [<span data-ttu-id="942d6-178">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="942d6-178">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="942d6-179">角色分配请求的日程安排。</span><span class="sxs-lookup"><span data-stu-id="942d6-179">The schedule of the role assignment request.</span></span> <span data-ttu-id="942d6-180">对于的请求类型 `UserAdd` ， `AdminAdd` 、 `AdminUpdate` 和， `AdminExtend` 它是必需的。</span><span class="sxs-lookup"><span data-stu-id="942d6-180">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="942d6-181">响应</span><span class="sxs-lookup"><span data-stu-id="942d6-181">Response</span></span>

<span data-ttu-id="942d6-182">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="942d6-182">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="942d6-183">错误代码</span><span class="sxs-lookup"><span data-stu-id="942d6-183">Error codes</span></span>

<span data-ttu-id="942d6-184">此 API 返回标准的 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="942d6-184">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="942d6-185">此外，它还返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="942d6-185">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="942d6-186">错误代码</span><span class="sxs-lookup"><span data-stu-id="942d6-186">Error code</span></span>     | <span data-ttu-id="942d6-187">错误消息</span><span class="sxs-lookup"><span data-stu-id="942d6-187">Error message</span></span>                               | <span data-ttu-id="942d6-188">详细信息</span><span class="sxs-lookup"><span data-stu-id="942d6-188">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="942d6-189">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="942d6-189">400 BadRequest</span></span> | <span data-ttu-id="942d6-190">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="942d6-190">RoleNotFound</span></span>                                | <span data-ttu-id="942d6-191">`roleDefinitionId`找不到请求正文中提供的。</span><span class="sxs-lookup"><span data-stu-id="942d6-191">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="942d6-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="942d6-192">400 BadRequest</span></span> | <span data-ttu-id="942d6-193">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="942d6-193">ResourceIsLocked</span></span>                            | <span data-ttu-id="942d6-194">请求正文中提供的资源处于状态 `Locked` ，并且无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="942d6-194">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="942d6-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="942d6-195">400 BadRequest</span></span> | <span data-ttu-id="942d6-196">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="942d6-196">SubjectNotFound</span></span>                             | <span data-ttu-id="942d6-197">`subjectId`找不到请求正文中提供的。</span><span class="sxs-lookup"><span data-stu-id="942d6-197">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="942d6-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="942d6-198">400 BadRequest</span></span> | <span data-ttu-id="942d6-199">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="942d6-199">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="942d6-200">系统中已存在一个挂起的 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 。</span><span class="sxs-lookup"><span data-stu-id="942d6-200">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="942d6-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="942d6-201">400 BadRequest</span></span> | <span data-ttu-id="942d6-202">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="942d6-202">RoleAssignmentExists</span></span>                        | <span data-ttu-id="942d6-203">系统中已存在请求创建的 [governanceRoleAssignment](../resources/governanceroleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="942d6-203">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="942d6-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="942d6-204">400 BadRequest</span></span> | <span data-ttu-id="942d6-205">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="942d6-205">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="942d6-206">系统中不存在请求进行更新/扩展的 [governanceRoleAssignment](../resources/governanceroleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="942d6-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="942d6-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="942d6-207">400 BadRequest</span></span> | <span data-ttu-id="942d6-208">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="942d6-208">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="942d6-209">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部策略，因此无法创建。</span><span class="sxs-lookup"><span data-stu-id="942d6-209">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="942d6-210">示例</span><span class="sxs-lookup"><span data-stu-id="942d6-210">Examples</span></span>

<span data-ttu-id="942d6-211">下面的示例演示如何使用此 API。</span><span class="sxs-lookup"><span data-stu-id="942d6-211">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="942d6-212">示例1：管理员为用户分配角色</span><span class="sxs-lookup"><span data-stu-id="942d6-212">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="942d6-213">在此示例中，管理员向计费读者角色分配用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="942d6-213">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="942d6-214">**注意：** 除了权限之外，本示例还要求请求者在资源上至少有一个 `Active` 管理员角色分配 (`owner` 或 `user access administrator`) 。</span><span class="sxs-lookup"><span data-stu-id="942d6-214">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="942d6-215">属性</span><span class="sxs-lookup"><span data-stu-id="942d6-215">Property</span></span>         | <span data-ttu-id="942d6-216">类型</span><span class="sxs-lookup"><span data-stu-id="942d6-216">Type</span></span>                                                     | <span data-ttu-id="942d6-217">必需</span><span class="sxs-lookup"><span data-stu-id="942d6-217">Required</span></span>                 | <span data-ttu-id="942d6-218">值</span><span class="sxs-lookup"><span data-stu-id="942d6-218">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="942d6-219">resourceId</span><span class="sxs-lookup"><span data-stu-id="942d6-219">resourceId</span></span>       | <span data-ttu-id="942d6-220">String</span><span class="sxs-lookup"><span data-stu-id="942d6-220">String</span></span>                                                   | <span data-ttu-id="942d6-221">是</span><span class="sxs-lookup"><span data-stu-id="942d6-221">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="942d6-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="942d6-222">roleDefinitionId</span></span> | <span data-ttu-id="942d6-223">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-223">String</span></span>                                                   | <span data-ttu-id="942d6-224">是</span><span class="sxs-lookup"><span data-stu-id="942d6-224">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="942d6-225">subjectId</span><span class="sxs-lookup"><span data-stu-id="942d6-225">subjectId</span></span>        | <span data-ttu-id="942d6-226">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-226">String</span></span>                                                   | <span data-ttu-id="942d6-227">是</span><span class="sxs-lookup"><span data-stu-id="942d6-227">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="942d6-228">assignmentState</span><span class="sxs-lookup"><span data-stu-id="942d6-228">assignmentState</span></span>  | <span data-ttu-id="942d6-229">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-229">String</span></span>                                                   | <span data-ttu-id="942d6-230">是</span><span class="sxs-lookup"><span data-stu-id="942d6-230">Yes</span></span>                      | <span data-ttu-id="942d6-231">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="942d6-231">Eligible / Active</span></span> |
| <span data-ttu-id="942d6-232">type</span><span class="sxs-lookup"><span data-stu-id="942d6-232">type</span></span>             | <span data-ttu-id="942d6-233">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-233">String</span></span>                                                   | <span data-ttu-id="942d6-234">是</span><span class="sxs-lookup"><span data-stu-id="942d6-234">Yes</span></span>                      | <span data-ttu-id="942d6-235">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="942d6-235">AdminAdd</span></span> |
| <span data-ttu-id="942d6-236">reason</span><span class="sxs-lookup"><span data-stu-id="942d6-236">reason</span></span>           | <span data-ttu-id="942d6-237">String</span><span class="sxs-lookup"><span data-stu-id="942d6-237">String</span></span>                                                   | <span data-ttu-id="942d6-238">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="942d6-238">depends on role Settings</span></span> |   |
| <span data-ttu-id="942d6-239">schedule</span><span class="sxs-lookup"><span data-stu-id="942d6-239">schedule</span></span>         | [<span data-ttu-id="942d6-240">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="942d6-240">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="942d6-241">是</span><span class="sxs-lookup"><span data-stu-id="942d6-241">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="942d6-242">请求</span><span class="sxs-lookup"><span data-stu-id="942d6-242">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="942d6-243">HTTP</span><span class="sxs-lookup"><span data-stu-id="942d6-243">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="942d6-244">C#</span><span class="sxs-lookup"><span data-stu-id="942d6-244">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="942d6-245">JavaScript</span><span class="sxs-lookup"><span data-stu-id="942d6-245">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="942d6-246">Objective-C</span><span class="sxs-lookup"><span data-stu-id="942d6-246">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="942d6-247">响应</span><span class="sxs-lookup"><span data-stu-id="942d6-247">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="942d6-248">示例2：用户激活符合条件的角色</span><span class="sxs-lookup"><span data-stu-id="942d6-248">Example 2: User activates eligible role</span></span>

<span data-ttu-id="942d6-249">在此示例中，用户 nawu@fimdev.net 激活符合条件的计费阅读者角色。</span><span class="sxs-lookup"><span data-stu-id="942d6-249">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="942d6-250">属性</span><span class="sxs-lookup"><span data-stu-id="942d6-250">Property</span></span>         | <span data-ttu-id="942d6-251">类型</span><span class="sxs-lookup"><span data-stu-id="942d6-251">Type</span></span>                                                     | <span data-ttu-id="942d6-252">必需</span><span class="sxs-lookup"><span data-stu-id="942d6-252">Required</span></span>                 | <span data-ttu-id="942d6-253">值</span><span class="sxs-lookup"><span data-stu-id="942d6-253">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="942d6-254">resourceId</span><span class="sxs-lookup"><span data-stu-id="942d6-254">resourceId</span></span>       | <span data-ttu-id="942d6-255">String</span><span class="sxs-lookup"><span data-stu-id="942d6-255">String</span></span>                                                   | <span data-ttu-id="942d6-256">是</span><span class="sxs-lookup"><span data-stu-id="942d6-256">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="942d6-257">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="942d6-257">roleDefinitionId</span></span> | <span data-ttu-id="942d6-258">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-258">String</span></span>                                                   | <span data-ttu-id="942d6-259">是</span><span class="sxs-lookup"><span data-stu-id="942d6-259">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="942d6-260">subjectId</span><span class="sxs-lookup"><span data-stu-id="942d6-260">subjectId</span></span>        | <span data-ttu-id="942d6-261">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-261">String</span></span>                                                   | <span data-ttu-id="942d6-262">是</span><span class="sxs-lookup"><span data-stu-id="942d6-262">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="942d6-263">assignmentState</span><span class="sxs-lookup"><span data-stu-id="942d6-263">assignmentState</span></span>  | <span data-ttu-id="942d6-264">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-264">String</span></span>                                                   | <span data-ttu-id="942d6-265">是</span><span class="sxs-lookup"><span data-stu-id="942d6-265">Yes</span></span>                      | <span data-ttu-id="942d6-266">活动</span><span class="sxs-lookup"><span data-stu-id="942d6-266">Active</span></span> |
| <span data-ttu-id="942d6-267">type</span><span class="sxs-lookup"><span data-stu-id="942d6-267">type</span></span>             | <span data-ttu-id="942d6-268">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-268">String</span></span>                                                   | <span data-ttu-id="942d6-269">是</span><span class="sxs-lookup"><span data-stu-id="942d6-269">Yes</span></span>                      | <span data-ttu-id="942d6-270">UserAdd</span><span class="sxs-lookup"><span data-stu-id="942d6-270">UserAdd</span></span> |
| <span data-ttu-id="942d6-271">reason</span><span class="sxs-lookup"><span data-stu-id="942d6-271">reason</span></span>           | <span data-ttu-id="942d6-272">String</span><span class="sxs-lookup"><span data-stu-id="942d6-272">String</span></span>                                                   | <span data-ttu-id="942d6-273">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="942d6-273">depends on role Settings</span></span> |   |
| <span data-ttu-id="942d6-274">schedule</span><span class="sxs-lookup"><span data-stu-id="942d6-274">schedule</span></span>         | [<span data-ttu-id="942d6-275">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="942d6-275">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="942d6-276">是</span><span class="sxs-lookup"><span data-stu-id="942d6-276">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="942d6-277">请求</span><span class="sxs-lookup"><span data-stu-id="942d6-277">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="942d6-278">响应</span><span class="sxs-lookup"><span data-stu-id="942d6-278">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="942d6-279">示例3：用户停用分配的角色</span><span class="sxs-lookup"><span data-stu-id="942d6-279">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="942d6-280">在此示例中，用户 nawu@fimdev.net 停用活动的帐单阅读者角色。</span><span class="sxs-lookup"><span data-stu-id="942d6-280">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="942d6-281">属性</span><span class="sxs-lookup"><span data-stu-id="942d6-281">Property</span></span>         | <span data-ttu-id="942d6-282">类型</span><span class="sxs-lookup"><span data-stu-id="942d6-282">Type</span></span>                                                     | <span data-ttu-id="942d6-283">必需</span><span class="sxs-lookup"><span data-stu-id="942d6-283">Required</span></span> | <span data-ttu-id="942d6-284">值</span><span class="sxs-lookup"><span data-stu-id="942d6-284">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="942d6-285">resourceId</span><span class="sxs-lookup"><span data-stu-id="942d6-285">resourceId</span></span>       | <span data-ttu-id="942d6-286">String</span><span class="sxs-lookup"><span data-stu-id="942d6-286">String</span></span>                                                   | <span data-ttu-id="942d6-287">是</span><span class="sxs-lookup"><span data-stu-id="942d6-287">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="942d6-288">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="942d6-288">roleDefinitionId</span></span> | <span data-ttu-id="942d6-289">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-289">String</span></span>                                                   | <span data-ttu-id="942d6-290">是</span><span class="sxs-lookup"><span data-stu-id="942d6-290">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="942d6-291">subjectId</span><span class="sxs-lookup"><span data-stu-id="942d6-291">subjectId</span></span>        | <span data-ttu-id="942d6-292">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-292">String</span></span>                                                   | <span data-ttu-id="942d6-293">是</span><span class="sxs-lookup"><span data-stu-id="942d6-293">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="942d6-294">assignmentState</span><span class="sxs-lookup"><span data-stu-id="942d6-294">assignmentState</span></span>  | <span data-ttu-id="942d6-295">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-295">String</span></span>                                                   | <span data-ttu-id="942d6-296">是</span><span class="sxs-lookup"><span data-stu-id="942d6-296">Yes</span></span>      | <span data-ttu-id="942d6-297">活动</span><span class="sxs-lookup"><span data-stu-id="942d6-297">Active</span></span> |
| <span data-ttu-id="942d6-298">type</span><span class="sxs-lookup"><span data-stu-id="942d6-298">type</span></span>             | <span data-ttu-id="942d6-299">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-299">String</span></span>                                                   | <span data-ttu-id="942d6-300">是</span><span class="sxs-lookup"><span data-stu-id="942d6-300">Yes</span></span>      | <span data-ttu-id="942d6-301">UserRemove</span><span class="sxs-lookup"><span data-stu-id="942d6-301">UserRemove</span></span> |
| <span data-ttu-id="942d6-302">reason</span><span class="sxs-lookup"><span data-stu-id="942d6-302">reason</span></span>           | <span data-ttu-id="942d6-303">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-303">String</span></span>                                                   | <span data-ttu-id="942d6-304">否</span><span class="sxs-lookup"><span data-stu-id="942d6-304">No</span></span>       |   |
| <span data-ttu-id="942d6-305">schedule</span><span class="sxs-lookup"><span data-stu-id="942d6-305">schedule</span></span>         | [<span data-ttu-id="942d6-306">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="942d6-306">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="942d6-307">否</span><span class="sxs-lookup"><span data-stu-id="942d6-307">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="942d6-308">请求</span><span class="sxs-lookup"><span data-stu-id="942d6-308">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="942d6-309">响应</span><span class="sxs-lookup"><span data-stu-id="942d6-309">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="942d6-310">示例4：管理员从角色中删除用户</span><span class="sxs-lookup"><span data-stu-id="942d6-310">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="942d6-311">在此示例中，管理员从 "计费读者" 角色中删除用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="942d6-311">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="942d6-312">**注意：** 除了权限之外，本示例还要求请求者在资源上至少有一个 `Active` 管理员角色分配 (`owner` 或 `user access administrator`) 。</span><span class="sxs-lookup"><span data-stu-id="942d6-312">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="942d6-313">属性</span><span class="sxs-lookup"><span data-stu-id="942d6-313">Property</span></span>         | <span data-ttu-id="942d6-314">类型</span><span class="sxs-lookup"><span data-stu-id="942d6-314">Type</span></span>                                                     | <span data-ttu-id="942d6-315">必需</span><span class="sxs-lookup"><span data-stu-id="942d6-315">Required</span></span> | <span data-ttu-id="942d6-316">值</span><span class="sxs-lookup"><span data-stu-id="942d6-316">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="942d6-317">resourceId</span><span class="sxs-lookup"><span data-stu-id="942d6-317">resourceId</span></span>       | <span data-ttu-id="942d6-318">String</span><span class="sxs-lookup"><span data-stu-id="942d6-318">String</span></span>                                                   | <span data-ttu-id="942d6-319">是</span><span class="sxs-lookup"><span data-stu-id="942d6-319">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="942d6-320">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="942d6-320">roleDefinitionId</span></span> | <span data-ttu-id="942d6-321">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-321">String</span></span>                                                   | <span data-ttu-id="942d6-322">是</span><span class="sxs-lookup"><span data-stu-id="942d6-322">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="942d6-323">subjectId</span><span class="sxs-lookup"><span data-stu-id="942d6-323">subjectId</span></span>        | <span data-ttu-id="942d6-324">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-324">String</span></span>                                                   | <span data-ttu-id="942d6-325">是</span><span class="sxs-lookup"><span data-stu-id="942d6-325">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="942d6-326">assignmentState</span><span class="sxs-lookup"><span data-stu-id="942d6-326">assignmentState</span></span>  | <span data-ttu-id="942d6-327">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-327">String</span></span>                                                   | <span data-ttu-id="942d6-328">是</span><span class="sxs-lookup"><span data-stu-id="942d6-328">Yes</span></span>      | <span data-ttu-id="942d6-329">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="942d6-329">Eligible / Active</span></span> |
| <span data-ttu-id="942d6-330">type</span><span class="sxs-lookup"><span data-stu-id="942d6-330">type</span></span>             | <span data-ttu-id="942d6-331">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-331">String</span></span>                                                   | <span data-ttu-id="942d6-332">是</span><span class="sxs-lookup"><span data-stu-id="942d6-332">Yes</span></span>      | <span data-ttu-id="942d6-333">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="942d6-333">AdminRemove</span></span> |
| <span data-ttu-id="942d6-334">reason</span><span class="sxs-lookup"><span data-stu-id="942d6-334">reason</span></span>           | <span data-ttu-id="942d6-335">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-335">String</span></span>                                                   | <span data-ttu-id="942d6-336">否</span><span class="sxs-lookup"><span data-stu-id="942d6-336">No</span></span>       |   |
| <span data-ttu-id="942d6-337">schedule</span><span class="sxs-lookup"><span data-stu-id="942d6-337">schedule</span></span>         | [<span data-ttu-id="942d6-338">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="942d6-338">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="942d6-339">否</span><span class="sxs-lookup"><span data-stu-id="942d6-339">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="942d6-340">请求</span><span class="sxs-lookup"><span data-stu-id="942d6-340">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="942d6-341">响应</span><span class="sxs-lookup"><span data-stu-id="942d6-341">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="942d6-342">示例5：管理员更新角色分配</span><span class="sxs-lookup"><span data-stu-id="942d6-342">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="942d6-343">在此示例中，管理员将用户 nawu@fimdev.net 的角色分配更新为 "所有者"。</span><span class="sxs-lookup"><span data-stu-id="942d6-343">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="942d6-344">**注意：** 除了权限之外，本示例还要求请求者在资源上至少有一个 `Active` 管理员角色分配 (`owner` 或 `user access administrator`) 。</span><span class="sxs-lookup"><span data-stu-id="942d6-344">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="942d6-345">属性</span><span class="sxs-lookup"><span data-stu-id="942d6-345">Property</span></span>         | <span data-ttu-id="942d6-346">类型</span><span class="sxs-lookup"><span data-stu-id="942d6-346">Type</span></span>                                                     | <span data-ttu-id="942d6-347">必需</span><span class="sxs-lookup"><span data-stu-id="942d6-347">Required</span></span>                | <span data-ttu-id="942d6-348">值</span><span class="sxs-lookup"><span data-stu-id="942d6-348">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="942d6-349">resourceId</span><span class="sxs-lookup"><span data-stu-id="942d6-349">resourceId</span></span>       | <span data-ttu-id="942d6-350">String</span><span class="sxs-lookup"><span data-stu-id="942d6-350">String</span></span>                                                   | <span data-ttu-id="942d6-351">是</span><span class="sxs-lookup"><span data-stu-id="942d6-351">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="942d6-352">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="942d6-352">roleDefinitionId</span></span> | <span data-ttu-id="942d6-353">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-353">String</span></span>                                                   | <span data-ttu-id="942d6-354">是</span><span class="sxs-lookup"><span data-stu-id="942d6-354">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="942d6-355">subjectId</span><span class="sxs-lookup"><span data-stu-id="942d6-355">subjectId</span></span>        | <span data-ttu-id="942d6-356">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-356">String</span></span>                                                   | <span data-ttu-id="942d6-357">是</span><span class="sxs-lookup"><span data-stu-id="942d6-357">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="942d6-358">assignmentState</span><span class="sxs-lookup"><span data-stu-id="942d6-358">assignmentState</span></span>  | <span data-ttu-id="942d6-359">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-359">String</span></span>                                                   | <span data-ttu-id="942d6-360">是</span><span class="sxs-lookup"><span data-stu-id="942d6-360">Yes</span></span>                     | <span data-ttu-id="942d6-361">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="942d6-361">Eligible / Active</span></span> |
| <span data-ttu-id="942d6-362">type</span><span class="sxs-lookup"><span data-stu-id="942d6-362">type</span></span>             | <span data-ttu-id="942d6-363">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-363">String</span></span>                                                   | <span data-ttu-id="942d6-364">是</span><span class="sxs-lookup"><span data-stu-id="942d6-364">Yes</span></span>                     | <span data-ttu-id="942d6-365">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="942d6-365">AdminUpdate</span></span> |
| <span data-ttu-id="942d6-366">reason</span><span class="sxs-lookup"><span data-stu-id="942d6-366">reason</span></span>           | <span data-ttu-id="942d6-367">String</span><span class="sxs-lookup"><span data-stu-id="942d6-367">String</span></span>                                                   | <span data-ttu-id="942d6-368">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="942d6-368">depends on roleSettings</span></span> |   |
| <span data-ttu-id="942d6-369">schedule</span><span class="sxs-lookup"><span data-stu-id="942d6-369">schedule</span></span>         | [<span data-ttu-id="942d6-370">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="942d6-370">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="942d6-371">是</span><span class="sxs-lookup"><span data-stu-id="942d6-371">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="942d6-372">请求</span><span class="sxs-lookup"><span data-stu-id="942d6-372">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="942d6-373">响应</span><span class="sxs-lookup"><span data-stu-id="942d6-373">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="942d6-374">示例6：管理员扩展了即将过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="942d6-374">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="942d6-375">此示例将用户 ANUJCUSER 的过期角色分配扩展到 API Management Service 参与者。</span><span class="sxs-lookup"><span data-stu-id="942d6-375">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="942d6-376">**注意：** 除了权限之外，本示例还要求请求者在资源上至少有一个 `Active` 管理员角色分配 (`owner` 或 `user access administrator`) 。</span><span class="sxs-lookup"><span data-stu-id="942d6-376">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="942d6-377">属性</span><span class="sxs-lookup"><span data-stu-id="942d6-377">Property</span></span>         | <span data-ttu-id="942d6-378">类型</span><span class="sxs-lookup"><span data-stu-id="942d6-378">Type</span></span>                                                     | <span data-ttu-id="942d6-379">必需</span><span class="sxs-lookup"><span data-stu-id="942d6-379">Required</span></span>                | <span data-ttu-id="942d6-380">值</span><span class="sxs-lookup"><span data-stu-id="942d6-380">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="942d6-381">resourceId</span><span class="sxs-lookup"><span data-stu-id="942d6-381">resourceId</span></span>       | <span data-ttu-id="942d6-382">String</span><span class="sxs-lookup"><span data-stu-id="942d6-382">String</span></span>                                                   | <span data-ttu-id="942d6-383">是</span><span class="sxs-lookup"><span data-stu-id="942d6-383">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="942d6-384">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="942d6-384">roleDefinitionId</span></span> | <span data-ttu-id="942d6-385">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-385">String</span></span>                                                   | <span data-ttu-id="942d6-386">是</span><span class="sxs-lookup"><span data-stu-id="942d6-386">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="942d6-387">subjectId</span><span class="sxs-lookup"><span data-stu-id="942d6-387">subjectId</span></span>        | <span data-ttu-id="942d6-388">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-388">String</span></span>                                                   | <span data-ttu-id="942d6-389">是</span><span class="sxs-lookup"><span data-stu-id="942d6-389">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="942d6-390">assignmentState</span><span class="sxs-lookup"><span data-stu-id="942d6-390">assignmentState</span></span>  | <span data-ttu-id="942d6-391">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-391">String</span></span>                                                   | <span data-ttu-id="942d6-392">是</span><span class="sxs-lookup"><span data-stu-id="942d6-392">Yes</span></span>                     | <span data-ttu-id="942d6-393">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="942d6-393">Eligible / Active</span></span> |
| <span data-ttu-id="942d6-394">type</span><span class="sxs-lookup"><span data-stu-id="942d6-394">type</span></span>             | <span data-ttu-id="942d6-395">字符串</span><span class="sxs-lookup"><span data-stu-id="942d6-395">String</span></span>                                                   | <span data-ttu-id="942d6-396">是</span><span class="sxs-lookup"><span data-stu-id="942d6-396">Yes</span></span>                     | <span data-ttu-id="942d6-397">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="942d6-397">AdminExtend</span></span> |
| <span data-ttu-id="942d6-398">reason</span><span class="sxs-lookup"><span data-stu-id="942d6-398">reason</span></span>           | <span data-ttu-id="942d6-399">String</span><span class="sxs-lookup"><span data-stu-id="942d6-399">String</span></span>                                                   | <span data-ttu-id="942d6-400">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="942d6-400">depends on roleSettings</span></span> |   |
| <span data-ttu-id="942d6-401">schedule</span><span class="sxs-lookup"><span data-stu-id="942d6-401">schedule</span></span>         | [<span data-ttu-id="942d6-402">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="942d6-402">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="942d6-403">是</span><span class="sxs-lookup"><span data-stu-id="942d6-403">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="942d6-404">请求</span><span class="sxs-lookup"><span data-stu-id="942d6-404">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="942d6-405">响应</span><span class="sxs-lookup"><span data-stu-id="942d6-405">Response</span></span>

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


