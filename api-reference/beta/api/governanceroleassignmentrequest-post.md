---
title: 创建 governanceRoleAssignmentRequest
description: 创建角色分配一个请求，以表示要处理角色分配。 下表列出了操作。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 4883fedc71cfdcc6c50ab87b46299fdb173552a5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950775"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="7748c-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="7748c-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="7748c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7748c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7748c-106">创建角色分配一个请求，以表示要处理角色分配。</span><span class="sxs-lookup"><span data-stu-id="7748c-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="7748c-107">下表列出了操作。</span><span class="sxs-lookup"><span data-stu-id="7748c-107">The following table lists the operations.</span></span>

| <span data-ttu-id="7748c-108">Operation</span><span class="sxs-lookup"><span data-stu-id="7748c-108">Operation</span></span>                                   | <span data-ttu-id="7748c-109">类型</span><span class="sxs-lookup"><span data-stu-id="7748c-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="7748c-110">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="7748c-110">Assign a role assignment</span></span>                    | <span data-ttu-id="7748c-111">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="7748c-111">AdminAdd</span></span>    |
| <span data-ttu-id="7748c-112">激活符合条件的角色分配</span><span class="sxs-lookup"><span data-stu-id="7748c-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="7748c-113">UserAdd</span><span class="sxs-lookup"><span data-stu-id="7748c-113">UserAdd</span></span>     |
| <span data-ttu-id="7748c-114">停用已激活角色分配</span><span class="sxs-lookup"><span data-stu-id="7748c-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="7748c-115">UserRemove</span><span class="sxs-lookup"><span data-stu-id="7748c-115">UserRemove</span></span>  |
| <span data-ttu-id="7748c-116">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="7748c-116">Remove a role assignment</span></span>                    | <span data-ttu-id="7748c-117">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="7748c-117">AdminRemove</span></span> |
| <span data-ttu-id="7748c-118">更新角色分配</span><span class="sxs-lookup"><span data-stu-id="7748c-118">Update a role assignment</span></span>                    | <span data-ttu-id="7748c-119">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="7748c-119">AdminUpdate</span></span> |
| <span data-ttu-id="7748c-120">请求扩展我的角色分配</span><span class="sxs-lookup"><span data-stu-id="7748c-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="7748c-121">UserExtend</span><span class="sxs-lookup"><span data-stu-id="7748c-121">UserExtend</span></span>  |
| <span data-ttu-id="7748c-122">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="7748c-122">Extend a role assignment</span></span>                    | <span data-ttu-id="7748c-123">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="7748c-123">AdminExtend</span></span> |
| <span data-ttu-id="7748c-124">请求续订已过期角色分配</span><span class="sxs-lookup"><span data-stu-id="7748c-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="7748c-125">UserRenew</span><span class="sxs-lookup"><span data-stu-id="7748c-125">UserRenew</span></span>   |
| <span data-ttu-id="7748c-126">续订过期角色分配</span><span class="sxs-lookup"><span data-stu-id="7748c-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="7748c-127">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="7748c-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="7748c-128">权限</span><span class="sxs-lookup"><span data-stu-id="7748c-128">Permissions</span></span>

<span data-ttu-id="7748c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="7748c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="7748c-131">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="7748c-131">Azure resources</span></span>

| <span data-ttu-id="7748c-132">权限类型</span><span class="sxs-lookup"><span data-stu-id="7748c-132">Permission type</span></span> | <span data-ttu-id="7748c-133">权限</span><span class="sxs-lookup"><span data-stu-id="7748c-133">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="7748c-134">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7748c-134">Delegated (work or school account)</span></span> | <span data-ttu-id="7748c-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="7748c-135">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="7748c-136">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7748c-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7748c-137">不支持。</span><span class="sxs-lookup"><span data-stu-id="7748c-137">Not supported.</span></span> |
| <span data-ttu-id="7748c-138">应用程序</span><span class="sxs-lookup"><span data-stu-id="7748c-138">Application</span></span> | <span data-ttu-id="7748c-139">不支持。</span><span class="sxs-lookup"><span data-stu-id="7748c-139">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="7748c-140">Azure AD</span><span class="sxs-lookup"><span data-stu-id="7748c-140">Azure AD</span></span>

| <span data-ttu-id="7748c-141">权限类型</span><span class="sxs-lookup"><span data-stu-id="7748c-141">Permission type</span></span> | <span data-ttu-id="7748c-142">权限</span><span class="sxs-lookup"><span data-stu-id="7748c-142">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="7748c-143">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7748c-143">Delegated (work or school account)</span></span> | <span data-ttu-id="7748c-144">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="7748c-144">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="7748c-145">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7748c-145">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7748c-146">不支持。</span><span class="sxs-lookup"><span data-stu-id="7748c-146">Not supported.</span></span> |
| <span data-ttu-id="7748c-147">应用程序</span><span class="sxs-lookup"><span data-stu-id="7748c-147">Application</span></span> | <span data-ttu-id="7748c-148">不支持。</span><span class="sxs-lookup"><span data-stu-id="7748c-148">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="7748c-149">组</span><span class="sxs-lookup"><span data-stu-id="7748c-149">Groups</span></span>

