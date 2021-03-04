---
title: 创建 governanceRoleAssignmentRequest
description: 创建角色分配请求，以表示要执行的操作角色分配。 下表列出了操作。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 2cb6ee71c888e90ee082c1f70ecced2c21199939
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435859"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="18ed0-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="18ed0-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="18ed0-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18ed0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18ed0-106">创建角色分配请求，以表示要执行的操作角色分配。</span><span class="sxs-lookup"><span data-stu-id="18ed0-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="18ed0-107">下表列出了操作。</span><span class="sxs-lookup"><span data-stu-id="18ed0-107">The following table lists the operations.</span></span>

| <span data-ttu-id="18ed0-108">Operation</span><span class="sxs-lookup"><span data-stu-id="18ed0-108">Operation</span></span>                                   | <span data-ttu-id="18ed0-109">类型</span><span class="sxs-lookup"><span data-stu-id="18ed0-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="18ed0-110">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="18ed0-110">Assign a role assignment</span></span>                    | <span data-ttu-id="18ed0-111">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="18ed0-111">AdminAdd</span></span>    |
| <span data-ttu-id="18ed0-112">激活符合条件的角色分配</span><span class="sxs-lookup"><span data-stu-id="18ed0-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="18ed0-113">UserAdd</span><span class="sxs-lookup"><span data-stu-id="18ed0-113">UserAdd</span></span>     |
| <span data-ttu-id="18ed0-114">停用已激活角色分配</span><span class="sxs-lookup"><span data-stu-id="18ed0-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="18ed0-115">UserRemove</span><span class="sxs-lookup"><span data-stu-id="18ed0-115">UserRemove</span></span>  |
| <span data-ttu-id="18ed0-116">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="18ed0-116">Remove a role assignment</span></span>                    | <span data-ttu-id="18ed0-117">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="18ed0-117">AdminRemove</span></span> |
| <span data-ttu-id="18ed0-118">更新角色分配</span><span class="sxs-lookup"><span data-stu-id="18ed0-118">Update a role assignment</span></span>                    | <span data-ttu-id="18ed0-119">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="18ed0-119">AdminUpdate</span></span> |
| <span data-ttu-id="18ed0-120">请求扩展我的角色分配</span><span class="sxs-lookup"><span data-stu-id="18ed0-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="18ed0-121">UserExtend</span><span class="sxs-lookup"><span data-stu-id="18ed0-121">UserExtend</span></span>  |
| <span data-ttu-id="18ed0-122">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="18ed0-122">Extend a role assignment</span></span>                    | <span data-ttu-id="18ed0-123">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="18ed0-123">AdminExtend</span></span> |
| <span data-ttu-id="18ed0-124">请求续订已过期角色分配</span><span class="sxs-lookup"><span data-stu-id="18ed0-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="18ed0-125">UserRenew</span><span class="sxs-lookup"><span data-stu-id="18ed0-125">UserRenew</span></span>   |
| <span data-ttu-id="18ed0-126">续订已过期角色分配</span><span class="sxs-lookup"><span data-stu-id="18ed0-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="18ed0-127">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="18ed0-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="18ed0-128">Permissions</span><span class="sxs-lookup"><span data-stu-id="18ed0-128">Permissions</span></span>

<span data-ttu-id="18ed0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="18ed0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="18ed0-131">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="18ed0-131">Azure resources</span></span>

| <span data-ttu-id="18ed0-132">权限类型</span><span class="sxs-lookup"><span data-stu-id="18ed0-132">Permission type</span></span> | <span data-ttu-id="18ed0-133">权限</span><span class="sxs-lookup"><span data-stu-id="18ed0-133">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="18ed0-134">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18ed0-134">Delegated (work or school account)</span></span> | <span data-ttu-id="18ed0-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="18ed0-135">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="18ed0-136">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18ed0-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18ed0-137">不支持。</span><span class="sxs-lookup"><span data-stu-id="18ed0-137">Not supported.</span></span> |
| <span data-ttu-id="18ed0-138">Application</span><span class="sxs-lookup"><span data-stu-id="18ed0-138">Application</span></span> | <span data-ttu-id="18ed0-139">不支持。</span><span class="sxs-lookup"><span data-stu-id="18ed0-139">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="18ed0-140">Azure AD</span><span class="sxs-lookup"><span data-stu-id="18ed0-140">Azure AD</span></span>

