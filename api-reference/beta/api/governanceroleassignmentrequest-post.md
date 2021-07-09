---
title: 创建 governanceRoleAssignmentRequest
description: 创建角色分配一个请求，以表示要处理角色分配。 下表列出了操作。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: babca9a53ad10d5b029fdbdd4119220d143b779a
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350906"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="29595-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="29595-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="29595-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29595-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29595-106">创建角色分配一个请求，以表示要处理角色分配。</span><span class="sxs-lookup"><span data-stu-id="29595-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="29595-107">下表列出了操作。</span><span class="sxs-lookup"><span data-stu-id="29595-107">The following table lists the operations.</span></span>

| <span data-ttu-id="29595-108">Operation</span><span class="sxs-lookup"><span data-stu-id="29595-108">Operation</span></span>                                   | <span data-ttu-id="29595-109">类型</span><span class="sxs-lookup"><span data-stu-id="29595-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="29595-110">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="29595-110">Assign a role assignment</span></span>                    | <span data-ttu-id="29595-111">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="29595-111">AdminAdd</span></span>    |
| <span data-ttu-id="29595-112">激活符合条件的角色分配</span><span class="sxs-lookup"><span data-stu-id="29595-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="29595-113">UserAdd</span><span class="sxs-lookup"><span data-stu-id="29595-113">UserAdd</span></span>     |
| <span data-ttu-id="29595-114">停用已激活角色分配</span><span class="sxs-lookup"><span data-stu-id="29595-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="29595-115">UserRemove</span><span class="sxs-lookup"><span data-stu-id="29595-115">UserRemove</span></span>  |
| <span data-ttu-id="29595-116">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="29595-116">Remove a role assignment</span></span>                    | <span data-ttu-id="29595-117">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="29595-117">AdminRemove</span></span> |
| <span data-ttu-id="29595-118">更新角色分配</span><span class="sxs-lookup"><span data-stu-id="29595-118">Update a role assignment</span></span>                    | <span data-ttu-id="29595-119">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="29595-119">AdminUpdate</span></span> |
| <span data-ttu-id="29595-120">请求扩展我的角色分配</span><span class="sxs-lookup"><span data-stu-id="29595-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="29595-121">UserExtend</span><span class="sxs-lookup"><span data-stu-id="29595-121">UserExtend</span></span>  |
| <span data-ttu-id="29595-122">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="29595-122">Extend a role assignment</span></span>                    | <span data-ttu-id="29595-123">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="29595-123">AdminExtend</span></span> |
| <span data-ttu-id="29595-124">请求续订已过期角色分配</span><span class="sxs-lookup"><span data-stu-id="29595-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="29595-125">UserRenew</span><span class="sxs-lookup"><span data-stu-id="29595-125">UserRenew</span></span>   |
| <span data-ttu-id="29595-126">续订过期角色分配</span><span class="sxs-lookup"><span data-stu-id="29595-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="29595-127">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="29595-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="29595-128">权限</span><span class="sxs-lookup"><span data-stu-id="29595-128">Permissions</span></span>

<span data-ttu-id="29595-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="29595-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="29595-131">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="29595-131">Azure resources</span></span>

| <span data-ttu-id="29595-132">权限类型</span><span class="sxs-lookup"><span data-stu-id="29595-132">Permission type</span></span> | <span data-ttu-id="29595-133">权限</span><span class="sxs-lookup"><span data-stu-id="29595-133">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="29595-134">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29595-134">Delegated (work or school account)</span></span> | <span data-ttu-id="29595-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="29595-135">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="29595-136">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29595-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29595-137">不支持。</span><span class="sxs-lookup"><span data-stu-id="29595-137">Not supported.</span></span> |
| <span data-ttu-id="29595-138">Application</span><span class="sxs-lookup"><span data-stu-id="29595-138">Application</span></span> | <span data-ttu-id="29595-139">不支持。</span><span class="sxs-lookup"><span data-stu-id="29595-139">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="29595-140">Azure AD</span><span class="sxs-lookup"><span data-stu-id="29595-140">Azure AD</span></span>

| <span data-ttu-id="29595-141">权限类型</span><span class="sxs-lookup"><span data-stu-id="29595-141">Permission type</span></span> | <span data-ttu-id="29595-142">权限</span><span class="sxs-lookup"><span data-stu-id="29595-142">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="29595-143">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29595-143">Delegated (work or school account)</span></span> | <span data-ttu-id="29595-144">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="29595-144">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="29595-145">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29595-145">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29595-146">不支持。</span><span class="sxs-lookup"><span data-stu-id="29595-146">Not supported.</span></span> |
| <span data-ttu-id="29595-147">Application</span><span class="sxs-lookup"><span data-stu-id="29595-147">Application</span></span> | <span data-ttu-id="29595-148">不支持。</span><span class="sxs-lookup"><span data-stu-id="29595-148">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="29595-149">组</span><span class="sxs-lookup"><span data-stu-id="29595-149">Groups</span></span>

