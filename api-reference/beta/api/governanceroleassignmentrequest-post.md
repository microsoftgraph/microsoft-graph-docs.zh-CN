---
title: 创建 governanceRoleAssignmentRequest
description: 创建一个角色分配请求, 以代表在角色分配上所需的操作。 下表列出了这些操作。
localization_priority: Normal
ms.openlocfilehash: 104ab1a0d4909bc2181df70bc4fc895fc4558260
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503275"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="a52a1-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="a52a1-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a52a1-105">创建一个角色分配请求, 以代表在角色分配上所需的操作。</span><span class="sxs-lookup"><span data-stu-id="a52a1-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="a52a1-106">下表列出了这些操作。</span><span class="sxs-lookup"><span data-stu-id="a52a1-106">The following table lists the operations.</span></span>

| <span data-ttu-id="a52a1-107">操作</span><span class="sxs-lookup"><span data-stu-id="a52a1-107">Operation</span></span>                                   | <span data-ttu-id="a52a1-108">类型</span><span class="sxs-lookup"><span data-stu-id="a52a1-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="a52a1-109">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="a52a1-109">Assign a role assignment</span></span>                    | <span data-ttu-id="a52a1-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="a52a1-110">AdminAdd</span></span>    |
| <span data-ttu-id="a52a1-111">激活符合条件的角色分配</span><span class="sxs-lookup"><span data-stu-id="a52a1-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="a52a1-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="a52a1-112">UserAdd</span></span>     |
| <span data-ttu-id="a52a1-113">停用已激活的角色分配</span><span class="sxs-lookup"><span data-stu-id="a52a1-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="a52a1-114">UserRemove</span><span class="sxs-lookup"><span data-stu-id="a52a1-114">UserRemove</span></span>  |
| <span data-ttu-id="a52a1-115">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="a52a1-115">Remove a role assignment</span></span>                    | <span data-ttu-id="a52a1-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="a52a1-116">AdminRemove</span></span> |
| <span data-ttu-id="a52a1-117">更新角色分配</span><span class="sxs-lookup"><span data-stu-id="a52a1-117">Update a role assignment</span></span>                    | <span data-ttu-id="a52a1-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="a52a1-118">AdminUpdate</span></span> |
| <span data-ttu-id="a52a1-119">请求扩展我的角色分配</span><span class="sxs-lookup"><span data-stu-id="a52a1-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="a52a1-120">UserExtend</span><span class="sxs-lookup"><span data-stu-id="a52a1-120">UserExtend</span></span>  |
| <span data-ttu-id="a52a1-121">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="a52a1-121">Extend a role assignment</span></span>                    | <span data-ttu-id="a52a1-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="a52a1-122">AdminExtend</span></span> |
| <span data-ttu-id="a52a1-123">续订我的过期角色分配的请求</span><span class="sxs-lookup"><span data-stu-id="a52a1-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="a52a1-124">UserRenew</span><span class="sxs-lookup"><span data-stu-id="a52a1-124">UserRenew</span></span>   |
| <span data-ttu-id="a52a1-125">续订过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="a52a1-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="a52a1-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="a52a1-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="a52a1-127">权限</span><span class="sxs-lookup"><span data-stu-id="a52a1-127">Permissions</span></span>

<span data-ttu-id="a52a1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a52a1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a52a1-130">权限类型</span><span class="sxs-lookup"><span data-stu-id="a52a1-130">Permission type</span></span>                        | <span data-ttu-id="a52a1-131">权限</span><span class="sxs-lookup"><span data-stu-id="a52a1-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="a52a1-132">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a52a1-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="a52a1-133">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="a52a1-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="a52a1-134">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a52a1-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a52a1-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="a52a1-135">Not supported.</span></span>                            |
| <span data-ttu-id="a52a1-136">应用程序</span><span class="sxs-lookup"><span data-stu-id="a52a1-136">Application</span></span>                            | <span data-ttu-id="a52a1-137">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="a52a1-137">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="a52a1-138">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a52a1-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="a52a1-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="a52a1-139">Request headers</span></span>