| <span data-ttu-id="18ed0-141">权限类型</span><span class="sxs-lookup"><span data-stu-id="18ed0-141">Permission type</span></span> | <span data-ttu-id="18ed0-142">权限</span><span class="sxs-lookup"><span data-stu-id="18ed0-142">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="18ed0-143">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18ed0-143">Delegated (work or school account)</span></span> | <span data-ttu-id="18ed0-144">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="18ed0-144">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="18ed0-145">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18ed0-145">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18ed0-146">不支持。</span><span class="sxs-lookup"><span data-stu-id="18ed0-146">Not supported.</span></span> |
| <span data-ttu-id="18ed0-147">Application</span><span class="sxs-lookup"><span data-stu-id="18ed0-147">Application</span></span> | <span data-ttu-id="18ed0-148">不支持。</span><span class="sxs-lookup"><span data-stu-id="18ed0-148">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="18ed0-149">组</span><span class="sxs-lookup"><span data-stu-id="18ed0-149">Groups</span></span>

|<span data-ttu-id="18ed0-150">权限类型</span><span class="sxs-lookup"><span data-stu-id="18ed0-150">Permission type</span></span> | <span data-ttu-id="18ed0-151">权限</span><span class="sxs-lookup"><span data-stu-id="18ed0-151">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="18ed0-152">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18ed0-152">Delegated (work or school account)</span></span> | <span data-ttu-id="18ed0-153">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="18ed0-153">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="18ed0-154">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18ed0-154">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18ed0-155">不支持。</span><span class="sxs-lookup"><span data-stu-id="18ed0-155">Not supported.</span></span> |
| <span data-ttu-id="18ed0-156">Application</span><span class="sxs-lookup"><span data-stu-id="18ed0-156">Application</span></span> | <span data-ttu-id="18ed0-157">不支持。</span><span class="sxs-lookup"><span data-stu-id="18ed0-157">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="18ed0-158">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18ed0-158">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="18ed0-159">请求标头</span><span class="sxs-lookup"><span data-stu-id="18ed0-159">Request headers</span></span>

| <span data-ttu-id="18ed0-160">名称</span><span class="sxs-lookup"><span data-stu-id="18ed0-160">Name</span></span>          | <span data-ttu-id="18ed0-161">说明</span><span class="sxs-lookup"><span data-stu-id="18ed0-161">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="18ed0-162">Authorization</span><span class="sxs-lookup"><span data-stu-id="18ed0-162">Authorization</span></span> | <span data-ttu-id="18ed0-163">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="18ed0-163">Bearer {code}</span></span>    |
| <span data-ttu-id="18ed0-164">Content-type</span><span class="sxs-lookup"><span data-stu-id="18ed0-164">Content-type</span></span>  | <span data-ttu-id="18ed0-165">application/json</span><span class="sxs-lookup"><span data-stu-id="18ed0-165">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="18ed0-166">请求正文</span><span class="sxs-lookup"><span data-stu-id="18ed0-166">Request body</span></span>