|<span data-ttu-id="7748c-150">权限类型</span><span class="sxs-lookup"><span data-stu-id="7748c-150">Permission type</span></span> | <span data-ttu-id="7748c-151">权限</span><span class="sxs-lookup"><span data-stu-id="7748c-151">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="7748c-152">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7748c-152">Delegated (work or school account)</span></span> | <span data-ttu-id="7748c-153">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="7748c-153">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="7748c-154">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7748c-154">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7748c-155">不支持。</span><span class="sxs-lookup"><span data-stu-id="7748c-155">Not supported.</span></span> |
| <span data-ttu-id="7748c-156">应用程序</span><span class="sxs-lookup"><span data-stu-id="7748c-156">Application</span></span> | <span data-ttu-id="7748c-157">不支持。</span><span class="sxs-lookup"><span data-stu-id="7748c-157">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7748c-158">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7748c-158">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="7748c-159">请求标头</span><span class="sxs-lookup"><span data-stu-id="7748c-159">Request headers</span></span>

| <span data-ttu-id="7748c-160">名称</span><span class="sxs-lookup"><span data-stu-id="7748c-160">Name</span></span>          | <span data-ttu-id="7748c-161">说明</span><span class="sxs-lookup"><span data-stu-id="7748c-161">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="7748c-162">Authorization</span><span class="sxs-lookup"><span data-stu-id="7748c-162">Authorization</span></span> | <span data-ttu-id="7748c-163">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7748c-163">Bearer {code}</span></span>    |
| <span data-ttu-id="7748c-164">Content-type</span><span class="sxs-lookup"><span data-stu-id="7748c-164">Content-type</span></span>  | <span data-ttu-id="7748c-165">application/json</span><span class="sxs-lookup"><span data-stu-id="7748c-165">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7748c-166">请求正文</span><span class="sxs-lookup"><span data-stu-id="7748c-166">Request body</span></span>