| <span data-ttu-id="a52a1-140">名称</span><span class="sxs-lookup"><span data-stu-id="a52a1-140">Name</span></span>          | <span data-ttu-id="a52a1-141">说明</span><span class="sxs-lookup"><span data-stu-id="a52a1-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="a52a1-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="a52a1-142">Authorization</span></span> | <span data-ttu-id="a52a1-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a52a1-143">Bearer {code}</span></span>    |
| <span data-ttu-id="a52a1-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="a52a1-144">Content-type</span></span>  | <span data-ttu-id="a52a1-145">application/json</span><span class="sxs-lookup"><span data-stu-id="a52a1-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a52a1-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="a52a1-146">Request body</span></span>

<span data-ttu-id="a52a1-147">在请求正文中, 提供[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a52a1-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="a52a1-148">属性</span><span class="sxs-lookup"><span data-stu-id="a52a1-148">Property</span></span>         | <span data-ttu-id="a52a1-149">类型</span><span class="sxs-lookup"><span data-stu-id="a52a1-149">Type</span></span>                                                     | <span data-ttu-id="a52a1-150">说明</span><span class="sxs-lookup"><span data-stu-id="a52a1-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="a52a1-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="a52a1-151">resourceId</span></span>       | <span data-ttu-id="a52a1-152">String</span><span class="sxs-lookup"><span data-stu-id="a52a1-152">String</span></span>                                                   | <span data-ttu-id="a52a1-153">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="a52a1-153">The ID of the resource.</span></span> <span data-ttu-id="a52a1-154">必需。</span><span class="sxs-lookup"><span data-stu-id="a52a1-154">Required.</span></span> |
| <span data-ttu-id="a52a1-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a52a1-155">roleDefinitionId</span></span> | <span data-ttu-id="a52a1-156">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-156">String</span></span>                                                   | <span data-ttu-id="a52a1-157">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="a52a1-157">The ID of the role definition.</span></span> <span data-ttu-id="a52a1-158">必需。</span><span class="sxs-lookup"><span data-stu-id="a52a1-158">Required.</span></span> |
| <span data-ttu-id="a52a1-159">subjectId</span><span class="sxs-lookup"><span data-stu-id="a52a1-159">subjectId</span></span>        | <span data-ttu-id="a52a1-160">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-160">String</span></span>                                                   | <span data-ttu-id="a52a1-161">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="a52a1-161">The ID of the subject.</span></span> <span data-ttu-id="a52a1-162">必需。</span><span class="sxs-lookup"><span data-stu-id="a52a1-162">Required.</span></span> |
| <span data-ttu-id="a52a1-163">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a52a1-163">assignmentState</span></span>  | <span data-ttu-id="a52a1-164">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-164">String</span></span>                                                   | <span data-ttu-id="a52a1-165">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="a52a1-165">The state of assignment.</span></span> <span data-ttu-id="a52a1-166">值可以是`Eligible`和`Active`。</span><span class="sxs-lookup"><span data-stu-id="a52a1-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="a52a1-167">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="a52a1-167">Required.</span></span> |
| <span data-ttu-id="a52a1-168">type</span><span class="sxs-lookup"><span data-stu-id="a52a1-168">type</span></span>             | <span data-ttu-id="a52a1-169">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-169">String</span></span>                                                   | <span data-ttu-id="a52a1-170">请求类型。</span><span class="sxs-lookup"><span data-stu-id="a52a1-170">The request type.</span></span> <span data-ttu-id="a52a1-171">值可以是`AdminAdd` `UserAdd`、、 `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `AdminRenew` `AdminExtend`、、、、和。 `UserRenew`</span><span class="sxs-lookup"><span data-stu-id="a52a1-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="a52a1-172">必需。</span><span class="sxs-lookup"><span data-stu-id="a52a1-172">Required.</span></span> |
| <span data-ttu-id="a52a1-173">在于</span><span class="sxs-lookup"><span data-stu-id="a52a1-173">reason</span></span>           | <span data-ttu-id="a52a1-174">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-174">String</span></span>                                                   | <span data-ttu-id="a52a1-175">需要为角色分配请求提供审核和审阅目的的原因。</span><span class="sxs-lookup"><span data-stu-id="a52a1-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="a52a1-176">设定</span><span class="sxs-lookup"><span data-stu-id="a52a1-176">schedule</span></span>         | [<span data-ttu-id="a52a1-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a52a1-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a52a1-178">角色分配请求的日程安排。</span><span class="sxs-lookup"><span data-stu-id="a52a1-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="a52a1-179">对于的请求类型`UserAdd`, `AdminAdd` `AdminUpdate`、和`AdminExtend`, 它是必需的。</span><span class="sxs-lookup"><span data-stu-id="a52a1-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="a52a1-180">响应</span><span class="sxs-lookup"><span data-stu-id="a52a1-180">Response</span></span>

<span data-ttu-id="a52a1-181">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a52a1-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="a52a1-182">错误代码</span><span class="sxs-lookup"><span data-stu-id="a52a1-182">Error codes</span></span>

<span data-ttu-id="a52a1-183">此 API 返回标准的 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="a52a1-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="a52a1-184">此外, 它还返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="a52a1-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="a52a1-185">错误代码</span><span class="sxs-lookup"><span data-stu-id="a52a1-185">Error code</span></span>     | <span data-ttu-id="a52a1-186">错误消息</span><span class="sxs-lookup"><span data-stu-id="a52a1-186">Error message</span></span>                               | <span data-ttu-id="a52a1-187">详细信息</span><span class="sxs-lookup"><span data-stu-id="a52a1-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="a52a1-188">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a52a1-188">400 BadRequest</span></span> | <span data-ttu-id="a52a1-189">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="a52a1-189">RoleNotFound</span></span>                                | <span data-ttu-id="a52a1-190">找`roleDefinitionId`不到请求正文中提供的。</span><span class="sxs-lookup"><span data-stu-id="a52a1-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="a52a1-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a52a1-191">400 BadRequest</span></span> | <span data-ttu-id="a52a1-192">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="a52a1-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="a52a1-193">请求正文中提供的资源处于状态`Locked` , 并且无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="a52a1-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="a52a1-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a52a1-194">400 BadRequest</span></span> | <span data-ttu-id="a52a1-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="a52a1-195">SubjectNotFound</span></span>                             | <span data-ttu-id="a52a1-196">找`subjectId`不到请求正文中提供的。</span><span class="sxs-lookup"><span data-stu-id="a52a1-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="a52a1-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a52a1-197">400 BadRequest</span></span> | <span data-ttu-id="a52a1-198">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="a52a1-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="a52a1-199">系统中已存在一个挂起的[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 。</span><span class="sxs-lookup"><span data-stu-id="a52a1-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="a52a1-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a52a1-200">400 BadRequest</span></span> | <span data-ttu-id="a52a1-201">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="a52a1-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="a52a1-202">系统中已存在请求创建的[governanceRoleAssignment](../resources/governanceroleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="a52a1-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="a52a1-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a52a1-203">400 BadRequest</span></span> | <span data-ttu-id="a52a1-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="a52a1-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="a52a1-205">系统中不存在请求进行更新/扩展的[governanceRoleAssignment](../resources/governanceroleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="a52a1-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="a52a1-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a52a1-206">400 BadRequest</span></span> | <span data-ttu-id="a52a1-207">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="a52a1-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="a52a1-208">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部策略, 因此无法创建。</span><span class="sxs-lookup"><span data-stu-id="a52a1-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="a52a1-209">示例</span><span class="sxs-lookup"><span data-stu-id="a52a1-209">Examples</span></span>

<span data-ttu-id="a52a1-210">下面的示例演示如何使用此 API。</span><span class="sxs-lookup"><span data-stu-id="a52a1-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="a52a1-211">示例 1: 管理员为用户分配角色</span><span class="sxs-lookup"><span data-stu-id="a52a1-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="a52a1-212">在此示例中, 管理员向计费读者角色分配用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="a52a1-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="a52a1-213">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="a52a1-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="a52a1-214">属性</span><span class="sxs-lookup"><span data-stu-id="a52a1-214">Property</span></span>         | <span data-ttu-id="a52a1-215">类型</span><span class="sxs-lookup"><span data-stu-id="a52a1-215">Type</span></span>                                                     | <span data-ttu-id="a52a1-216">必需</span><span class="sxs-lookup"><span data-stu-id="a52a1-216">Required</span></span>                 | <span data-ttu-id="a52a1-217">值</span><span class="sxs-lookup"><span data-stu-id="a52a1-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="a52a1-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="a52a1-218">resourceId</span></span>       | <span data-ttu-id="a52a1-219">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-219">String</span></span>                                                   | <span data-ttu-id="a52a1-220">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-220">Yes</span></span>                      | <span data-ttu-id="a52a1-221">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a52a1-221">\<resourceId\></span></span> |
| <span data-ttu-id="a52a1-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a52a1-222">roleDefinitionId</span></span> | <span data-ttu-id="a52a1-223">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-223">String</span></span>                                                   | <span data-ttu-id="a52a1-224">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-224">Yes</span></span>                      | <span data-ttu-id="a52a1-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a52a1-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="a52a1-226">subjectId</span><span class="sxs-lookup"><span data-stu-id="a52a1-226">subjectId</span></span>        | <span data-ttu-id="a52a1-227">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-227">String</span></span>                                                   | <span data-ttu-id="a52a1-228">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-228">Yes</span></span>                      | <span data-ttu-id="a52a1-229">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a52a1-229">\<subjectId\></span></span> |
| <span data-ttu-id="a52a1-230">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a52a1-230">assignmentState</span></span>  | <span data-ttu-id="a52a1-231">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-231">String</span></span>                                                   | <span data-ttu-id="a52a1-232">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-232">Yes</span></span>                      | <span data-ttu-id="a52a1-233">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="a52a1-233">Eligible / Active</span></span> |
| <span data-ttu-id="a52a1-234">类型</span><span class="sxs-lookup"><span data-stu-id="a52a1-234">type</span></span>             | <span data-ttu-id="a52a1-235">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-235">String</span></span>                                                   | <span data-ttu-id="a52a1-236">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-236">Yes</span></span>                      | <span data-ttu-id="a52a1-237">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="a52a1-237">AdminAdd</span></span> |
| <span data-ttu-id="a52a1-238">在于</span><span class="sxs-lookup"><span data-stu-id="a52a1-238">reason</span></span>           | <span data-ttu-id="a52a1-239">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-239">String</span></span>                                                   | <span data-ttu-id="a52a1-240">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="a52a1-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="a52a1-241">设定</span><span class="sxs-lookup"><span data-stu-id="a52a1-241">schedule</span></span>         | [<span data-ttu-id="a52a1-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a52a1-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a52a1-243">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="a52a1-244">请求</span><span class="sxs-lookup"><span data-stu-id="a52a1-244">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="a52a1-245">响应</span><span class="sxs-lookup"><span data-stu-id="a52a1-245">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="a52a1-246">示例 2: 用户激活符合条件的角色</span><span class="sxs-lookup"><span data-stu-id="a52a1-246">Example 2: User activates eligible role</span></span>

<span data-ttu-id="a52a1-247">在此示例中, 用户 nawu@fimdev.net 激活符合条件的计费阅读者角色。</span><span class="sxs-lookup"><span data-stu-id="a52a1-247">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="a52a1-248">属性</span><span class="sxs-lookup"><span data-stu-id="a52a1-248">Property</span></span>         | <span data-ttu-id="a52a1-249">类型</span><span class="sxs-lookup"><span data-stu-id="a52a1-249">Type</span></span>                                                     | <span data-ttu-id="a52a1-250">必需</span><span class="sxs-lookup"><span data-stu-id="a52a1-250">Required</span></span>                 | <span data-ttu-id="a52a1-251">值</span><span class="sxs-lookup"><span data-stu-id="a52a1-251">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="a52a1-252">resourceId</span><span class="sxs-lookup"><span data-stu-id="a52a1-252">resourceId</span></span>       | <span data-ttu-id="a52a1-253">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-253">String</span></span>                                                   | <span data-ttu-id="a52a1-254">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-254">Yes</span></span>                      | <span data-ttu-id="a52a1-255">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a52a1-255">\<resourceId\></span></span> |
| <span data-ttu-id="a52a1-256">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a52a1-256">roleDefinitionId</span></span> | <span data-ttu-id="a52a1-257">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-257">String</span></span>                                                   | <span data-ttu-id="a52a1-258">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-258">Yes</span></span>                      | <span data-ttu-id="a52a1-259">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a52a1-259">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="a52a1-260">subjectId</span><span class="sxs-lookup"><span data-stu-id="a52a1-260">subjectId</span></span>        | <span data-ttu-id="a52a1-261">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-261">String</span></span>                                                   | <span data-ttu-id="a52a1-262">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-262">Yes</span></span>                      | <span data-ttu-id="a52a1-263">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a52a1-263">\<subjectId\></span></span> |
| <span data-ttu-id="a52a1-264">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a52a1-264">assignmentState</span></span>  | <span data-ttu-id="a52a1-265">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-265">String</span></span>                                                   | <span data-ttu-id="a52a1-266">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-266">Yes</span></span>                      | <span data-ttu-id="a52a1-267">活动</span><span class="sxs-lookup"><span data-stu-id="a52a1-267">Active</span></span> |
| <span data-ttu-id="a52a1-268">类型</span><span class="sxs-lookup"><span data-stu-id="a52a1-268">type</span></span>             | <span data-ttu-id="a52a1-269">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-269">String</span></span>                                                   | <span data-ttu-id="a52a1-270">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-270">Yes</span></span>                      | <span data-ttu-id="a52a1-271">UserAdd</span><span class="sxs-lookup"><span data-stu-id="a52a1-271">UserAdd</span></span> |
| <span data-ttu-id="a52a1-272">在于</span><span class="sxs-lookup"><span data-stu-id="a52a1-272">reason</span></span>           | <span data-ttu-id="a52a1-273">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-273">String</span></span>                                                   | <span data-ttu-id="a52a1-274">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="a52a1-274">depends on role Settings</span></span> |   |
| <span data-ttu-id="a52a1-275">设定</span><span class="sxs-lookup"><span data-stu-id="a52a1-275">schedule</span></span>         | [<span data-ttu-id="a52a1-276">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a52a1-276">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a52a1-277">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-277">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="a52a1-278">请求</span><span class="sxs-lookup"><span data-stu-id="a52a1-278">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="a52a1-279">响应</span><span class="sxs-lookup"><span data-stu-id="a52a1-279">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="a52a1-280">示例 3: 用户停用分配的角色</span><span class="sxs-lookup"><span data-stu-id="a52a1-280">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="a52a1-281">在此示例中, 用户 nawu@fimdev.net 停用活动的帐单阅读者角色。</span><span class="sxs-lookup"><span data-stu-id="a52a1-281">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="a52a1-282">属性</span><span class="sxs-lookup"><span data-stu-id="a52a1-282">Property</span></span>         | <span data-ttu-id="a52a1-283">类型</span><span class="sxs-lookup"><span data-stu-id="a52a1-283">Type</span></span>                                                     | <span data-ttu-id="a52a1-284">必需</span><span class="sxs-lookup"><span data-stu-id="a52a1-284">Required</span></span> | <span data-ttu-id="a52a1-285">值</span><span class="sxs-lookup"><span data-stu-id="a52a1-285">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="a52a1-286">resourceId</span><span class="sxs-lookup"><span data-stu-id="a52a1-286">resourceId</span></span>       | <span data-ttu-id="a52a1-287">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-287">String</span></span>                                                   | <span data-ttu-id="a52a1-288">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-288">Yes</span></span>      | <span data-ttu-id="a52a1-289">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a52a1-289">\<resourceId\></span></span> |
| <span data-ttu-id="a52a1-290">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a52a1-290">roleDefinitionId</span></span> | <span data-ttu-id="a52a1-291">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-291">String</span></span>                                                   | <span data-ttu-id="a52a1-292">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-292">Yes</span></span>      | <span data-ttu-id="a52a1-293">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a52a1-293">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="a52a1-294">subjectId</span><span class="sxs-lookup"><span data-stu-id="a52a1-294">subjectId</span></span>        | <span data-ttu-id="a52a1-295">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-295">String</span></span>                                                   | <span data-ttu-id="a52a1-296">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-296">Yes</span></span>      | <span data-ttu-id="a52a1-297">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a52a1-297">\<subjectId\></span></span> |
| <span data-ttu-id="a52a1-298">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a52a1-298">assignmentState</span></span>  | <span data-ttu-id="a52a1-299">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-299">String</span></span>                                                   | <span data-ttu-id="a52a1-300">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-300">Yes</span></span>      | <span data-ttu-id="a52a1-301">活动</span><span class="sxs-lookup"><span data-stu-id="a52a1-301">Active</span></span> |
| <span data-ttu-id="a52a1-302">类型</span><span class="sxs-lookup"><span data-stu-id="a52a1-302">type</span></span>             | <span data-ttu-id="a52a1-303">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-303">String</span></span>                                                   | <span data-ttu-id="a52a1-304">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-304">Yes</span></span>      | <span data-ttu-id="a52a1-305">UserRemove</span><span class="sxs-lookup"><span data-stu-id="a52a1-305">UserRemove</span></span> |
| <span data-ttu-id="a52a1-306">在于</span><span class="sxs-lookup"><span data-stu-id="a52a1-306">reason</span></span>           | <span data-ttu-id="a52a1-307">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-307">String</span></span>                                                   | <span data-ttu-id="a52a1-308">否</span><span class="sxs-lookup"><span data-stu-id="a52a1-308">No</span></span>       |   |
| <span data-ttu-id="a52a1-309">设定</span><span class="sxs-lookup"><span data-stu-id="a52a1-309">schedule</span></span>         | [<span data-ttu-id="a52a1-310">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a52a1-310">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a52a1-311">否</span><span class="sxs-lookup"><span data-stu-id="a52a1-311">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="a52a1-312">请求</span><span class="sxs-lookup"><span data-stu-id="a52a1-312">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="a52a1-313">响应</span><span class="sxs-lookup"><span data-stu-id="a52a1-313">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="a52a1-314">示例 4: 管理员从角色中删除用户</span><span class="sxs-lookup"><span data-stu-id="a52a1-314">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="a52a1-315">在此示例中, 管理员从 "计费读者" 角色中删除用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="a52a1-315">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="a52a1-316">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="a52a1-316">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="a52a1-317">属性</span><span class="sxs-lookup"><span data-stu-id="a52a1-317">Property</span></span>         | <span data-ttu-id="a52a1-318">类型</span><span class="sxs-lookup"><span data-stu-id="a52a1-318">Type</span></span>                                                     | <span data-ttu-id="a52a1-319">必需</span><span class="sxs-lookup"><span data-stu-id="a52a1-319">Required</span></span> | <span data-ttu-id="a52a1-320">值</span><span class="sxs-lookup"><span data-stu-id="a52a1-320">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="a52a1-321">resourceId</span><span class="sxs-lookup"><span data-stu-id="a52a1-321">resourceId</span></span>       | <span data-ttu-id="a52a1-322">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-322">String</span></span>                                                   | <span data-ttu-id="a52a1-323">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-323">Yes</span></span>      | <span data-ttu-id="a52a1-324">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a52a1-324">\<resourceId\></span></span> |
| <span data-ttu-id="a52a1-325">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a52a1-325">roleDefinitionId</span></span> | <span data-ttu-id="a52a1-326">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-326">String</span></span>                                                   | <span data-ttu-id="a52a1-327">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-327">Yes</span></span>      | <span data-ttu-id="a52a1-328">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a52a1-328">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="a52a1-329">subjectId</span><span class="sxs-lookup"><span data-stu-id="a52a1-329">subjectId</span></span>        | <span data-ttu-id="a52a1-330">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-330">String</span></span>                                                   | <span data-ttu-id="a52a1-331">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-331">Yes</span></span>      | <span data-ttu-id="a52a1-332">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a52a1-332">\<subjectId\></span></span> |
| <span data-ttu-id="a52a1-333">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a52a1-333">assignmentState</span></span>  | <span data-ttu-id="a52a1-334">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-334">String</span></span>                                                   | <span data-ttu-id="a52a1-335">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-335">Yes</span></span>      | <span data-ttu-id="a52a1-336">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="a52a1-336">Eligible / Active</span></span> |
| <span data-ttu-id="a52a1-337">类型</span><span class="sxs-lookup"><span data-stu-id="a52a1-337">type</span></span>             | <span data-ttu-id="a52a1-338">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-338">String</span></span>                                                   | <span data-ttu-id="a52a1-339">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-339">Yes</span></span>      | <span data-ttu-id="a52a1-340">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="a52a1-340">AdminRemove</span></span> |
| <span data-ttu-id="a52a1-341">在于</span><span class="sxs-lookup"><span data-stu-id="a52a1-341">reason</span></span>           | <span data-ttu-id="a52a1-342">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-342">String</span></span>                                                   | <span data-ttu-id="a52a1-343">否</span><span class="sxs-lookup"><span data-stu-id="a52a1-343">No</span></span>       |   |
| <span data-ttu-id="a52a1-344">设定</span><span class="sxs-lookup"><span data-stu-id="a52a1-344">schedule</span></span>         | [<span data-ttu-id="a52a1-345">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a52a1-345">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a52a1-346">否</span><span class="sxs-lookup"><span data-stu-id="a52a1-346">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="a52a1-347">请求</span><span class="sxs-lookup"><span data-stu-id="a52a1-347">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="a52a1-348">响应</span><span class="sxs-lookup"><span data-stu-id="a52a1-348">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="a52a1-349">示例 5: 管理员更新角色分配</span><span class="sxs-lookup"><span data-stu-id="a52a1-349">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="a52a1-350">在此示例中, 管理员将用户 nawu@fimdev.net 的角色分配更新为 "所有者"。</span><span class="sxs-lookup"><span data-stu-id="a52a1-350">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="a52a1-351">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="a52a1-351">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="a52a1-352">属性</span><span class="sxs-lookup"><span data-stu-id="a52a1-352">Property</span></span>         | <span data-ttu-id="a52a1-353">类型</span><span class="sxs-lookup"><span data-stu-id="a52a1-353">Type</span></span>                                                     | <span data-ttu-id="a52a1-354">必需</span><span class="sxs-lookup"><span data-stu-id="a52a1-354">Required</span></span>                | <span data-ttu-id="a52a1-355">值</span><span class="sxs-lookup"><span data-stu-id="a52a1-355">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="a52a1-356">resourceId</span><span class="sxs-lookup"><span data-stu-id="a52a1-356">resourceId</span></span>       | <span data-ttu-id="a52a1-357">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-357">String</span></span>                                                   | <span data-ttu-id="a52a1-358">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-358">Yes</span></span>                     | <span data-ttu-id="a52a1-359">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a52a1-359">\<resourceId\></span></span> |
| <span data-ttu-id="a52a1-360">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a52a1-360">roleDefinitionId</span></span> | <span data-ttu-id="a52a1-361">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-361">String</span></span>                                                   | <span data-ttu-id="a52a1-362">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-362">Yes</span></span>                     | <span data-ttu-id="a52a1-363">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a52a1-363">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="a52a1-364">subjectId</span><span class="sxs-lookup"><span data-stu-id="a52a1-364">subjectId</span></span>        | <span data-ttu-id="a52a1-365">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-365">String</span></span>                                                   | <span data-ttu-id="a52a1-366">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-366">Yes</span></span>                     | <span data-ttu-id="a52a1-367">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a52a1-367">\<subjectId\></span></span> |
| <span data-ttu-id="a52a1-368">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a52a1-368">assignmentState</span></span>  | <span data-ttu-id="a52a1-369">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-369">String</span></span>                                                   | <span data-ttu-id="a52a1-370">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-370">Yes</span></span>                     | <span data-ttu-id="a52a1-371">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="a52a1-371">Eligible / Active</span></span> |
| <span data-ttu-id="a52a1-372">类型</span><span class="sxs-lookup"><span data-stu-id="a52a1-372">type</span></span>             | <span data-ttu-id="a52a1-373">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-373">String</span></span>                                                   | <span data-ttu-id="a52a1-374">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-374">Yes</span></span>                     | <span data-ttu-id="a52a1-375">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="a52a1-375">AdminUpdate</span></span> |
| <span data-ttu-id="a52a1-376">在于</span><span class="sxs-lookup"><span data-stu-id="a52a1-376">reason</span></span>           | <span data-ttu-id="a52a1-377">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-377">String</span></span>                                                   | <span data-ttu-id="a52a1-378">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="a52a1-378">depends on roleSettings</span></span> |   |
| <span data-ttu-id="a52a1-379">设定</span><span class="sxs-lookup"><span data-stu-id="a52a1-379">schedule</span></span>         | [<span data-ttu-id="a52a1-380">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a52a1-380">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a52a1-381">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-381">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="a52a1-382">请求</span><span class="sxs-lookup"><span data-stu-id="a52a1-382">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="a52a1-383">响应</span><span class="sxs-lookup"><span data-stu-id="a52a1-383">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="a52a1-384">示例 6: 管理员扩展了即将过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="a52a1-384">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="a52a1-385">此示例将用户 ANUJCUSER 的过期角色分配扩展到 API Management Service 参与者。</span><span class="sxs-lookup"><span data-stu-id="a52a1-385">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="a52a1-386">**注意:** 除了权限之外, 此示例还要求请求者在资源上至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`)。</span><span class="sxs-lookup"><span data-stu-id="a52a1-386">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="a52a1-387">属性</span><span class="sxs-lookup"><span data-stu-id="a52a1-387">Property</span></span>         | <span data-ttu-id="a52a1-388">类型</span><span class="sxs-lookup"><span data-stu-id="a52a1-388">Type</span></span>                                                     | <span data-ttu-id="a52a1-389">必需</span><span class="sxs-lookup"><span data-stu-id="a52a1-389">Required</span></span>                | <span data-ttu-id="a52a1-390">值</span><span class="sxs-lookup"><span data-stu-id="a52a1-390">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="a52a1-391">resourceId</span><span class="sxs-lookup"><span data-stu-id="a52a1-391">resourceId</span></span>       | <span data-ttu-id="a52a1-392">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-392">String</span></span>                                                   | <span data-ttu-id="a52a1-393">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-393">Yes</span></span>                     | <span data-ttu-id="a52a1-394">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a52a1-394">\<resourceId\></span></span> |
| <span data-ttu-id="a52a1-395">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a52a1-395">roleDefinitionId</span></span> | <span data-ttu-id="a52a1-396">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-396">String</span></span>                                                   | <span data-ttu-id="a52a1-397">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-397">Yes</span></span>                     | <span data-ttu-id="a52a1-398">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a52a1-398">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="a52a1-399">subjectId</span><span class="sxs-lookup"><span data-stu-id="a52a1-399">subjectId</span></span>        | <span data-ttu-id="a52a1-400">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-400">String</span></span>                                                   | <span data-ttu-id="a52a1-401">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-401">Yes</span></span>                     | <span data-ttu-id="a52a1-402">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a52a1-402">\<subjectId\></span></span> |
| <span data-ttu-id="a52a1-403">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a52a1-403">assignmentState</span></span>  | <span data-ttu-id="a52a1-404">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-404">String</span></span>                                                   | <span data-ttu-id="a52a1-405">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-405">Yes</span></span>                     | <span data-ttu-id="a52a1-406">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="a52a1-406">Eligible / Active</span></span> |
| <span data-ttu-id="a52a1-407">类型</span><span class="sxs-lookup"><span data-stu-id="a52a1-407">type</span></span>             | <span data-ttu-id="a52a1-408">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-408">String</span></span>                                                   | <span data-ttu-id="a52a1-409">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-409">Yes</span></span>                     | <span data-ttu-id="a52a1-410">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="a52a1-410">AdminExtend</span></span> |
| <span data-ttu-id="a52a1-411">在于</span><span class="sxs-lookup"><span data-stu-id="a52a1-411">reason</span></span>           | <span data-ttu-id="a52a1-412">字符串</span><span class="sxs-lookup"><span data-stu-id="a52a1-412">String</span></span>                                                   | <span data-ttu-id="a52a1-413">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="a52a1-413">depends on roleSettings</span></span> |   |
| <span data-ttu-id="a52a1-414">设定</span><span class="sxs-lookup"><span data-stu-id="a52a1-414">schedule</span></span>         | [<span data-ttu-id="a52a1-415">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a52a1-415">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="a52a1-416">是</span><span class="sxs-lookup"><span data-stu-id="a52a1-416">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="a52a1-417">请求</span><span class="sxs-lookup"><span data-stu-id="a52a1-417">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="a52a1-418">响应</span><span class="sxs-lookup"><span data-stu-id="a52a1-418">Response</span></span>

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