<span data-ttu-id="18ed0-167">在请求正文中，提供 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18ed0-167">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="18ed0-168">属性</span><span class="sxs-lookup"><span data-stu-id="18ed0-168">Property</span></span>         | <span data-ttu-id="18ed0-169">类型</span><span class="sxs-lookup"><span data-stu-id="18ed0-169">Type</span></span>                                                     | <span data-ttu-id="18ed0-170">说明</span><span class="sxs-lookup"><span data-stu-id="18ed0-170">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="18ed0-171">resourceId</span><span class="sxs-lookup"><span data-stu-id="18ed0-171">resourceId</span></span>       | <span data-ttu-id="18ed0-172">String</span><span class="sxs-lookup"><span data-stu-id="18ed0-172">String</span></span>                                                   | <span data-ttu-id="18ed0-173">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="18ed0-173">The ID of the resource.</span></span> <span data-ttu-id="18ed0-174">必需。</span><span class="sxs-lookup"><span data-stu-id="18ed0-174">Required.</span></span> |
| <span data-ttu-id="18ed0-175">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="18ed0-175">roleDefinitionId</span></span> | <span data-ttu-id="18ed0-176">String</span><span class="sxs-lookup"><span data-stu-id="18ed0-176">String</span></span>                                                   | <span data-ttu-id="18ed0-177">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="18ed0-177">The ID of the role definition.</span></span> <span data-ttu-id="18ed0-178">必需。</span><span class="sxs-lookup"><span data-stu-id="18ed0-178">Required.</span></span> |
| <span data-ttu-id="18ed0-179">subjectId</span><span class="sxs-lookup"><span data-stu-id="18ed0-179">subjectId</span></span>        | <span data-ttu-id="18ed0-180">String</span><span class="sxs-lookup"><span data-stu-id="18ed0-180">String</span></span>                                                   | <span data-ttu-id="18ed0-181">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="18ed0-181">The ID of the subject.</span></span> <span data-ttu-id="18ed0-182">必需。</span><span class="sxs-lookup"><span data-stu-id="18ed0-182">Required.</span></span> |
| <span data-ttu-id="18ed0-183">assignmentState</span><span class="sxs-lookup"><span data-stu-id="18ed0-183">assignmentState</span></span>  | <span data-ttu-id="18ed0-184">String</span><span class="sxs-lookup"><span data-stu-id="18ed0-184">String</span></span>                                                   | <span data-ttu-id="18ed0-185">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="18ed0-185">The state of assignment.</span></span> <span data-ttu-id="18ed0-186">值可以是 `Eligible` 和 `Active` 。</span><span class="sxs-lookup"><span data-stu-id="18ed0-186">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="18ed0-187">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="18ed0-187">Required.</span></span> |
| <span data-ttu-id="18ed0-188">type</span><span class="sxs-lookup"><span data-stu-id="18ed0-188">type</span></span>             | <span data-ttu-id="18ed0-189">String</span><span class="sxs-lookup"><span data-stu-id="18ed0-189">String</span></span>                                                   | <span data-ttu-id="18ed0-190">请求类型。</span><span class="sxs-lookup"><span data-stu-id="18ed0-190">The request type.</span></span> <span data-ttu-id="18ed0-191">值可以是 `AdminAdd` ， `UserAdd` ， ， ， ， `AdminUpdate` 和 `AdminRemove` `UserRemove` `UserExtend` `UserRenew` `AdminRenew` `AdminExtend` 。</span><span class="sxs-lookup"><span data-stu-id="18ed0-191">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="18ed0-192">必需。</span><span class="sxs-lookup"><span data-stu-id="18ed0-192">Required.</span></span> |
| <span data-ttu-id="18ed0-193">reason</span><span class="sxs-lookup"><span data-stu-id="18ed0-193">reason</span></span>           | <span data-ttu-id="18ed0-194">String</span><span class="sxs-lookup"><span data-stu-id="18ed0-194">String</span></span>                                                   | <span data-ttu-id="18ed0-195">需要为审核和审核角色分配请求提供原因。</span><span class="sxs-lookup"><span data-stu-id="18ed0-195">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="18ed0-196">schedule</span><span class="sxs-lookup"><span data-stu-id="18ed0-196">schedule</span></span>         | [<span data-ttu-id="18ed0-197">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="18ed0-197">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="18ed0-198">请求角色分配计划。</span><span class="sxs-lookup"><span data-stu-id="18ed0-198">The schedule of the role assignment request.</span></span> <span data-ttu-id="18ed0-199">对于 、 `UserAdd` `AdminAdd` 和 的请求类型 `AdminUpdate` `AdminExtend` ，是必需的。</span><span class="sxs-lookup"><span data-stu-id="18ed0-199">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="18ed0-200">响应</span><span class="sxs-lookup"><span data-stu-id="18ed0-200">Response</span></span>

<span data-ttu-id="18ed0-201">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="18ed0-201">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="18ed0-202">错误代码</span><span class="sxs-lookup"><span data-stu-id="18ed0-202">Error codes</span></span>

<span data-ttu-id="18ed0-203">此 API 返回标准 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="18ed0-203">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="18ed0-204">此外，它还返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="18ed0-204">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="18ed0-205">错误代码</span><span class="sxs-lookup"><span data-stu-id="18ed0-205">Error code</span></span>     | <span data-ttu-id="18ed0-206">错误消息</span><span class="sxs-lookup"><span data-stu-id="18ed0-206">Error message</span></span>                               | <span data-ttu-id="18ed0-207">详细信息</span><span class="sxs-lookup"><span data-stu-id="18ed0-207">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="18ed0-208">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="18ed0-208">400 BadRequest</span></span> | <span data-ttu-id="18ed0-209">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="18ed0-209">RoleNotFound</span></span>                                | <span data-ttu-id="18ed0-210">找不到 `roleDefinitionId` 请求正文中提供的信息。</span><span class="sxs-lookup"><span data-stu-id="18ed0-210">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="18ed0-211">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="18ed0-211">400 BadRequest</span></span> | <span data-ttu-id="18ed0-212">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="18ed0-212">ResourceIsLocked</span></span>                            | <span data-ttu-id="18ed0-213">请求正文中提供的资源的状态为， `Locked` 无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="18ed0-213">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="18ed0-214">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="18ed0-214">400 BadRequest</span></span> | <span data-ttu-id="18ed0-215">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="18ed0-215">SubjectNotFound</span></span>                             | <span data-ttu-id="18ed0-216">找不到 `subjectId` 请求正文中提供的信息。</span><span class="sxs-lookup"><span data-stu-id="18ed0-216">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="18ed0-217">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="18ed0-217">400 BadRequest</span></span> | <span data-ttu-id="18ed0-218">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="18ed0-218">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="18ed0-219">系统中已存在挂起的[governanceRoleAssignmentRequest。](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="18ed0-219">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="18ed0-220">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="18ed0-220">400 BadRequest</span></span> | <span data-ttu-id="18ed0-221">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="18ed0-221">RoleAssignmentExists</span></span>                        | <span data-ttu-id="18ed0-222">[系统中已存在请求创建的 governanceRoleAssignment。](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="18ed0-222">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="18ed0-223">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="18ed0-223">400 BadRequest</span></span> | <span data-ttu-id="18ed0-224">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="18ed0-224">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="18ed0-225">系统中不存在请求更新/扩展的[governanceRoleAssignment。](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="18ed0-225">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="18ed0-226">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="18ed0-226">400 BadRequest</span></span> | <span data-ttu-id="18ed0-227">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="18ed0-227">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="18ed0-228">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部策略，无法创建。</span><span class="sxs-lookup"><span data-stu-id="18ed0-228">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="18ed0-229">示例</span><span class="sxs-lookup"><span data-stu-id="18ed0-229">Examples</span></span>

<span data-ttu-id="18ed0-230">以下示例显示如何使用此 API。</span><span class="sxs-lookup"><span data-stu-id="18ed0-230">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="18ed0-231">示例 1：管理员将用户分配给角色</span><span class="sxs-lookup"><span data-stu-id="18ed0-231">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="18ed0-232">本示例中，管理员将用户nawu@contoso.com分配给"计费读者"角色。</span><span class="sxs-lookup"><span data-stu-id="18ed0-232">In this example, an administrator assigns user nawu@contoso.com to the Billing Reader role.</span></span>

 ><span data-ttu-id="18ed0-233">**注意：** 除了权限之外，此示例还要求请求者至少具有一个管理员角色分配 (`Active` `owner` 或) `user access administrator` 资源的权限。</span><span class="sxs-lookup"><span data-stu-id="18ed0-233">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="18ed0-234">属性</span><span class="sxs-lookup"><span data-stu-id="18ed0-234">Property</span></span>         | <span data-ttu-id="18ed0-235">类型</span><span class="sxs-lookup"><span data-stu-id="18ed0-235">Type</span></span>                                                     | <span data-ttu-id="18ed0-236">必需</span><span class="sxs-lookup"><span data-stu-id="18ed0-236">Required</span></span>                 | <span data-ttu-id="18ed0-237">值</span><span class="sxs-lookup"><span data-stu-id="18ed0-237">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="18ed0-238">resourceId</span><span class="sxs-lookup"><span data-stu-id="18ed0-238">resourceId</span></span>       | <span data-ttu-id="18ed0-239">String</span><span class="sxs-lookup"><span data-stu-id="18ed0-239">String</span></span>                                                   | <span data-ttu-id="18ed0-240">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-240">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="18ed0-241">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="18ed0-241">roleDefinitionId</span></span> | <span data-ttu-id="18ed0-242">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-242">String</span></span>                                                   | <span data-ttu-id="18ed0-243">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-243">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="18ed0-244">subjectId</span><span class="sxs-lookup"><span data-stu-id="18ed0-244">subjectId</span></span>        | <span data-ttu-id="18ed0-245">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-245">String</span></span>                                                   | <span data-ttu-id="18ed0-246">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-246">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="18ed0-247">assignmentState</span><span class="sxs-lookup"><span data-stu-id="18ed0-247">assignmentState</span></span>  | <span data-ttu-id="18ed0-248">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-248">String</span></span>                                                   | <span data-ttu-id="18ed0-249">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-249">Yes</span></span>                      | <span data-ttu-id="18ed0-250">符合条件的/活动的</span><span class="sxs-lookup"><span data-stu-id="18ed0-250">Eligible / Active</span></span> |
| <span data-ttu-id="18ed0-251">type</span><span class="sxs-lookup"><span data-stu-id="18ed0-251">type</span></span>             | <span data-ttu-id="18ed0-252">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-252">String</span></span>                                                   | <span data-ttu-id="18ed0-253">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-253">Yes</span></span>                      | <span data-ttu-id="18ed0-254">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="18ed0-254">AdminAdd</span></span> |
| <span data-ttu-id="18ed0-255">reason</span><span class="sxs-lookup"><span data-stu-id="18ed0-255">reason</span></span>           | <span data-ttu-id="18ed0-256">String</span><span class="sxs-lookup"><span data-stu-id="18ed0-256">String</span></span>                                                   | <span data-ttu-id="18ed0-257">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="18ed0-257">depends on role Settings</span></span> |   |
| <span data-ttu-id="18ed0-258">schedule</span><span class="sxs-lookup"><span data-stu-id="18ed0-258">schedule</span></span>         | [<span data-ttu-id="18ed0-259">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="18ed0-259">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="18ed0-260">是的。</span><span class="sxs-lookup"><span data-stu-id="18ed0-260">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="18ed0-261">请求</span><span class="sxs-lookup"><span data-stu-id="18ed0-261">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="18ed0-262">HTTP</span><span class="sxs-lookup"><span data-stu-id="18ed0-262">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="18ed0-263">C#</span><span class="sxs-lookup"><span data-stu-id="18ed0-263">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18ed0-264">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18ed0-264">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18ed0-265">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18ed0-265">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18ed0-266">Java</span><span class="sxs-lookup"><span data-stu-id="18ed0-266">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="18ed0-267">响应</span><span class="sxs-lookup"><span data-stu-id="18ed0-267">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="18ed0-268">示例 2：用户激活符合条件的角色</span><span class="sxs-lookup"><span data-stu-id="18ed0-268">Example 2: User activates eligible role</span></span>

<span data-ttu-id="18ed0-269">此示例中，用户nawu@contoso.com激活符合条件的计费阅读器角色。</span><span class="sxs-lookup"><span data-stu-id="18ed0-269">In this example, the user nawu@contoso.com activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="18ed0-270">属性</span><span class="sxs-lookup"><span data-stu-id="18ed0-270">Property</span></span>         | <span data-ttu-id="18ed0-271">类型</span><span class="sxs-lookup"><span data-stu-id="18ed0-271">Type</span></span>                                                     | <span data-ttu-id="18ed0-272">必需</span><span class="sxs-lookup"><span data-stu-id="18ed0-272">Required</span></span>                 | <span data-ttu-id="18ed0-273">值</span><span class="sxs-lookup"><span data-stu-id="18ed0-273">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="18ed0-274">resourceId</span><span class="sxs-lookup"><span data-stu-id="18ed0-274">resourceId</span></span>       | <span data-ttu-id="18ed0-275">String</span><span class="sxs-lookup"><span data-stu-id="18ed0-275">String</span></span>                                                   | <span data-ttu-id="18ed0-276">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-276">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="18ed0-277">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="18ed0-277">roleDefinitionId</span></span> | <span data-ttu-id="18ed0-278">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-278">String</span></span>                                                   | <span data-ttu-id="18ed0-279">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-279">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="18ed0-280">subjectId</span><span class="sxs-lookup"><span data-stu-id="18ed0-280">subjectId</span></span>        | <span data-ttu-id="18ed0-281">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-281">String</span></span>                                                   | <span data-ttu-id="18ed0-282">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-282">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="18ed0-283">assignmentState</span><span class="sxs-lookup"><span data-stu-id="18ed0-283">assignmentState</span></span>  | <span data-ttu-id="18ed0-284">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-284">String</span></span>                                                   | <span data-ttu-id="18ed0-285">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-285">Yes</span></span>                      | <span data-ttu-id="18ed0-286">活动</span><span class="sxs-lookup"><span data-stu-id="18ed0-286">Active</span></span> |
| <span data-ttu-id="18ed0-287">type</span><span class="sxs-lookup"><span data-stu-id="18ed0-287">type</span></span>             | <span data-ttu-id="18ed0-288">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-288">String</span></span>                                                   | <span data-ttu-id="18ed0-289">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-289">Yes</span></span>                      | <span data-ttu-id="18ed0-290">UserAdd</span><span class="sxs-lookup"><span data-stu-id="18ed0-290">UserAdd</span></span> |
| <span data-ttu-id="18ed0-291">reason</span><span class="sxs-lookup"><span data-stu-id="18ed0-291">reason</span></span>           | <span data-ttu-id="18ed0-292">String</span><span class="sxs-lookup"><span data-stu-id="18ed0-292">String</span></span>                                                   | <span data-ttu-id="18ed0-293">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="18ed0-293">depends on role Settings</span></span> |   |
| <span data-ttu-id="18ed0-294">schedule</span><span class="sxs-lookup"><span data-stu-id="18ed0-294">schedule</span></span>         | [<span data-ttu-id="18ed0-295">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="18ed0-295">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="18ed0-296">是的。</span><span class="sxs-lookup"><span data-stu-id="18ed0-296">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="18ed0-297">请求</span><span class="sxs-lookup"><span data-stu-id="18ed0-297">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="18ed0-298">响应</span><span class="sxs-lookup"><span data-stu-id="18ed0-298">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="18ed0-299">示例 3：用户停用分配的角色</span><span class="sxs-lookup"><span data-stu-id="18ed0-299">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="18ed0-300">本示例中，用户nawu@contoso.com停用活动的计费阅读器角色。</span><span class="sxs-lookup"><span data-stu-id="18ed0-300">In this example, the user nawu@contoso.com deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="18ed0-301">属性</span><span class="sxs-lookup"><span data-stu-id="18ed0-301">Property</span></span>         | <span data-ttu-id="18ed0-302">类型</span><span class="sxs-lookup"><span data-stu-id="18ed0-302">Type</span></span>                                                     | <span data-ttu-id="18ed0-303">必需</span><span class="sxs-lookup"><span data-stu-id="18ed0-303">Required</span></span> | <span data-ttu-id="18ed0-304">值</span><span class="sxs-lookup"><span data-stu-id="18ed0-304">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="18ed0-305">resourceId</span><span class="sxs-lookup"><span data-stu-id="18ed0-305">resourceId</span></span>       | <span data-ttu-id="18ed0-306">String</span><span class="sxs-lookup"><span data-stu-id="18ed0-306">String</span></span>                                                   | <span data-ttu-id="18ed0-307">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-307">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="18ed0-308">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="18ed0-308">roleDefinitionId</span></span> | <span data-ttu-id="18ed0-309">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-309">String</span></span>                                                   | <span data-ttu-id="18ed0-310">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-310">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="18ed0-311">subjectId</span><span class="sxs-lookup"><span data-stu-id="18ed0-311">subjectId</span></span>        | <span data-ttu-id="18ed0-312">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-312">String</span></span>                                                   | <span data-ttu-id="18ed0-313">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-313">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="18ed0-314">assignmentState</span><span class="sxs-lookup"><span data-stu-id="18ed0-314">assignmentState</span></span>  | <span data-ttu-id="18ed0-315">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-315">String</span></span>                                                   | <span data-ttu-id="18ed0-316">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-316">Yes</span></span>      | <span data-ttu-id="18ed0-317">活动</span><span class="sxs-lookup"><span data-stu-id="18ed0-317">Active</span></span> |
| <span data-ttu-id="18ed0-318">type</span><span class="sxs-lookup"><span data-stu-id="18ed0-318">type</span></span>             | <span data-ttu-id="18ed0-319">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-319">String</span></span>                                                   | <span data-ttu-id="18ed0-320">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-320">Yes</span></span>      | <span data-ttu-id="18ed0-321">UserRemove</span><span class="sxs-lookup"><span data-stu-id="18ed0-321">UserRemove</span></span> |
| <span data-ttu-id="18ed0-322">reason</span><span class="sxs-lookup"><span data-stu-id="18ed0-322">reason</span></span>           | <span data-ttu-id="18ed0-323">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-323">String</span></span>                                                   | <span data-ttu-id="18ed0-324">否</span><span class="sxs-lookup"><span data-stu-id="18ed0-324">No</span></span>       |   |
| <span data-ttu-id="18ed0-325">schedule</span><span class="sxs-lookup"><span data-stu-id="18ed0-325">schedule</span></span>         | [<span data-ttu-id="18ed0-326">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="18ed0-326">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="18ed0-327">否</span><span class="sxs-lookup"><span data-stu-id="18ed0-327">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="18ed0-328">请求</span><span class="sxs-lookup"><span data-stu-id="18ed0-328">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="18ed0-329">响应</span><span class="sxs-lookup"><span data-stu-id="18ed0-329">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="18ed0-330">示例 4：管理员从角色中删除用户</span><span class="sxs-lookup"><span data-stu-id="18ed0-330">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="18ed0-331">此示例中，管理员从"nawu@contoso.com读取者"角色中删除用户权限。</span><span class="sxs-lookup"><span data-stu-id="18ed0-331">In this example, an administrator removes the user nawu@contoso.com from the Billing Reader role.</span></span>

 ><span data-ttu-id="18ed0-332">**注意：** 除了权限之外，此示例还要求请求者至少具有一个管理员角色分配 (`Active` `owner` 或) `user access administrator` 资源的权限。</span><span class="sxs-lookup"><span data-stu-id="18ed0-332">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="18ed0-333">属性</span><span class="sxs-lookup"><span data-stu-id="18ed0-333">Property</span></span>         | <span data-ttu-id="18ed0-334">类型</span><span class="sxs-lookup"><span data-stu-id="18ed0-334">Type</span></span>                                                     | <span data-ttu-id="18ed0-335">必需</span><span class="sxs-lookup"><span data-stu-id="18ed0-335">Required</span></span> | <span data-ttu-id="18ed0-336">值</span><span class="sxs-lookup"><span data-stu-id="18ed0-336">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="18ed0-337">resourceId</span><span class="sxs-lookup"><span data-stu-id="18ed0-337">resourceId</span></span>       | <span data-ttu-id="18ed0-338">String</span><span class="sxs-lookup"><span data-stu-id="18ed0-338">String</span></span>                                                   | <span data-ttu-id="18ed0-339">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-339">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="18ed0-340">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="18ed0-340">roleDefinitionId</span></span> | <span data-ttu-id="18ed0-341">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-341">String</span></span>                                                   | <span data-ttu-id="18ed0-342">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-342">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="18ed0-343">subjectId</span><span class="sxs-lookup"><span data-stu-id="18ed0-343">subjectId</span></span>        | <span data-ttu-id="18ed0-344">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-344">String</span></span>                                                   | <span data-ttu-id="18ed0-345">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-345">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="18ed0-346">assignmentState</span><span class="sxs-lookup"><span data-stu-id="18ed0-346">assignmentState</span></span>  | <span data-ttu-id="18ed0-347">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-347">String</span></span>                                                   | <span data-ttu-id="18ed0-348">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-348">Yes</span></span>      | <span data-ttu-id="18ed0-349">符合条件的/活动的</span><span class="sxs-lookup"><span data-stu-id="18ed0-349">Eligible / Active</span></span> |
| <span data-ttu-id="18ed0-350">type</span><span class="sxs-lookup"><span data-stu-id="18ed0-350">type</span></span>             | <span data-ttu-id="18ed0-351">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-351">String</span></span>                                                   | <span data-ttu-id="18ed0-352">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-352">Yes</span></span>      | <span data-ttu-id="18ed0-353">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="18ed0-353">AdminRemove</span></span> |
| <span data-ttu-id="18ed0-354">reason</span><span class="sxs-lookup"><span data-stu-id="18ed0-354">reason</span></span>           | <span data-ttu-id="18ed0-355">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-355">String</span></span>                                                   | <span data-ttu-id="18ed0-356">否</span><span class="sxs-lookup"><span data-stu-id="18ed0-356">No</span></span>       |   |
| <span data-ttu-id="18ed0-357">schedule</span><span class="sxs-lookup"><span data-stu-id="18ed0-357">schedule</span></span>         | [<span data-ttu-id="18ed0-358">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="18ed0-358">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="18ed0-359">否</span><span class="sxs-lookup"><span data-stu-id="18ed0-359">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="18ed0-360">请求</span><span class="sxs-lookup"><span data-stu-id="18ed0-360">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="18ed0-361">响应</span><span class="sxs-lookup"><span data-stu-id="18ed0-361">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="18ed0-362">示例 5：管理员更新角色分配</span><span class="sxs-lookup"><span data-stu-id="18ed0-362">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="18ed0-363">此示例中，管理员将角色分配所有者nawu@contoso.com更新。</span><span class="sxs-lookup"><span data-stu-id="18ed0-363">In this example, administrators update the role assignment for the user nawu@contoso.com to Owner.</span></span>

 ><span data-ttu-id="18ed0-364">**注意：** 除了权限之外，此示例还要求请求者至少具有一个管理员角色分配 (`Active` `owner` 或) `user access administrator` 资源的权限。</span><span class="sxs-lookup"><span data-stu-id="18ed0-364">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="18ed0-365">属性</span><span class="sxs-lookup"><span data-stu-id="18ed0-365">Property</span></span>         | <span data-ttu-id="18ed0-366">类型</span><span class="sxs-lookup"><span data-stu-id="18ed0-366">Type</span></span>                                                     | <span data-ttu-id="18ed0-367">必需</span><span class="sxs-lookup"><span data-stu-id="18ed0-367">Required</span></span>                | <span data-ttu-id="18ed0-368">值</span><span class="sxs-lookup"><span data-stu-id="18ed0-368">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="18ed0-369">resourceId</span><span class="sxs-lookup"><span data-stu-id="18ed0-369">resourceId</span></span>       | <span data-ttu-id="18ed0-370">String</span><span class="sxs-lookup"><span data-stu-id="18ed0-370">String</span></span>                                                   | <span data-ttu-id="18ed0-371">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-371">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="18ed0-372">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="18ed0-372">roleDefinitionId</span></span> | <span data-ttu-id="18ed0-373">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-373">String</span></span>                                                   | <span data-ttu-id="18ed0-374">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-374">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="18ed0-375">subjectId</span><span class="sxs-lookup"><span data-stu-id="18ed0-375">subjectId</span></span>        | <span data-ttu-id="18ed0-376">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-376">String</span></span>                                                   | <span data-ttu-id="18ed0-377">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-377">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="18ed0-378">assignmentState</span><span class="sxs-lookup"><span data-stu-id="18ed0-378">assignmentState</span></span>  | <span data-ttu-id="18ed0-379">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-379">String</span></span>                                                   | <span data-ttu-id="18ed0-380">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-380">Yes</span></span>                     | <span data-ttu-id="18ed0-381">符合条件的/活动的</span><span class="sxs-lookup"><span data-stu-id="18ed0-381">Eligible / Active</span></span> |
| <span data-ttu-id="18ed0-382">type</span><span class="sxs-lookup"><span data-stu-id="18ed0-382">type</span></span>             | <span data-ttu-id="18ed0-383">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-383">String</span></span>                                                   | <span data-ttu-id="18ed0-384">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-384">Yes</span></span>                     | <span data-ttu-id="18ed0-385">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="18ed0-385">AdminUpdate</span></span> |
| <span data-ttu-id="18ed0-386">reason</span><span class="sxs-lookup"><span data-stu-id="18ed0-386">reason</span></span>           | <span data-ttu-id="18ed0-387">String</span><span class="sxs-lookup"><span data-stu-id="18ed0-387">String</span></span>                                                   | <span data-ttu-id="18ed0-388">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="18ed0-388">depends on roleSettings</span></span> |   |
| <span data-ttu-id="18ed0-389">schedule</span><span class="sxs-lookup"><span data-stu-id="18ed0-389">schedule</span></span>         | [<span data-ttu-id="18ed0-390">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="18ed0-390">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="18ed0-391">是的。</span><span class="sxs-lookup"><span data-stu-id="18ed0-391">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="18ed0-392">请求</span><span class="sxs-lookup"><span data-stu-id="18ed0-392">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="18ed0-393">响应</span><span class="sxs-lookup"><span data-stu-id="18ed0-393">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="18ed0-394">示例 6：管理员扩展过期角色分配</span><span class="sxs-lookup"><span data-stu-id="18ed0-394">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="18ed0-395">此示例将用户 ANUJCUSER 角色分配 API 管理服务参与者的到期期限。</span><span class="sxs-lookup"><span data-stu-id="18ed0-395">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="18ed0-396">**注意：** 除了权限之外，此示例还要求请求者至少具有一个管理员角色分配 (`Active` `owner` 或) `user access administrator` 资源的权限。</span><span class="sxs-lookup"><span data-stu-id="18ed0-396">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="18ed0-397">属性</span><span class="sxs-lookup"><span data-stu-id="18ed0-397">Property</span></span>         | <span data-ttu-id="18ed0-398">类型</span><span class="sxs-lookup"><span data-stu-id="18ed0-398">Type</span></span>                                                     | <span data-ttu-id="18ed0-399">必需</span><span class="sxs-lookup"><span data-stu-id="18ed0-399">Required</span></span>                | <span data-ttu-id="18ed0-400">值</span><span class="sxs-lookup"><span data-stu-id="18ed0-400">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="18ed0-401">resourceId</span><span class="sxs-lookup"><span data-stu-id="18ed0-401">resourceId</span></span>       | <span data-ttu-id="18ed0-402">String</span><span class="sxs-lookup"><span data-stu-id="18ed0-402">String</span></span>                                                   | <span data-ttu-id="18ed0-403">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-403">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="18ed0-404">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="18ed0-404">roleDefinitionId</span></span> | <span data-ttu-id="18ed0-405">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-405">String</span></span>                                                   | <span data-ttu-id="18ed0-406">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-406">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="18ed0-407">subjectId</span><span class="sxs-lookup"><span data-stu-id="18ed0-407">subjectId</span></span>        | <span data-ttu-id="18ed0-408">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-408">String</span></span>                                                   | <span data-ttu-id="18ed0-409">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-409">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="18ed0-410">assignmentState</span><span class="sxs-lookup"><span data-stu-id="18ed0-410">assignmentState</span></span>  | <span data-ttu-id="18ed0-411">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-411">String</span></span>                                                   | <span data-ttu-id="18ed0-412">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-412">Yes</span></span>                     | <span data-ttu-id="18ed0-413">符合条件的/活动的</span><span class="sxs-lookup"><span data-stu-id="18ed0-413">Eligible / Active</span></span> |
| <span data-ttu-id="18ed0-414">type</span><span class="sxs-lookup"><span data-stu-id="18ed0-414">type</span></span>             | <span data-ttu-id="18ed0-415">字符串</span><span class="sxs-lookup"><span data-stu-id="18ed0-415">String</span></span>                                                   | <span data-ttu-id="18ed0-416">是</span><span class="sxs-lookup"><span data-stu-id="18ed0-416">Yes</span></span>                     | <span data-ttu-id="18ed0-417">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="18ed0-417">AdminExtend</span></span> |
| <span data-ttu-id="18ed0-418">reason</span><span class="sxs-lookup"><span data-stu-id="18ed0-418">reason</span></span>           | <span data-ttu-id="18ed0-419">String</span><span class="sxs-lookup"><span data-stu-id="18ed0-419">String</span></span>                                                   | <span data-ttu-id="18ed0-420">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="18ed0-420">depends on roleSettings</span></span> |   |
| <span data-ttu-id="18ed0-421">schedule</span><span class="sxs-lookup"><span data-stu-id="18ed0-421">schedule</span></span>         | [<span data-ttu-id="18ed0-422">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="18ed0-422">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="18ed0-423">是的。</span><span class="sxs-lookup"><span data-stu-id="18ed0-423">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="18ed0-424">请求</span><span class="sxs-lookup"><span data-stu-id="18ed0-424">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="18ed0-425">响应</span><span class="sxs-lookup"><span data-stu-id="18ed0-425">Response</span></span>

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