<span data-ttu-id="7748c-167">在请求正文中，提供 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7748c-167">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="7748c-168">属性</span><span class="sxs-lookup"><span data-stu-id="7748c-168">Property</span></span>         | <span data-ttu-id="7748c-169">类型</span><span class="sxs-lookup"><span data-stu-id="7748c-169">Type</span></span>                                                     | <span data-ttu-id="7748c-170">说明</span><span class="sxs-lookup"><span data-stu-id="7748c-170">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="7748c-171">resourceId</span><span class="sxs-lookup"><span data-stu-id="7748c-171">resourceId</span></span>       | <span data-ttu-id="7748c-172">String</span><span class="sxs-lookup"><span data-stu-id="7748c-172">String</span></span>                                                   | <span data-ttu-id="7748c-173">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="7748c-173">The ID of the resource.</span></span> <span data-ttu-id="7748c-174">必填。</span><span class="sxs-lookup"><span data-stu-id="7748c-174">Required.</span></span> |
| <span data-ttu-id="7748c-175">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7748c-175">roleDefinitionId</span></span> | <span data-ttu-id="7748c-176">String</span><span class="sxs-lookup"><span data-stu-id="7748c-176">String</span></span>                                                   | <span data-ttu-id="7748c-177">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="7748c-177">The ID of the role definition.</span></span> <span data-ttu-id="7748c-178">必填。</span><span class="sxs-lookup"><span data-stu-id="7748c-178">Required.</span></span> |
| <span data-ttu-id="7748c-179">subjectId</span><span class="sxs-lookup"><span data-stu-id="7748c-179">subjectId</span></span>        | <span data-ttu-id="7748c-180">String</span><span class="sxs-lookup"><span data-stu-id="7748c-180">String</span></span>                                                   | <span data-ttu-id="7748c-181">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="7748c-181">The ID of the subject.</span></span> <span data-ttu-id="7748c-182">必填。</span><span class="sxs-lookup"><span data-stu-id="7748c-182">Required.</span></span> |
| <span data-ttu-id="7748c-183">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7748c-183">assignmentState</span></span>  | <span data-ttu-id="7748c-184">String</span><span class="sxs-lookup"><span data-stu-id="7748c-184">String</span></span>                                                   | <span data-ttu-id="7748c-185">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="7748c-185">The state of assignment.</span></span> <span data-ttu-id="7748c-186">值可以是 和 `Eligible` `Active` 。</span><span class="sxs-lookup"><span data-stu-id="7748c-186">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="7748c-187">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="7748c-187">Required.</span></span> |
| <span data-ttu-id="7748c-188">type</span><span class="sxs-lookup"><span data-stu-id="7748c-188">type</span></span>             | <span data-ttu-id="7748c-189">String</span><span class="sxs-lookup"><span data-stu-id="7748c-189">String</span></span>                                                   | <span data-ttu-id="7748c-190">请求类型。</span><span class="sxs-lookup"><span data-stu-id="7748c-190">The request type.</span></span> <span data-ttu-id="7748c-191">值可以是 `AdminAdd` `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` 、、、、、 `UserExtend` `UserRenew` 和 `AdminRenew` `AdminExtend` 。</span><span class="sxs-lookup"><span data-stu-id="7748c-191">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="7748c-192">必填。</span><span class="sxs-lookup"><span data-stu-id="7748c-192">Required.</span></span> |
| <span data-ttu-id="7748c-193">reason</span><span class="sxs-lookup"><span data-stu-id="7748c-193">reason</span></span>           | <span data-ttu-id="7748c-194">String</span><span class="sxs-lookup"><span data-stu-id="7748c-194">String</span></span>                                                   | <span data-ttu-id="7748c-195">需要为请求审核和审核角色分配提供原因。</span><span class="sxs-lookup"><span data-stu-id="7748c-195">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="7748c-196">schedule</span><span class="sxs-lookup"><span data-stu-id="7748c-196">schedule</span></span>         | [<span data-ttu-id="7748c-197">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7748c-197">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7748c-198">请求角色分配计划。</span><span class="sxs-lookup"><span data-stu-id="7748c-198">The schedule of the role assignment request.</span></span> <span data-ttu-id="7748c-199">对于 、 `UserAdd` `AdminAdd` 、 `AdminUpdate` 和 `AdminExtend` 的请求类型，是必需的。</span><span class="sxs-lookup"><span data-stu-id="7748c-199">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="7748c-200">响应</span><span class="sxs-lookup"><span data-stu-id="7748c-200">Response</span></span>

<span data-ttu-id="7748c-201">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7748c-201">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="7748c-202">错误代码</span><span class="sxs-lookup"><span data-stu-id="7748c-202">Error codes</span></span>

<span data-ttu-id="7748c-203">此 API 返回标准 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="7748c-203">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="7748c-204">此外，它还返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="7748c-204">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="7748c-205">错误代码</span><span class="sxs-lookup"><span data-stu-id="7748c-205">Error code</span></span>     | <span data-ttu-id="7748c-206">错误消息</span><span class="sxs-lookup"><span data-stu-id="7748c-206">Error message</span></span>                               | <span data-ttu-id="7748c-207">详细信息</span><span class="sxs-lookup"><span data-stu-id="7748c-207">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="7748c-208">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7748c-208">400 BadRequest</span></span> | <span data-ttu-id="7748c-209">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="7748c-209">RoleNotFound</span></span>                                | <span data-ttu-id="7748c-210">`roleDefinitionId`找不到请求正文中提供的 。</span><span class="sxs-lookup"><span data-stu-id="7748c-210">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="7748c-211">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7748c-211">400 BadRequest</span></span> | <span data-ttu-id="7748c-212">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="7748c-212">ResourceIsLocked</span></span>                            | <span data-ttu-id="7748c-213">请求正文中提供的资源的状态为 ， `Locked` 无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="7748c-213">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="7748c-214">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7748c-214">400 BadRequest</span></span> | <span data-ttu-id="7748c-215">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="7748c-215">SubjectNotFound</span></span>                             | <span data-ttu-id="7748c-216">`subjectId`找不到请求正文中提供的 。</span><span class="sxs-lookup"><span data-stu-id="7748c-216">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="7748c-217">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7748c-217">400 BadRequest</span></span> | <span data-ttu-id="7748c-218">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="7748c-218">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="7748c-219">系统中已存在待定[governanceRoleAssignmentRequest。](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="7748c-219">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="7748c-220">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7748c-220">400 BadRequest</span></span> | <span data-ttu-id="7748c-221">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="7748c-221">RoleAssignmentExists</span></span>                        | <span data-ttu-id="7748c-222">系统中已存在请求创建的[governanceRoleAssignment。](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7748c-222">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="7748c-223">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7748c-223">400 BadRequest</span></span> | <span data-ttu-id="7748c-224">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="7748c-224">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="7748c-225">系统中不存在请求更新/扩展的[governanceRoleAssignment。](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7748c-225">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="7748c-226">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7748c-226">400 BadRequest</span></span> | <span data-ttu-id="7748c-227">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="7748c-227">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="7748c-228">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部策略，无法创建。</span><span class="sxs-lookup"><span data-stu-id="7748c-228">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="7748c-229">示例</span><span class="sxs-lookup"><span data-stu-id="7748c-229">Examples</span></span>

<span data-ttu-id="7748c-230">以下示例显示如何使用此 API。</span><span class="sxs-lookup"><span data-stu-id="7748c-230">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="7748c-231">示例 1：管理员将用户分配给角色</span><span class="sxs-lookup"><span data-stu-id="7748c-231">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="7748c-232">本示例中，管理员将 nawu@contoso.com 分配给"计费读取者"角色。</span><span class="sxs-lookup"><span data-stu-id="7748c-232">In this example, an administrator assigns user nawu@contoso.com to the Billing Reader role.</span></span>

 ><span data-ttu-id="7748c-233">**注意：** 除了权限之外，此示例还要求请求者至少具有一个管理员角色分配 (`Active` `owner` 或) `user access administrator` 资源。</span><span class="sxs-lookup"><span data-stu-id="7748c-233">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="7748c-234">属性</span><span class="sxs-lookup"><span data-stu-id="7748c-234">Property</span></span>         | <span data-ttu-id="7748c-235">类型</span><span class="sxs-lookup"><span data-stu-id="7748c-235">Type</span></span>                                                     | <span data-ttu-id="7748c-236">必需</span><span class="sxs-lookup"><span data-stu-id="7748c-236">Required</span></span>                 | <span data-ttu-id="7748c-237">值</span><span class="sxs-lookup"><span data-stu-id="7748c-237">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="7748c-238">resourceId</span><span class="sxs-lookup"><span data-stu-id="7748c-238">resourceId</span></span>       | <span data-ttu-id="7748c-239">String</span><span class="sxs-lookup"><span data-stu-id="7748c-239">String</span></span>                                                   | <span data-ttu-id="7748c-240">是</span><span class="sxs-lookup"><span data-stu-id="7748c-240">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="7748c-241">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7748c-241">roleDefinitionId</span></span> | <span data-ttu-id="7748c-242">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-242">String</span></span>                                                   | <span data-ttu-id="7748c-243">是</span><span class="sxs-lookup"><span data-stu-id="7748c-243">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="7748c-244">subjectId</span><span class="sxs-lookup"><span data-stu-id="7748c-244">subjectId</span></span>        | <span data-ttu-id="7748c-245">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-245">String</span></span>                                                   | <span data-ttu-id="7748c-246">是</span><span class="sxs-lookup"><span data-stu-id="7748c-246">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="7748c-247">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7748c-247">assignmentState</span></span>  | <span data-ttu-id="7748c-248">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-248">String</span></span>                                                   | <span data-ttu-id="7748c-249">是</span><span class="sxs-lookup"><span data-stu-id="7748c-249">Yes</span></span>                      | <span data-ttu-id="7748c-250">符合条件的/活动的</span><span class="sxs-lookup"><span data-stu-id="7748c-250">Eligible / Active</span></span> |
| <span data-ttu-id="7748c-251">type</span><span class="sxs-lookup"><span data-stu-id="7748c-251">type</span></span>             | <span data-ttu-id="7748c-252">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-252">String</span></span>                                                   | <span data-ttu-id="7748c-253">是</span><span class="sxs-lookup"><span data-stu-id="7748c-253">Yes</span></span>                      | <span data-ttu-id="7748c-254">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="7748c-254">AdminAdd</span></span> |
| <span data-ttu-id="7748c-255">reason</span><span class="sxs-lookup"><span data-stu-id="7748c-255">reason</span></span>           | <span data-ttu-id="7748c-256">String</span><span class="sxs-lookup"><span data-stu-id="7748c-256">String</span></span>                                                   | <span data-ttu-id="7748c-257">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="7748c-257">depends on role Settings</span></span> |   |
| <span data-ttu-id="7748c-258">schedule</span><span class="sxs-lookup"><span data-stu-id="7748c-258">schedule</span></span>         | [<span data-ttu-id="7748c-259">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7748c-259">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7748c-260">是</span><span class="sxs-lookup"><span data-stu-id="7748c-260">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="7748c-261">请求</span><span class="sxs-lookup"><span data-stu-id="7748c-261">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7748c-262">HTTP</span><span class="sxs-lookup"><span data-stu-id="7748c-262">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7748c-263">C#</span><span class="sxs-lookup"><span data-stu-id="7748c-263">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7748c-264">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7748c-264">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7748c-265">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7748c-265">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7748c-266">Java</span><span class="sxs-lookup"><span data-stu-id="7748c-266">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="7748c-267">响应</span><span class="sxs-lookup"><span data-stu-id="7748c-267">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="7748c-268">示例 2：用户激活符合条件的角色</span><span class="sxs-lookup"><span data-stu-id="7748c-268">Example 2: User activates eligible role</span></span>

<span data-ttu-id="7748c-269">本示例中，用户 nawu@contoso.com 激活符合条件的计费读取者角色。</span><span class="sxs-lookup"><span data-stu-id="7748c-269">In this example, the user nawu@contoso.com activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="7748c-270">属性</span><span class="sxs-lookup"><span data-stu-id="7748c-270">Property</span></span>         | <span data-ttu-id="7748c-271">类型</span><span class="sxs-lookup"><span data-stu-id="7748c-271">Type</span></span>                                                     | <span data-ttu-id="7748c-272">必需</span><span class="sxs-lookup"><span data-stu-id="7748c-272">Required</span></span>                 | <span data-ttu-id="7748c-273">值</span><span class="sxs-lookup"><span data-stu-id="7748c-273">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="7748c-274">resourceId</span><span class="sxs-lookup"><span data-stu-id="7748c-274">resourceId</span></span>       | <span data-ttu-id="7748c-275">String</span><span class="sxs-lookup"><span data-stu-id="7748c-275">String</span></span>                                                   | <span data-ttu-id="7748c-276">是</span><span class="sxs-lookup"><span data-stu-id="7748c-276">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="7748c-277">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7748c-277">roleDefinitionId</span></span> | <span data-ttu-id="7748c-278">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-278">String</span></span>                                                   | <span data-ttu-id="7748c-279">是</span><span class="sxs-lookup"><span data-stu-id="7748c-279">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="7748c-280">subjectId</span><span class="sxs-lookup"><span data-stu-id="7748c-280">subjectId</span></span>        | <span data-ttu-id="7748c-281">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-281">String</span></span>                                                   | <span data-ttu-id="7748c-282">是</span><span class="sxs-lookup"><span data-stu-id="7748c-282">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="7748c-283">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7748c-283">assignmentState</span></span>  | <span data-ttu-id="7748c-284">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-284">String</span></span>                                                   | <span data-ttu-id="7748c-285">是</span><span class="sxs-lookup"><span data-stu-id="7748c-285">Yes</span></span>                      | <span data-ttu-id="7748c-286">活动</span><span class="sxs-lookup"><span data-stu-id="7748c-286">Active</span></span> |
| <span data-ttu-id="7748c-287">type</span><span class="sxs-lookup"><span data-stu-id="7748c-287">type</span></span>             | <span data-ttu-id="7748c-288">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-288">String</span></span>                                                   | <span data-ttu-id="7748c-289">是</span><span class="sxs-lookup"><span data-stu-id="7748c-289">Yes</span></span>                      | <span data-ttu-id="7748c-290">UserAdd</span><span class="sxs-lookup"><span data-stu-id="7748c-290">UserAdd</span></span> |
| <span data-ttu-id="7748c-291">reason</span><span class="sxs-lookup"><span data-stu-id="7748c-291">reason</span></span>           | <span data-ttu-id="7748c-292">String</span><span class="sxs-lookup"><span data-stu-id="7748c-292">String</span></span>                                                   | <span data-ttu-id="7748c-293">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="7748c-293">depends on role Settings</span></span> |   |
| <span data-ttu-id="7748c-294">schedule</span><span class="sxs-lookup"><span data-stu-id="7748c-294">schedule</span></span>         | [<span data-ttu-id="7748c-295">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7748c-295">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7748c-296">是</span><span class="sxs-lookup"><span data-stu-id="7748c-296">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="7748c-297">请求</span><span class="sxs-lookup"><span data-stu-id="7748c-297">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7748c-298">HTTP</span><span class="sxs-lookup"><span data-stu-id="7748c-298">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7748c-299">C#</span><span class="sxs-lookup"><span data-stu-id="7748c-299">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7748c-300">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7748c-300">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7748c-301">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7748c-301">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7748c-302">Java</span><span class="sxs-lookup"><span data-stu-id="7748c-302">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7748c-303">响应</span><span class="sxs-lookup"><span data-stu-id="7748c-303">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="7748c-304">示例 3：用户停用分配的角色</span><span class="sxs-lookup"><span data-stu-id="7748c-304">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="7748c-305">本示例中，用户 nawu@contoso.com 活动"计费读取者"角色。</span><span class="sxs-lookup"><span data-stu-id="7748c-305">In this example, the user nawu@contoso.com deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="7748c-306">属性</span><span class="sxs-lookup"><span data-stu-id="7748c-306">Property</span></span>         | <span data-ttu-id="7748c-307">类型</span><span class="sxs-lookup"><span data-stu-id="7748c-307">Type</span></span>                                                     | <span data-ttu-id="7748c-308">必需</span><span class="sxs-lookup"><span data-stu-id="7748c-308">Required</span></span> | <span data-ttu-id="7748c-309">值</span><span class="sxs-lookup"><span data-stu-id="7748c-309">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="7748c-310">resourceId</span><span class="sxs-lookup"><span data-stu-id="7748c-310">resourceId</span></span>       | <span data-ttu-id="7748c-311">String</span><span class="sxs-lookup"><span data-stu-id="7748c-311">String</span></span>                                                   | <span data-ttu-id="7748c-312">是</span><span class="sxs-lookup"><span data-stu-id="7748c-312">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="7748c-313">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7748c-313">roleDefinitionId</span></span> | <span data-ttu-id="7748c-314">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-314">String</span></span>                                                   | <span data-ttu-id="7748c-315">是</span><span class="sxs-lookup"><span data-stu-id="7748c-315">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="7748c-316">subjectId</span><span class="sxs-lookup"><span data-stu-id="7748c-316">subjectId</span></span>        | <span data-ttu-id="7748c-317">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-317">String</span></span>                                                   | <span data-ttu-id="7748c-318">是</span><span class="sxs-lookup"><span data-stu-id="7748c-318">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="7748c-319">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7748c-319">assignmentState</span></span>  | <span data-ttu-id="7748c-320">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-320">String</span></span>                                                   | <span data-ttu-id="7748c-321">是</span><span class="sxs-lookup"><span data-stu-id="7748c-321">Yes</span></span>      | <span data-ttu-id="7748c-322">活动</span><span class="sxs-lookup"><span data-stu-id="7748c-322">Active</span></span> |
| <span data-ttu-id="7748c-323">type</span><span class="sxs-lookup"><span data-stu-id="7748c-323">type</span></span>             | <span data-ttu-id="7748c-324">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-324">String</span></span>                                                   | <span data-ttu-id="7748c-325">是</span><span class="sxs-lookup"><span data-stu-id="7748c-325">Yes</span></span>      | <span data-ttu-id="7748c-326">UserRemove</span><span class="sxs-lookup"><span data-stu-id="7748c-326">UserRemove</span></span> |
| <span data-ttu-id="7748c-327">reason</span><span class="sxs-lookup"><span data-stu-id="7748c-327">reason</span></span>           | <span data-ttu-id="7748c-328">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-328">String</span></span>                                                   | <span data-ttu-id="7748c-329">否</span><span class="sxs-lookup"><span data-stu-id="7748c-329">No</span></span>       |   |
| <span data-ttu-id="7748c-330">schedule</span><span class="sxs-lookup"><span data-stu-id="7748c-330">schedule</span></span>         | [<span data-ttu-id="7748c-331">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7748c-331">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7748c-332">否</span><span class="sxs-lookup"><span data-stu-id="7748c-332">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="7748c-333">请求</span><span class="sxs-lookup"><span data-stu-id="7748c-333">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7748c-334">HTTP</span><span class="sxs-lookup"><span data-stu-id="7748c-334">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7748c-335">C#</span><span class="sxs-lookup"><span data-stu-id="7748c-335">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7748c-336">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7748c-336">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7748c-337">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7748c-337">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7748c-338">Java</span><span class="sxs-lookup"><span data-stu-id="7748c-338">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7748c-339">响应</span><span class="sxs-lookup"><span data-stu-id="7748c-339">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="7748c-340">示例 4：管理员从角色中删除用户</span><span class="sxs-lookup"><span data-stu-id="7748c-340">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="7748c-341">本示例中，管理员从计费读取 nawu@contoso.com 中删除用户角色。</span><span class="sxs-lookup"><span data-stu-id="7748c-341">In this example, an administrator removes the user nawu@contoso.com from the Billing Reader role.</span></span>

 ><span data-ttu-id="7748c-342">**注意：** 除了权限之外，此示例还要求请求者至少具有一个管理员角色分配 (`Active` `owner` 或) `user access administrator` 资源。</span><span class="sxs-lookup"><span data-stu-id="7748c-342">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="7748c-343">属性</span><span class="sxs-lookup"><span data-stu-id="7748c-343">Property</span></span>         | <span data-ttu-id="7748c-344">类型</span><span class="sxs-lookup"><span data-stu-id="7748c-344">Type</span></span>                                                     | <span data-ttu-id="7748c-345">必需</span><span class="sxs-lookup"><span data-stu-id="7748c-345">Required</span></span> | <span data-ttu-id="7748c-346">值</span><span class="sxs-lookup"><span data-stu-id="7748c-346">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="7748c-347">resourceId</span><span class="sxs-lookup"><span data-stu-id="7748c-347">resourceId</span></span>       | <span data-ttu-id="7748c-348">String</span><span class="sxs-lookup"><span data-stu-id="7748c-348">String</span></span>                                                   | <span data-ttu-id="7748c-349">是</span><span class="sxs-lookup"><span data-stu-id="7748c-349">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="7748c-350">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7748c-350">roleDefinitionId</span></span> | <span data-ttu-id="7748c-351">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-351">String</span></span>                                                   | <span data-ttu-id="7748c-352">是</span><span class="sxs-lookup"><span data-stu-id="7748c-352">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="7748c-353">subjectId</span><span class="sxs-lookup"><span data-stu-id="7748c-353">subjectId</span></span>        | <span data-ttu-id="7748c-354">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-354">String</span></span>                                                   | <span data-ttu-id="7748c-355">是</span><span class="sxs-lookup"><span data-stu-id="7748c-355">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="7748c-356">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7748c-356">assignmentState</span></span>  | <span data-ttu-id="7748c-357">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-357">String</span></span>                                                   | <span data-ttu-id="7748c-358">是</span><span class="sxs-lookup"><span data-stu-id="7748c-358">Yes</span></span>      | <span data-ttu-id="7748c-359">符合条件的/活动的</span><span class="sxs-lookup"><span data-stu-id="7748c-359">Eligible / Active</span></span> |
| <span data-ttu-id="7748c-360">type</span><span class="sxs-lookup"><span data-stu-id="7748c-360">type</span></span>             | <span data-ttu-id="7748c-361">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-361">String</span></span>                                                   | <span data-ttu-id="7748c-362">是</span><span class="sxs-lookup"><span data-stu-id="7748c-362">Yes</span></span>      | <span data-ttu-id="7748c-363">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="7748c-363">AdminRemove</span></span> |
| <span data-ttu-id="7748c-364">reason</span><span class="sxs-lookup"><span data-stu-id="7748c-364">reason</span></span>           | <span data-ttu-id="7748c-365">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-365">String</span></span>                                                   | <span data-ttu-id="7748c-366">否</span><span class="sxs-lookup"><span data-stu-id="7748c-366">No</span></span>       |   |
| <span data-ttu-id="7748c-367">schedule</span><span class="sxs-lookup"><span data-stu-id="7748c-367">schedule</span></span>         | [<span data-ttu-id="7748c-368">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7748c-368">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7748c-369">否</span><span class="sxs-lookup"><span data-stu-id="7748c-369">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="7748c-370">请求</span><span class="sxs-lookup"><span data-stu-id="7748c-370">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7748c-371">HTTP</span><span class="sxs-lookup"><span data-stu-id="7748c-371">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7748c-372">C#</span><span class="sxs-lookup"><span data-stu-id="7748c-372">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7748c-373">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7748c-373">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7748c-374">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7748c-374">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7748c-375">Java</span><span class="sxs-lookup"><span data-stu-id="7748c-375">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7748c-376">响应</span><span class="sxs-lookup"><span data-stu-id="7748c-376">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="7748c-377">示例 5：管理员更新角色分配</span><span class="sxs-lookup"><span data-stu-id="7748c-377">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="7748c-378">本示例中，管理员更新角色分配所有者 nawu@contoso.com 权限。</span><span class="sxs-lookup"><span data-stu-id="7748c-378">In this example, administrators update the role assignment for the user nawu@contoso.com to Owner.</span></span>

 ><span data-ttu-id="7748c-379">**注意：** 除了权限之外，此示例还要求请求者至少具有一个管理员角色分配 (`Active` `owner` 或) `user access administrator` 资源。</span><span class="sxs-lookup"><span data-stu-id="7748c-379">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="7748c-380">属性</span><span class="sxs-lookup"><span data-stu-id="7748c-380">Property</span></span>         | <span data-ttu-id="7748c-381">类型</span><span class="sxs-lookup"><span data-stu-id="7748c-381">Type</span></span>                                                     | <span data-ttu-id="7748c-382">必需</span><span class="sxs-lookup"><span data-stu-id="7748c-382">Required</span></span>                | <span data-ttu-id="7748c-383">值</span><span class="sxs-lookup"><span data-stu-id="7748c-383">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="7748c-384">resourceId</span><span class="sxs-lookup"><span data-stu-id="7748c-384">resourceId</span></span>       | <span data-ttu-id="7748c-385">String</span><span class="sxs-lookup"><span data-stu-id="7748c-385">String</span></span>                                                   | <span data-ttu-id="7748c-386">是</span><span class="sxs-lookup"><span data-stu-id="7748c-386">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="7748c-387">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7748c-387">roleDefinitionId</span></span> | <span data-ttu-id="7748c-388">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-388">String</span></span>                                                   | <span data-ttu-id="7748c-389">是</span><span class="sxs-lookup"><span data-stu-id="7748c-389">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="7748c-390">subjectId</span><span class="sxs-lookup"><span data-stu-id="7748c-390">subjectId</span></span>        | <span data-ttu-id="7748c-391">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-391">String</span></span>                                                   | <span data-ttu-id="7748c-392">是</span><span class="sxs-lookup"><span data-stu-id="7748c-392">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="7748c-393">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7748c-393">assignmentState</span></span>  | <span data-ttu-id="7748c-394">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-394">String</span></span>                                                   | <span data-ttu-id="7748c-395">是</span><span class="sxs-lookup"><span data-stu-id="7748c-395">Yes</span></span>                     | <span data-ttu-id="7748c-396">符合条件的/活动的</span><span class="sxs-lookup"><span data-stu-id="7748c-396">Eligible / Active</span></span> |
| <span data-ttu-id="7748c-397">type</span><span class="sxs-lookup"><span data-stu-id="7748c-397">type</span></span>             | <span data-ttu-id="7748c-398">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-398">String</span></span>                                                   | <span data-ttu-id="7748c-399">是</span><span class="sxs-lookup"><span data-stu-id="7748c-399">Yes</span></span>                     | <span data-ttu-id="7748c-400">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="7748c-400">AdminUpdate</span></span> |
| <span data-ttu-id="7748c-401">reason</span><span class="sxs-lookup"><span data-stu-id="7748c-401">reason</span></span>           | <span data-ttu-id="7748c-402">String</span><span class="sxs-lookup"><span data-stu-id="7748c-402">String</span></span>                                                   | <span data-ttu-id="7748c-403">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="7748c-403">depends on roleSettings</span></span> |   |
| <span data-ttu-id="7748c-404">schedule</span><span class="sxs-lookup"><span data-stu-id="7748c-404">schedule</span></span>         | [<span data-ttu-id="7748c-405">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7748c-405">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7748c-406">是</span><span class="sxs-lookup"><span data-stu-id="7748c-406">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="7748c-407">请求</span><span class="sxs-lookup"><span data-stu-id="7748c-407">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7748c-408">HTTP</span><span class="sxs-lookup"><span data-stu-id="7748c-408">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7748c-409">C#</span><span class="sxs-lookup"><span data-stu-id="7748c-409">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7748c-410">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7748c-410">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7748c-411">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7748c-411">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7748c-412">Java</span><span class="sxs-lookup"><span data-stu-id="7748c-412">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7748c-413">响应</span><span class="sxs-lookup"><span data-stu-id="7748c-413">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="7748c-414">示例 6：管理员扩展过期角色分配</span><span class="sxs-lookup"><span data-stu-id="7748c-414">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="7748c-415">此示例将用户 ANUJCUSER 角色分配 API 管理服务参与者的到期日期。</span><span class="sxs-lookup"><span data-stu-id="7748c-415">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="7748c-416">**注意：** 除了权限之外，此示例还要求请求者至少具有一个管理员角色分配 (`Active` `owner` 或) `user access administrator` 资源。</span><span class="sxs-lookup"><span data-stu-id="7748c-416">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="7748c-417">属性</span><span class="sxs-lookup"><span data-stu-id="7748c-417">Property</span></span>         | <span data-ttu-id="7748c-418">类型</span><span class="sxs-lookup"><span data-stu-id="7748c-418">Type</span></span>                                                     | <span data-ttu-id="7748c-419">必需</span><span class="sxs-lookup"><span data-stu-id="7748c-419">Required</span></span>                | <span data-ttu-id="7748c-420">值</span><span class="sxs-lookup"><span data-stu-id="7748c-420">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="7748c-421">resourceId</span><span class="sxs-lookup"><span data-stu-id="7748c-421">resourceId</span></span>       | <span data-ttu-id="7748c-422">String</span><span class="sxs-lookup"><span data-stu-id="7748c-422">String</span></span>                                                   | <span data-ttu-id="7748c-423">是</span><span class="sxs-lookup"><span data-stu-id="7748c-423">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="7748c-424">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7748c-424">roleDefinitionId</span></span> | <span data-ttu-id="7748c-425">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-425">String</span></span>                                                   | <span data-ttu-id="7748c-426">是</span><span class="sxs-lookup"><span data-stu-id="7748c-426">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="7748c-427">subjectId</span><span class="sxs-lookup"><span data-stu-id="7748c-427">subjectId</span></span>        | <span data-ttu-id="7748c-428">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-428">String</span></span>                                                   | <span data-ttu-id="7748c-429">是</span><span class="sxs-lookup"><span data-stu-id="7748c-429">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="7748c-430">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7748c-430">assignmentState</span></span>  | <span data-ttu-id="7748c-431">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-431">String</span></span>                                                   | <span data-ttu-id="7748c-432">是</span><span class="sxs-lookup"><span data-stu-id="7748c-432">Yes</span></span>                     | <span data-ttu-id="7748c-433">符合条件的/活动的</span><span class="sxs-lookup"><span data-stu-id="7748c-433">Eligible / Active</span></span> |
| <span data-ttu-id="7748c-434">type</span><span class="sxs-lookup"><span data-stu-id="7748c-434">type</span></span>             | <span data-ttu-id="7748c-435">字符串</span><span class="sxs-lookup"><span data-stu-id="7748c-435">String</span></span>                                                   | <span data-ttu-id="7748c-436">是</span><span class="sxs-lookup"><span data-stu-id="7748c-436">Yes</span></span>                     | <span data-ttu-id="7748c-437">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="7748c-437">AdminExtend</span></span> |
| <span data-ttu-id="7748c-438">reason</span><span class="sxs-lookup"><span data-stu-id="7748c-438">reason</span></span>           | <span data-ttu-id="7748c-439">String</span><span class="sxs-lookup"><span data-stu-id="7748c-439">String</span></span>                                                   | <span data-ttu-id="7748c-440">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="7748c-440">depends on roleSettings</span></span> |   |
| <span data-ttu-id="7748c-441">schedule</span><span class="sxs-lookup"><span data-stu-id="7748c-441">schedule</span></span>         | [<span data-ttu-id="7748c-442">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7748c-442">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7748c-443">是</span><span class="sxs-lookup"><span data-stu-id="7748c-443">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="7748c-444">请求</span><span class="sxs-lookup"><span data-stu-id="7748c-444">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7748c-445">HTTP</span><span class="sxs-lookup"><span data-stu-id="7748c-445">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7748c-446">C#</span><span class="sxs-lookup"><span data-stu-id="7748c-446">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-6-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7748c-447">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7748c-447">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-6-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7748c-448">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7748c-448">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-6-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7748c-449">Java</span><span class="sxs-lookup"><span data-stu-id="7748c-449">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-6-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7748c-450">响应</span><span class="sxs-lookup"><span data-stu-id="7748c-450">Response</span></span>

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