|<span data-ttu-id="29595-150">权限类型</span><span class="sxs-lookup"><span data-stu-id="29595-150">Permission type</span></span> | <span data-ttu-id="29595-151">权限</span><span class="sxs-lookup"><span data-stu-id="29595-151">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="29595-152">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29595-152">Delegated (work or school account)</span></span> | <span data-ttu-id="29595-153">PrivilegedAccess.ReadWrite.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="29595-153">PrivilegedAccess.ReadWrite.AzureADGroup</span></span> |
| <span data-ttu-id="29595-154">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29595-154">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29595-155">不支持。</span><span class="sxs-lookup"><span data-stu-id="29595-155">Not supported.</span></span> |
| <span data-ttu-id="29595-156">Application</span><span class="sxs-lookup"><span data-stu-id="29595-156">Application</span></span> | <span data-ttu-id="29595-157">不支持。</span><span class="sxs-lookup"><span data-stu-id="29595-157">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="29595-158">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29595-158">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="29595-159">请求标头</span><span class="sxs-lookup"><span data-stu-id="29595-159">Request headers</span></span>

| <span data-ttu-id="29595-160">名称</span><span class="sxs-lookup"><span data-stu-id="29595-160">Name</span></span>          | <span data-ttu-id="29595-161">说明</span><span class="sxs-lookup"><span data-stu-id="29595-161">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="29595-162">Authorization</span><span class="sxs-lookup"><span data-stu-id="29595-162">Authorization</span></span> | <span data-ttu-id="29595-163">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="29595-163">Bearer {code}</span></span>    |
| <span data-ttu-id="29595-164">Content-type</span><span class="sxs-lookup"><span data-stu-id="29595-164">Content-type</span></span>  | <span data-ttu-id="29595-165">application/json</span><span class="sxs-lookup"><span data-stu-id="29595-165">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="29595-166">请求正文</span><span class="sxs-lookup"><span data-stu-id="29595-166">Request body</span></span>

<span data-ttu-id="29595-167">在请求正文中，提供 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29595-167">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="29595-168">属性</span><span class="sxs-lookup"><span data-stu-id="29595-168">Property</span></span>         | <span data-ttu-id="29595-169">类型</span><span class="sxs-lookup"><span data-stu-id="29595-169">Type</span></span>                                                     | <span data-ttu-id="29595-170">说明</span><span class="sxs-lookup"><span data-stu-id="29595-170">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="29595-171">resourceId</span><span class="sxs-lookup"><span data-stu-id="29595-171">resourceId</span></span>       | <span data-ttu-id="29595-172">String</span><span class="sxs-lookup"><span data-stu-id="29595-172">String</span></span>                                                   | <span data-ttu-id="29595-173">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="29595-173">The ID of the resource.</span></span> <span data-ttu-id="29595-174">必填。</span><span class="sxs-lookup"><span data-stu-id="29595-174">Required.</span></span> |
| <span data-ttu-id="29595-175">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="29595-175">roleDefinitionId</span></span> | <span data-ttu-id="29595-176">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-176">String</span></span>                                                   | <span data-ttu-id="29595-177">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="29595-177">The ID of the role definition.</span></span> <span data-ttu-id="29595-178">必填。</span><span class="sxs-lookup"><span data-stu-id="29595-178">Required.</span></span> |
| <span data-ttu-id="29595-179">subjectId</span><span class="sxs-lookup"><span data-stu-id="29595-179">subjectId</span></span>        | <span data-ttu-id="29595-180">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-180">String</span></span>                                                   | <span data-ttu-id="29595-181">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="29595-181">The ID of the subject.</span></span> <span data-ttu-id="29595-182">必填。</span><span class="sxs-lookup"><span data-stu-id="29595-182">Required.</span></span> |
| <span data-ttu-id="29595-183">assignmentState</span><span class="sxs-lookup"><span data-stu-id="29595-183">assignmentState</span></span>  | <span data-ttu-id="29595-184">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-184">String</span></span>                                                   | <span data-ttu-id="29595-185">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="29595-185">The state of assignment.</span></span> <span data-ttu-id="29595-186">值可以是 和 `Eligible` `Active` 。</span><span class="sxs-lookup"><span data-stu-id="29595-186">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="29595-187">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="29595-187">Required.</span></span> |
| <span data-ttu-id="29595-188">type</span><span class="sxs-lookup"><span data-stu-id="29595-188">type</span></span>             | <span data-ttu-id="29595-189">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-189">String</span></span>                                                   | <span data-ttu-id="29595-190">请求类型。</span><span class="sxs-lookup"><span data-stu-id="29595-190">The request type.</span></span> <span data-ttu-id="29595-191">值可以是 `AdminAdd` `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` 、、、、、 `UserExtend` `UserRenew` 和 `AdminRenew` `AdminExtend` 。</span><span class="sxs-lookup"><span data-stu-id="29595-191">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="29595-192">必填。</span><span class="sxs-lookup"><span data-stu-id="29595-192">Required.</span></span> |
| <span data-ttu-id="29595-193">reason</span><span class="sxs-lookup"><span data-stu-id="29595-193">reason</span></span>           | <span data-ttu-id="29595-194">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-194">String</span></span>                                                   | <span data-ttu-id="29595-195">需要为请求审核和审核角色分配提供原因。</span><span class="sxs-lookup"><span data-stu-id="29595-195">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="29595-196">schedule</span><span class="sxs-lookup"><span data-stu-id="29595-196">schedule</span></span>         | [<span data-ttu-id="29595-197">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="29595-197">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="29595-198">请求角色分配计划。</span><span class="sxs-lookup"><span data-stu-id="29595-198">The schedule of the role assignment request.</span></span> <span data-ttu-id="29595-199">对于 、 `UserAdd` `AdminAdd` 、 `AdminUpdate` 和 `AdminExtend` 的请求类型，是必需的。</span><span class="sxs-lookup"><span data-stu-id="29595-199">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="29595-200">响应</span><span class="sxs-lookup"><span data-stu-id="29595-200">Response</span></span>

<span data-ttu-id="29595-201">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="29595-201">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="29595-202">错误代码</span><span class="sxs-lookup"><span data-stu-id="29595-202">Error codes</span></span>

<span data-ttu-id="29595-203">此 API 返回标准 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="29595-203">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="29595-204">此外，它还返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="29595-204">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="29595-205">错误代码</span><span class="sxs-lookup"><span data-stu-id="29595-205">Error code</span></span>     | <span data-ttu-id="29595-206">错误消息</span><span class="sxs-lookup"><span data-stu-id="29595-206">Error message</span></span>                               | <span data-ttu-id="29595-207">详细信息</span><span class="sxs-lookup"><span data-stu-id="29595-207">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="29595-208">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="29595-208">400 BadRequest</span></span> | <span data-ttu-id="29595-209">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="29595-209">RoleNotFound</span></span>                                | <span data-ttu-id="29595-210">`roleDefinitionId`找不到请求正文中提供的 。</span><span class="sxs-lookup"><span data-stu-id="29595-210">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="29595-211">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="29595-211">400 BadRequest</span></span> | <span data-ttu-id="29595-212">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="29595-212">ResourceIsLocked</span></span>                            | <span data-ttu-id="29595-213">请求正文中提供的资源的状态为 ， `Locked` 无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="29595-213">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="29595-214">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="29595-214">400 BadRequest</span></span> | <span data-ttu-id="29595-215">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="29595-215">SubjectNotFound</span></span>                             | <span data-ttu-id="29595-216">`subjectId`找不到请求正文中提供的 。</span><span class="sxs-lookup"><span data-stu-id="29595-216">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="29595-217">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="29595-217">400 BadRequest</span></span> | <span data-ttu-id="29595-218">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="29595-218">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="29595-219">系统中已存在待定[governanceRoleAssignmentRequest。](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="29595-219">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="29595-220">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="29595-220">400 BadRequest</span></span> | <span data-ttu-id="29595-221">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="29595-221">RoleAssignmentExists</span></span>                        | <span data-ttu-id="29595-222">系统中已存在请求创建的[governanceRoleAssignment。](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="29595-222">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="29595-223">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="29595-223">400 BadRequest</span></span> | <span data-ttu-id="29595-224">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="29595-224">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="29595-225">系统中不存在请求更新/扩展的[governanceRoleAssignment。](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="29595-225">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="29595-226">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="29595-226">400 BadRequest</span></span> | <span data-ttu-id="29595-227">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="29595-227">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="29595-228">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部策略，无法创建。</span><span class="sxs-lookup"><span data-stu-id="29595-228">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="29595-229">示例</span><span class="sxs-lookup"><span data-stu-id="29595-229">Examples</span></span>

<span data-ttu-id="29595-230">以下示例显示如何使用此 API。</span><span class="sxs-lookup"><span data-stu-id="29595-230">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="29595-231">示例 1：管理员将用户分配给角色</span><span class="sxs-lookup"><span data-stu-id="29595-231">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="29595-232">本示例中，管理员将 nawu@contoso.com 分配给"计费读取者"角色。</span><span class="sxs-lookup"><span data-stu-id="29595-232">In this example, an administrator assigns user nawu@contoso.com to the Billing Reader role.</span></span>

 ><span data-ttu-id="29595-233">**注意：** 除了权限之外，此示例还要求请求者至少具有一个管理员角色分配 (`Active` `owner` 或) `user access administrator` 资源。</span><span class="sxs-lookup"><span data-stu-id="29595-233">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="29595-234">属性</span><span class="sxs-lookup"><span data-stu-id="29595-234">Property</span></span>         | <span data-ttu-id="29595-235">类型</span><span class="sxs-lookup"><span data-stu-id="29595-235">Type</span></span>                                                     | <span data-ttu-id="29595-236">必需</span><span class="sxs-lookup"><span data-stu-id="29595-236">Required</span></span>                 | <span data-ttu-id="29595-237">值</span><span class="sxs-lookup"><span data-stu-id="29595-237">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="29595-238">resourceId</span><span class="sxs-lookup"><span data-stu-id="29595-238">resourceId</span></span>       | <span data-ttu-id="29595-239">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-239">String</span></span>                                                   | <span data-ttu-id="29595-240">是</span><span class="sxs-lookup"><span data-stu-id="29595-240">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="29595-241">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="29595-241">roleDefinitionId</span></span> | <span data-ttu-id="29595-242">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-242">String</span></span>                                                   | <span data-ttu-id="29595-243">是</span><span class="sxs-lookup"><span data-stu-id="29595-243">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="29595-244">subjectId</span><span class="sxs-lookup"><span data-stu-id="29595-244">subjectId</span></span>        | <span data-ttu-id="29595-245">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-245">String</span></span>                                                   | <span data-ttu-id="29595-246">是</span><span class="sxs-lookup"><span data-stu-id="29595-246">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="29595-247">assignmentState</span><span class="sxs-lookup"><span data-stu-id="29595-247">assignmentState</span></span>  | <span data-ttu-id="29595-248">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-248">String</span></span>                                                   | <span data-ttu-id="29595-249">是</span><span class="sxs-lookup"><span data-stu-id="29595-249">Yes</span></span>                      | <span data-ttu-id="29595-250">符合条件的/活动的</span><span class="sxs-lookup"><span data-stu-id="29595-250">Eligible / Active</span></span> |
| <span data-ttu-id="29595-251">type</span><span class="sxs-lookup"><span data-stu-id="29595-251">type</span></span>             | <span data-ttu-id="29595-252">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-252">String</span></span>                                                   | <span data-ttu-id="29595-253">是</span><span class="sxs-lookup"><span data-stu-id="29595-253">Yes</span></span>                      | <span data-ttu-id="29595-254">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="29595-254">AdminAdd</span></span> |
| <span data-ttu-id="29595-255">reason</span><span class="sxs-lookup"><span data-stu-id="29595-255">reason</span></span>           | <span data-ttu-id="29595-256">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-256">String</span></span>                                                   | <span data-ttu-id="29595-257">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="29595-257">depends on role Settings</span></span> |   |
| <span data-ttu-id="29595-258">schedule</span><span class="sxs-lookup"><span data-stu-id="29595-258">schedule</span></span>         | [<span data-ttu-id="29595-259">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="29595-259">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="29595-260">是</span><span class="sxs-lookup"><span data-stu-id="29595-260">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="29595-261">请求</span><span class="sxs-lookup"><span data-stu-id="29595-261">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="29595-262">HTTP</span><span class="sxs-lookup"><span data-stu-id="29595-262">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post_1"
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
# <a name="c"></a>[<span data-ttu-id="29595-263">C#</span><span class="sxs-lookup"><span data-stu-id="29595-263">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29595-264">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29595-264">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29595-265">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29595-265">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29595-266">Java</span><span class="sxs-lookup"><span data-stu-id="29595-266">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="29595-267">响应</span><span class="sxs-lookup"><span data-stu-id="29595-267">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="29595-268">示例 2：用户激活符合条件的角色</span><span class="sxs-lookup"><span data-stu-id="29595-268">Example 2: User activates eligible role</span></span>

<span data-ttu-id="29595-269">本示例中，用户 nawu@contoso.com 激活符合条件的计费读取者角色。</span><span class="sxs-lookup"><span data-stu-id="29595-269">In this example, the user nawu@contoso.com activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="29595-270">属性</span><span class="sxs-lookup"><span data-stu-id="29595-270">Property</span></span>         | <span data-ttu-id="29595-271">类型</span><span class="sxs-lookup"><span data-stu-id="29595-271">Type</span></span>                                                     | <span data-ttu-id="29595-272">必需</span><span class="sxs-lookup"><span data-stu-id="29595-272">Required</span></span>                 | <span data-ttu-id="29595-273">值</span><span class="sxs-lookup"><span data-stu-id="29595-273">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="29595-274">resourceId</span><span class="sxs-lookup"><span data-stu-id="29595-274">resourceId</span></span>       | <span data-ttu-id="29595-275">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-275">String</span></span>                                                   | <span data-ttu-id="29595-276">是</span><span class="sxs-lookup"><span data-stu-id="29595-276">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="29595-277">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="29595-277">roleDefinitionId</span></span> | <span data-ttu-id="29595-278">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-278">String</span></span>                                                   | <span data-ttu-id="29595-279">是</span><span class="sxs-lookup"><span data-stu-id="29595-279">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="29595-280">subjectId</span><span class="sxs-lookup"><span data-stu-id="29595-280">subjectId</span></span>        | <span data-ttu-id="29595-281">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-281">String</span></span>                                                   | <span data-ttu-id="29595-282">是</span><span class="sxs-lookup"><span data-stu-id="29595-282">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="29595-283">assignmentState</span><span class="sxs-lookup"><span data-stu-id="29595-283">assignmentState</span></span>  | <span data-ttu-id="29595-284">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-284">String</span></span>                                                   | <span data-ttu-id="29595-285">是</span><span class="sxs-lookup"><span data-stu-id="29595-285">Yes</span></span>                      | <span data-ttu-id="29595-286">活动</span><span class="sxs-lookup"><span data-stu-id="29595-286">Active</span></span> |
| <span data-ttu-id="29595-287">type</span><span class="sxs-lookup"><span data-stu-id="29595-287">type</span></span>             | <span data-ttu-id="29595-288">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-288">String</span></span>                                                   | <span data-ttu-id="29595-289">是</span><span class="sxs-lookup"><span data-stu-id="29595-289">Yes</span></span>                      | <span data-ttu-id="29595-290">UserAdd</span><span class="sxs-lookup"><span data-stu-id="29595-290">UserAdd</span></span> |
| <span data-ttu-id="29595-291">reason</span><span class="sxs-lookup"><span data-stu-id="29595-291">reason</span></span>           | <span data-ttu-id="29595-292">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-292">String</span></span>                                                   | <span data-ttu-id="29595-293">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="29595-293">depends on role Settings</span></span> |   |
| <span data-ttu-id="29595-294">schedule</span><span class="sxs-lookup"><span data-stu-id="29595-294">schedule</span></span>         | [<span data-ttu-id="29595-295">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="29595-295">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="29595-296">是</span><span class="sxs-lookup"><span data-stu-id="29595-296">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="29595-297">请求</span><span class="sxs-lookup"><span data-stu-id="29595-297">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="29595-298">HTTP</span><span class="sxs-lookup"><span data-stu-id="29595-298">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post_2"
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
# <a name="c"></a>[<span data-ttu-id="29595-299">C#</span><span class="sxs-lookup"><span data-stu-id="29595-299">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29595-300">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29595-300">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29595-301">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29595-301">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29595-302">Java</span><span class="sxs-lookup"><span data-stu-id="29595-302">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="29595-303">响应</span><span class="sxs-lookup"><span data-stu-id="29595-303">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="29595-304">示例 3：用户停用分配的角色</span><span class="sxs-lookup"><span data-stu-id="29595-304">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="29595-305">本示例中，用户 nawu@contoso.com 活动"计费读取者"角色。</span><span class="sxs-lookup"><span data-stu-id="29595-305">In this example, the user nawu@contoso.com deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="29595-306">属性</span><span class="sxs-lookup"><span data-stu-id="29595-306">Property</span></span>         | <span data-ttu-id="29595-307">类型</span><span class="sxs-lookup"><span data-stu-id="29595-307">Type</span></span>                                                     | <span data-ttu-id="29595-308">必需</span><span class="sxs-lookup"><span data-stu-id="29595-308">Required</span></span> | <span data-ttu-id="29595-309">值</span><span class="sxs-lookup"><span data-stu-id="29595-309">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="29595-310">resourceId</span><span class="sxs-lookup"><span data-stu-id="29595-310">resourceId</span></span>       | <span data-ttu-id="29595-311">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-311">String</span></span>                                                   | <span data-ttu-id="29595-312">是</span><span class="sxs-lookup"><span data-stu-id="29595-312">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="29595-313">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="29595-313">roleDefinitionId</span></span> | <span data-ttu-id="29595-314">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-314">String</span></span>                                                   | <span data-ttu-id="29595-315">是</span><span class="sxs-lookup"><span data-stu-id="29595-315">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="29595-316">subjectId</span><span class="sxs-lookup"><span data-stu-id="29595-316">subjectId</span></span>        | <span data-ttu-id="29595-317">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-317">String</span></span>                                                   | <span data-ttu-id="29595-318">是</span><span class="sxs-lookup"><span data-stu-id="29595-318">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="29595-319">assignmentState</span><span class="sxs-lookup"><span data-stu-id="29595-319">assignmentState</span></span>  | <span data-ttu-id="29595-320">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-320">String</span></span>                                                   | <span data-ttu-id="29595-321">是</span><span class="sxs-lookup"><span data-stu-id="29595-321">Yes</span></span>      | <span data-ttu-id="29595-322">活动</span><span class="sxs-lookup"><span data-stu-id="29595-322">Active</span></span> |
| <span data-ttu-id="29595-323">type</span><span class="sxs-lookup"><span data-stu-id="29595-323">type</span></span>             | <span data-ttu-id="29595-324">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-324">String</span></span>                                                   | <span data-ttu-id="29595-325">是</span><span class="sxs-lookup"><span data-stu-id="29595-325">Yes</span></span>      | <span data-ttu-id="29595-326">UserRemove</span><span class="sxs-lookup"><span data-stu-id="29595-326">UserRemove</span></span> |
| <span data-ttu-id="29595-327">reason</span><span class="sxs-lookup"><span data-stu-id="29595-327">reason</span></span>           | <span data-ttu-id="29595-328">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-328">String</span></span>                                                   | <span data-ttu-id="29595-329">否</span><span class="sxs-lookup"><span data-stu-id="29595-329">No</span></span>       |   |
| <span data-ttu-id="29595-330">schedule</span><span class="sxs-lookup"><span data-stu-id="29595-330">schedule</span></span>         | [<span data-ttu-id="29595-331">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="29595-331">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="29595-332">否</span><span class="sxs-lookup"><span data-stu-id="29595-332">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="29595-333">请求</span><span class="sxs-lookup"><span data-stu-id="29595-333">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="29595-334">HTTP</span><span class="sxs-lookup"><span data-stu-id="29595-334">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post_3"
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
# <a name="c"></a>[<span data-ttu-id="29595-335">C#</span><span class="sxs-lookup"><span data-stu-id="29595-335">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29595-336">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29595-336">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29595-337">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29595-337">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29595-338">Java</span><span class="sxs-lookup"><span data-stu-id="29595-338">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="29595-339">响应</span><span class="sxs-lookup"><span data-stu-id="29595-339">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="29595-340">示例 4：管理员从角色中删除用户</span><span class="sxs-lookup"><span data-stu-id="29595-340">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="29595-341">本示例中，管理员从计费读取 nawu@contoso.com 中删除用户角色。</span><span class="sxs-lookup"><span data-stu-id="29595-341">In this example, an administrator removes the user nawu@contoso.com from the Billing Reader role.</span></span>

 ><span data-ttu-id="29595-342">**注意：** 除了权限之外，此示例还要求请求者至少具有一个管理员角色分配 (`Active` `owner` 或) `user access administrator` 资源。</span><span class="sxs-lookup"><span data-stu-id="29595-342">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="29595-343">属性</span><span class="sxs-lookup"><span data-stu-id="29595-343">Property</span></span>         | <span data-ttu-id="29595-344">类型</span><span class="sxs-lookup"><span data-stu-id="29595-344">Type</span></span>                                                     | <span data-ttu-id="29595-345">必需</span><span class="sxs-lookup"><span data-stu-id="29595-345">Required</span></span> | <span data-ttu-id="29595-346">值</span><span class="sxs-lookup"><span data-stu-id="29595-346">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="29595-347">resourceId</span><span class="sxs-lookup"><span data-stu-id="29595-347">resourceId</span></span>       | <span data-ttu-id="29595-348">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-348">String</span></span>                                                   | <span data-ttu-id="29595-349">是</span><span class="sxs-lookup"><span data-stu-id="29595-349">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="29595-350">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="29595-350">roleDefinitionId</span></span> | <span data-ttu-id="29595-351">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-351">String</span></span>                                                   | <span data-ttu-id="29595-352">是</span><span class="sxs-lookup"><span data-stu-id="29595-352">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="29595-353">subjectId</span><span class="sxs-lookup"><span data-stu-id="29595-353">subjectId</span></span>        | <span data-ttu-id="29595-354">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-354">String</span></span>                                                   | <span data-ttu-id="29595-355">是</span><span class="sxs-lookup"><span data-stu-id="29595-355">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="29595-356">assignmentState</span><span class="sxs-lookup"><span data-stu-id="29595-356">assignmentState</span></span>  | <span data-ttu-id="29595-357">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-357">String</span></span>                                                   | <span data-ttu-id="29595-358">是</span><span class="sxs-lookup"><span data-stu-id="29595-358">Yes</span></span>      | <span data-ttu-id="29595-359">符合条件的/活动的</span><span class="sxs-lookup"><span data-stu-id="29595-359">Eligible / Active</span></span> |
| <span data-ttu-id="29595-360">type</span><span class="sxs-lookup"><span data-stu-id="29595-360">type</span></span>             | <span data-ttu-id="29595-361">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-361">String</span></span>                                                   | <span data-ttu-id="29595-362">是</span><span class="sxs-lookup"><span data-stu-id="29595-362">Yes</span></span>      | <span data-ttu-id="29595-363">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="29595-363">AdminRemove</span></span> |
| <span data-ttu-id="29595-364">reason</span><span class="sxs-lookup"><span data-stu-id="29595-364">reason</span></span>           | <span data-ttu-id="29595-365">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-365">String</span></span>                                                   | <span data-ttu-id="29595-366">否</span><span class="sxs-lookup"><span data-stu-id="29595-366">No</span></span>       |   |
| <span data-ttu-id="29595-367">schedule</span><span class="sxs-lookup"><span data-stu-id="29595-367">schedule</span></span>         | [<span data-ttu-id="29595-368">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="29595-368">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="29595-369">否</span><span class="sxs-lookup"><span data-stu-id="29595-369">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="29595-370">请求</span><span class="sxs-lookup"><span data-stu-id="29595-370">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="29595-371">HTTP</span><span class="sxs-lookup"><span data-stu-id="29595-371">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post_4"
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
# <a name="c"></a>[<span data-ttu-id="29595-372">C#</span><span class="sxs-lookup"><span data-stu-id="29595-372">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29595-373">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29595-373">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29595-374">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29595-374">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29595-375">Java</span><span class="sxs-lookup"><span data-stu-id="29595-375">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="29595-376">响应</span><span class="sxs-lookup"><span data-stu-id="29595-376">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="29595-377">示例 5：管理员更新角色分配</span><span class="sxs-lookup"><span data-stu-id="29595-377">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="29595-378">本示例中，管理员更新角色分配所有者 nawu@contoso.com 权限。</span><span class="sxs-lookup"><span data-stu-id="29595-378">In this example, administrators update the role assignment for the user nawu@contoso.com to Owner.</span></span>

 ><span data-ttu-id="29595-379">**注意：** 除了权限之外，此示例还要求请求者至少具有一个管理员角色分配 (`Active` `owner` 或) `user access administrator` 资源。</span><span class="sxs-lookup"><span data-stu-id="29595-379">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="29595-380">属性</span><span class="sxs-lookup"><span data-stu-id="29595-380">Property</span></span>         | <span data-ttu-id="29595-381">类型</span><span class="sxs-lookup"><span data-stu-id="29595-381">Type</span></span>                                                     | <span data-ttu-id="29595-382">必需</span><span class="sxs-lookup"><span data-stu-id="29595-382">Required</span></span>                | <span data-ttu-id="29595-383">值</span><span class="sxs-lookup"><span data-stu-id="29595-383">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="29595-384">resourceId</span><span class="sxs-lookup"><span data-stu-id="29595-384">resourceId</span></span>       | <span data-ttu-id="29595-385">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-385">String</span></span>                                                   | <span data-ttu-id="29595-386">是</span><span class="sxs-lookup"><span data-stu-id="29595-386">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="29595-387">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="29595-387">roleDefinitionId</span></span> | <span data-ttu-id="29595-388">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-388">String</span></span>                                                   | <span data-ttu-id="29595-389">是</span><span class="sxs-lookup"><span data-stu-id="29595-389">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="29595-390">subjectId</span><span class="sxs-lookup"><span data-stu-id="29595-390">subjectId</span></span>        | <span data-ttu-id="29595-391">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-391">String</span></span>                                                   | <span data-ttu-id="29595-392">是</span><span class="sxs-lookup"><span data-stu-id="29595-392">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="29595-393">assignmentState</span><span class="sxs-lookup"><span data-stu-id="29595-393">assignmentState</span></span>  | <span data-ttu-id="29595-394">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-394">String</span></span>                                                   | <span data-ttu-id="29595-395">是</span><span class="sxs-lookup"><span data-stu-id="29595-395">Yes</span></span>                     | <span data-ttu-id="29595-396">符合条件的/活动的</span><span class="sxs-lookup"><span data-stu-id="29595-396">Eligible / Active</span></span> |
| <span data-ttu-id="29595-397">type</span><span class="sxs-lookup"><span data-stu-id="29595-397">type</span></span>             | <span data-ttu-id="29595-398">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-398">String</span></span>                                                   | <span data-ttu-id="29595-399">是</span><span class="sxs-lookup"><span data-stu-id="29595-399">Yes</span></span>                     | <span data-ttu-id="29595-400">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="29595-400">AdminUpdate</span></span> |
| <span data-ttu-id="29595-401">reason</span><span class="sxs-lookup"><span data-stu-id="29595-401">reason</span></span>           | <span data-ttu-id="29595-402">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-402">String</span></span>                                                   | <span data-ttu-id="29595-403">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="29595-403">depends on roleSettings</span></span> |   |
| <span data-ttu-id="29595-404">schedule</span><span class="sxs-lookup"><span data-stu-id="29595-404">schedule</span></span>         | [<span data-ttu-id="29595-405">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="29595-405">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="29595-406">是</span><span class="sxs-lookup"><span data-stu-id="29595-406">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="29595-407">请求</span><span class="sxs-lookup"><span data-stu-id="29595-407">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="29595-408">HTTP</span><span class="sxs-lookup"><span data-stu-id="29595-408">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post_5"
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
# <a name="c"></a>[<span data-ttu-id="29595-409">C#</span><span class="sxs-lookup"><span data-stu-id="29595-409">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29595-410">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29595-410">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29595-411">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29595-411">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29595-412">Java</span><span class="sxs-lookup"><span data-stu-id="29595-412">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="29595-413">响应</span><span class="sxs-lookup"><span data-stu-id="29595-413">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="29595-414">示例 6：管理员扩展过期角色分配</span><span class="sxs-lookup"><span data-stu-id="29595-414">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="29595-415">此示例将用户 ANUJCUSER 角色分配 API 管理服务参与者的到期日期。</span><span class="sxs-lookup"><span data-stu-id="29595-415">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="29595-416">**注意：** 除了权限之外，此示例还要求请求者至少具有一个管理员角色分配 (`Active` `owner` 或) `user access administrator` 资源。</span><span class="sxs-lookup"><span data-stu-id="29595-416">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="29595-417">属性</span><span class="sxs-lookup"><span data-stu-id="29595-417">Property</span></span>         | <span data-ttu-id="29595-418">类型</span><span class="sxs-lookup"><span data-stu-id="29595-418">Type</span></span>                                                     | <span data-ttu-id="29595-419">必需</span><span class="sxs-lookup"><span data-stu-id="29595-419">Required</span></span>                | <span data-ttu-id="29595-420">值</span><span class="sxs-lookup"><span data-stu-id="29595-420">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="29595-421">resourceId</span><span class="sxs-lookup"><span data-stu-id="29595-421">resourceId</span></span>       | <span data-ttu-id="29595-422">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-422">String</span></span>                                                   | <span data-ttu-id="29595-423">是</span><span class="sxs-lookup"><span data-stu-id="29595-423">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="29595-424">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="29595-424">roleDefinitionId</span></span> | <span data-ttu-id="29595-425">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-425">String</span></span>                                                   | <span data-ttu-id="29595-426">是</span><span class="sxs-lookup"><span data-stu-id="29595-426">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="29595-427">subjectId</span><span class="sxs-lookup"><span data-stu-id="29595-427">subjectId</span></span>        | <span data-ttu-id="29595-428">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-428">String</span></span>                                                   | <span data-ttu-id="29595-429">是</span><span class="sxs-lookup"><span data-stu-id="29595-429">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="29595-430">assignmentState</span><span class="sxs-lookup"><span data-stu-id="29595-430">assignmentState</span></span>  | <span data-ttu-id="29595-431">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-431">String</span></span>                                                   | <span data-ttu-id="29595-432">是</span><span class="sxs-lookup"><span data-stu-id="29595-432">Yes</span></span>                     | <span data-ttu-id="29595-433">符合条件的/活动的</span><span class="sxs-lookup"><span data-stu-id="29595-433">Eligible / Active</span></span> |
| <span data-ttu-id="29595-434">type</span><span class="sxs-lookup"><span data-stu-id="29595-434">type</span></span>             | <span data-ttu-id="29595-435">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-435">String</span></span>                                                   | <span data-ttu-id="29595-436">是</span><span class="sxs-lookup"><span data-stu-id="29595-436">Yes</span></span>                     | <span data-ttu-id="29595-437">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="29595-437">AdminExtend</span></span> |
| <span data-ttu-id="29595-438">reason</span><span class="sxs-lookup"><span data-stu-id="29595-438">reason</span></span>           | <span data-ttu-id="29595-439">字符串</span><span class="sxs-lookup"><span data-stu-id="29595-439">String</span></span>                                                   | <span data-ttu-id="29595-440">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="29595-440">depends on roleSettings</span></span> |   |
| <span data-ttu-id="29595-441">schedule</span><span class="sxs-lookup"><span data-stu-id="29595-441">schedule</span></span>         | [<span data-ttu-id="29595-442">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="29595-442">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="29595-443">是</span><span class="sxs-lookup"><span data-stu-id="29595-443">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="29595-444">请求</span><span class="sxs-lookup"><span data-stu-id="29595-444">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="29595-445">HTTP</span><span class="sxs-lookup"><span data-stu-id="29595-445">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post_6"
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
# <a name="c"></a>[<span data-ttu-id="29595-446">C#</span><span class="sxs-lookup"><span data-stu-id="29595-446">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-6-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29595-447">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29595-447">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-6-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29595-448">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29595-448">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-6-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29595-449">Java</span><span class="sxs-lookup"><span data-stu-id="29595-449">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-6-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="29595-450">响应</span><span class="sxs-lookup"><span data-stu-id="29595-450">Response</span></span>

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


