---
title: 创建 governanceRoleAssignmentRequest
description: 创建一个角色分配请求，以代表在角色分配上所需的操作。 下表列出了这些操作。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: a76727ffd927f7d91b953c313b11a59e4512a65e
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634996"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="319f4-104">创建 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="319f4-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="319f4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="319f4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="319f4-106">创建一个角色分配请求，以代表在角色分配上所需的操作。</span><span class="sxs-lookup"><span data-stu-id="319f4-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="319f4-107">下表列出了这些操作。</span><span class="sxs-lookup"><span data-stu-id="319f4-107">The following table lists the operations.</span></span>

| <span data-ttu-id="319f4-108">Operation</span><span class="sxs-lookup"><span data-stu-id="319f4-108">Operation</span></span>                                   | <span data-ttu-id="319f4-109">类型</span><span class="sxs-lookup"><span data-stu-id="319f4-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="319f4-110">分配角色分配</span><span class="sxs-lookup"><span data-stu-id="319f4-110">Assign a role assignment</span></span>                    | <span data-ttu-id="319f4-111">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="319f4-111">AdminAdd</span></span>    |
| <span data-ttu-id="319f4-112">激活符合条件的角色分配</span><span class="sxs-lookup"><span data-stu-id="319f4-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="319f4-113">UserAdd</span><span class="sxs-lookup"><span data-stu-id="319f4-113">UserAdd</span></span>     |
| <span data-ttu-id="319f4-114">停用已激活的角色分配</span><span class="sxs-lookup"><span data-stu-id="319f4-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="319f4-115">UserRemove</span><span class="sxs-lookup"><span data-stu-id="319f4-115">UserRemove</span></span>  |
| <span data-ttu-id="319f4-116">删除角色分配</span><span class="sxs-lookup"><span data-stu-id="319f4-116">Remove a role assignment</span></span>                    | <span data-ttu-id="319f4-117">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="319f4-117">AdminRemove</span></span> |
| <span data-ttu-id="319f4-118">更新角色分配</span><span class="sxs-lookup"><span data-stu-id="319f4-118">Update a role assignment</span></span>                    | <span data-ttu-id="319f4-119">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="319f4-119">AdminUpdate</span></span> |
| <span data-ttu-id="319f4-120">请求扩展我的角色分配</span><span class="sxs-lookup"><span data-stu-id="319f4-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="319f4-121">UserExtend</span><span class="sxs-lookup"><span data-stu-id="319f4-121">UserExtend</span></span>  |
| <span data-ttu-id="319f4-122">扩展角色分配</span><span class="sxs-lookup"><span data-stu-id="319f4-122">Extend a role assignment</span></span>                    | <span data-ttu-id="319f4-123">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="319f4-123">AdminExtend</span></span> |
| <span data-ttu-id="319f4-124">续订我的过期角色分配的请求</span><span class="sxs-lookup"><span data-stu-id="319f4-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="319f4-125">UserRenew</span><span class="sxs-lookup"><span data-stu-id="319f4-125">UserRenew</span></span>   |
| <span data-ttu-id="319f4-126">续订过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="319f4-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="319f4-127">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="319f4-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="319f4-128">权限</span><span class="sxs-lookup"><span data-stu-id="319f4-128">Permissions</span></span>

<span data-ttu-id="319f4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="319f4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="319f4-131">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="319f4-131">Azure resources</span></span>

| <span data-ttu-id="319f4-132">权限类型</span><span class="sxs-lookup"><span data-stu-id="319f4-132">Permission type</span></span> | <span data-ttu-id="319f4-133">权限</span><span class="sxs-lookup"><span data-stu-id="319f4-133">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="319f4-134">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="319f4-134">Delegated (work or school account)</span></span> | <span data-ttu-id="319f4-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="319f4-135">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="319f4-136">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="319f4-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="319f4-137">不支持。</span><span class="sxs-lookup"><span data-stu-id="319f4-137">Not supported.</span></span> |
| <span data-ttu-id="319f4-138">应用程序</span><span class="sxs-lookup"><span data-stu-id="319f4-138">Application</span></span> | <span data-ttu-id="319f4-139">不支持。</span><span class="sxs-lookup"><span data-stu-id="319f4-139">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="319f4-140">Azure AD</span><span class="sxs-lookup"><span data-stu-id="319f4-140">Azure AD</span></span>

| <span data-ttu-id="319f4-141">权限类型</span><span class="sxs-lookup"><span data-stu-id="319f4-141">Permission type</span></span> | <span data-ttu-id="319f4-142">权限</span><span class="sxs-lookup"><span data-stu-id="319f4-142">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="319f4-143">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="319f4-143">Delegated (work or school account)</span></span> | <span data-ttu-id="319f4-144">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="319f4-144">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="319f4-145">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="319f4-145">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="319f4-146">不支持。</span><span class="sxs-lookup"><span data-stu-id="319f4-146">Not supported.</span></span> |
| <span data-ttu-id="319f4-147">应用程序</span><span class="sxs-lookup"><span data-stu-id="319f4-147">Application</span></span> | <span data-ttu-id="319f4-148">不支持。</span><span class="sxs-lookup"><span data-stu-id="319f4-148">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="319f4-149">组</span><span class="sxs-lookup"><span data-stu-id="319f4-149">Groups</span></span>

|<span data-ttu-id="319f4-150">权限类型</span><span class="sxs-lookup"><span data-stu-id="319f4-150">Permission type</span></span> | <span data-ttu-id="319f4-151">权限</span><span class="sxs-lookup"><span data-stu-id="319f4-151">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="319f4-152">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="319f4-152">Delegated (work or school account)</span></span> | <span data-ttu-id="319f4-153">PrivilegedAccess AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="319f4-153">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="319f4-154">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="319f4-154">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="319f4-155">不支持。</span><span class="sxs-lookup"><span data-stu-id="319f4-155">Not supported.</span></span> |
| <span data-ttu-id="319f4-156">应用程序</span><span class="sxs-lookup"><span data-stu-id="319f4-156">Application</span></span> | <span data-ttu-id="319f4-157">不支持。</span><span class="sxs-lookup"><span data-stu-id="319f4-157">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="319f4-158">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="319f4-158">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="319f4-159">请求标头</span><span class="sxs-lookup"><span data-stu-id="319f4-159">Request headers</span></span>

| <span data-ttu-id="319f4-160">名称</span><span class="sxs-lookup"><span data-stu-id="319f4-160">Name</span></span>          | <span data-ttu-id="319f4-161">说明</span><span class="sxs-lookup"><span data-stu-id="319f4-161">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="319f4-162">Authorization</span><span class="sxs-lookup"><span data-stu-id="319f4-162">Authorization</span></span> | <span data-ttu-id="319f4-163">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="319f4-163">Bearer {code}</span></span>    |
| <span data-ttu-id="319f4-164">Content-type</span><span class="sxs-lookup"><span data-stu-id="319f4-164">Content-type</span></span>  | <span data-ttu-id="319f4-165">application/json</span><span class="sxs-lookup"><span data-stu-id="319f4-165">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="319f4-166">请求正文</span><span class="sxs-lookup"><span data-stu-id="319f4-166">Request body</span></span>

<span data-ttu-id="319f4-167">在请求正文中，提供 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="319f4-167">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="319f4-168">属性</span><span class="sxs-lookup"><span data-stu-id="319f4-168">Property</span></span>         | <span data-ttu-id="319f4-169">类型</span><span class="sxs-lookup"><span data-stu-id="319f4-169">Type</span></span>                                                     | <span data-ttu-id="319f4-170">说明</span><span class="sxs-lookup"><span data-stu-id="319f4-170">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="319f4-171">resourceId</span><span class="sxs-lookup"><span data-stu-id="319f4-171">resourceId</span></span>       | <span data-ttu-id="319f4-172">String</span><span class="sxs-lookup"><span data-stu-id="319f4-172">String</span></span>                                                   | <span data-ttu-id="319f4-173">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="319f4-173">The ID of the resource.</span></span> <span data-ttu-id="319f4-174">必需。</span><span class="sxs-lookup"><span data-stu-id="319f4-174">Required.</span></span> |
| <span data-ttu-id="319f4-175">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="319f4-175">roleDefinitionId</span></span> | <span data-ttu-id="319f4-176">String</span><span class="sxs-lookup"><span data-stu-id="319f4-176">String</span></span>                                                   | <span data-ttu-id="319f4-177">角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="319f4-177">The ID of the role definition.</span></span> <span data-ttu-id="319f4-178">必需。</span><span class="sxs-lookup"><span data-stu-id="319f4-178">Required.</span></span> |
| <span data-ttu-id="319f4-179">subjectId</span><span class="sxs-lookup"><span data-stu-id="319f4-179">subjectId</span></span>        | <span data-ttu-id="319f4-180">String</span><span class="sxs-lookup"><span data-stu-id="319f4-180">String</span></span>                                                   | <span data-ttu-id="319f4-181">主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="319f4-181">The ID of the subject.</span></span> <span data-ttu-id="319f4-182">必需。</span><span class="sxs-lookup"><span data-stu-id="319f4-182">Required.</span></span> |
| <span data-ttu-id="319f4-183">assignmentState</span><span class="sxs-lookup"><span data-stu-id="319f4-183">assignmentState</span></span>  | <span data-ttu-id="319f4-184">String</span><span class="sxs-lookup"><span data-stu-id="319f4-184">String</span></span>                                                   | <span data-ttu-id="319f4-185">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="319f4-185">The state of assignment.</span></span> <span data-ttu-id="319f4-186">值可以是 `Eligible` 和 `Active` 。</span><span class="sxs-lookup"><span data-stu-id="319f4-186">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="319f4-187">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="319f4-187">Required.</span></span> |
| <span data-ttu-id="319f4-188">type</span><span class="sxs-lookup"><span data-stu-id="319f4-188">type</span></span>             | <span data-ttu-id="319f4-189">String</span><span class="sxs-lookup"><span data-stu-id="319f4-189">String</span></span>                                                   | <span data-ttu-id="319f4-190">请求类型。</span><span class="sxs-lookup"><span data-stu-id="319f4-190">The request type.</span></span> <span data-ttu-id="319f4-191">值可以是、、、、、、 `AdminAdd` `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew` `AdminRenew` 和 `AdminExtend` 。</span><span class="sxs-lookup"><span data-stu-id="319f4-191">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="319f4-192">必需。</span><span class="sxs-lookup"><span data-stu-id="319f4-192">Required.</span></span> |
| <span data-ttu-id="319f4-193">reason</span><span class="sxs-lookup"><span data-stu-id="319f4-193">reason</span></span>           | <span data-ttu-id="319f4-194">String</span><span class="sxs-lookup"><span data-stu-id="319f4-194">String</span></span>                                                   | <span data-ttu-id="319f4-195">需要为角色分配请求提供审核和审阅目的的原因。</span><span class="sxs-lookup"><span data-stu-id="319f4-195">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="319f4-196">schedule</span><span class="sxs-lookup"><span data-stu-id="319f4-196">schedule</span></span>         | [<span data-ttu-id="319f4-197">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="319f4-197">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="319f4-198">角色分配请求的日程安排。</span><span class="sxs-lookup"><span data-stu-id="319f4-198">The schedule of the role assignment request.</span></span> <span data-ttu-id="319f4-199">对于的请求类型 `UserAdd` ， `AdminAdd` 、 `AdminUpdate` 和， `AdminExtend` 它是必需的。</span><span class="sxs-lookup"><span data-stu-id="319f4-199">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="319f4-200">响应</span><span class="sxs-lookup"><span data-stu-id="319f4-200">Response</span></span>

<span data-ttu-id="319f4-201">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="319f4-201">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="319f4-202">错误代码</span><span class="sxs-lookup"><span data-stu-id="319f4-202">Error codes</span></span>

<span data-ttu-id="319f4-203">此 API 返回标准的 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="319f4-203">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="319f4-204">此外，它还返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="319f4-204">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="319f4-205">错误代码</span><span class="sxs-lookup"><span data-stu-id="319f4-205">Error code</span></span>     | <span data-ttu-id="319f4-206">错误消息</span><span class="sxs-lookup"><span data-stu-id="319f4-206">Error message</span></span>                               | <span data-ttu-id="319f4-207">详细信息</span><span class="sxs-lookup"><span data-stu-id="319f4-207">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="319f4-208">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="319f4-208">400 BadRequest</span></span> | <span data-ttu-id="319f4-209">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="319f4-209">RoleNotFound</span></span>                                | <span data-ttu-id="319f4-210">`roleDefinitionId`找不到请求正文中提供的。</span><span class="sxs-lookup"><span data-stu-id="319f4-210">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="319f4-211">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="319f4-211">400 BadRequest</span></span> | <span data-ttu-id="319f4-212">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="319f4-212">ResourceIsLocked</span></span>                            | <span data-ttu-id="319f4-213">请求正文中提供的资源处于状态 `Locked` ，并且无法创建角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="319f4-213">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="319f4-214">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="319f4-214">400 BadRequest</span></span> | <span data-ttu-id="319f4-215">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="319f4-215">SubjectNotFound</span></span>                             | <span data-ttu-id="319f4-216">`subjectId`找不到请求正文中提供的。</span><span class="sxs-lookup"><span data-stu-id="319f4-216">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="319f4-217">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="319f4-217">400 BadRequest</span></span> | <span data-ttu-id="319f4-218">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="319f4-218">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="319f4-219">系统中已存在一个挂起的 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 。</span><span class="sxs-lookup"><span data-stu-id="319f4-219">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="319f4-220">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="319f4-220">400 BadRequest</span></span> | <span data-ttu-id="319f4-221">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="319f4-221">RoleAssignmentExists</span></span>                        | <span data-ttu-id="319f4-222">系统中已存在请求创建的 [governanceRoleAssignment](../resources/governanceroleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="319f4-222">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="319f4-223">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="319f4-223">400 BadRequest</span></span> | <span data-ttu-id="319f4-224">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="319f4-224">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="319f4-225">系统中不存在请求进行更新/扩展的 [governanceRoleAssignment](../resources/governanceroleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="319f4-225">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="319f4-226">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="319f4-226">400 BadRequest</span></span> | <span data-ttu-id="319f4-227">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="319f4-227">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="319f4-228">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)不符合内部策略，因此无法创建。</span><span class="sxs-lookup"><span data-stu-id="319f4-228">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="319f4-229">示例</span><span class="sxs-lookup"><span data-stu-id="319f4-229">Examples</span></span>

<span data-ttu-id="319f4-230">下面的示例演示如何使用此 API。</span><span class="sxs-lookup"><span data-stu-id="319f4-230">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="319f4-231">示例1：管理员为用户分配角色</span><span class="sxs-lookup"><span data-stu-id="319f4-231">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="319f4-232">在此示例中，管理员向计费读者角色分配用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="319f4-232">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="319f4-233">**注意：** 除了权限之外，本示例还要求请求者在资源上至少有一个 `Active` 管理员角色分配 (`owner` 或 `user access administrator`) 。</span><span class="sxs-lookup"><span data-stu-id="319f4-233">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="319f4-234">属性</span><span class="sxs-lookup"><span data-stu-id="319f4-234">Property</span></span>         | <span data-ttu-id="319f4-235">类型</span><span class="sxs-lookup"><span data-stu-id="319f4-235">Type</span></span>                                                     | <span data-ttu-id="319f4-236">必需</span><span class="sxs-lookup"><span data-stu-id="319f4-236">Required</span></span>                 | <span data-ttu-id="319f4-237">值</span><span class="sxs-lookup"><span data-stu-id="319f4-237">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="319f4-238">resourceId</span><span class="sxs-lookup"><span data-stu-id="319f4-238">resourceId</span></span>       | <span data-ttu-id="319f4-239">String</span><span class="sxs-lookup"><span data-stu-id="319f4-239">String</span></span>                                                   | <span data-ttu-id="319f4-240">是</span><span class="sxs-lookup"><span data-stu-id="319f4-240">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="319f4-241">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="319f4-241">roleDefinitionId</span></span> | <span data-ttu-id="319f4-242">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-242">String</span></span>                                                   | <span data-ttu-id="319f4-243">是</span><span class="sxs-lookup"><span data-stu-id="319f4-243">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="319f4-244">subjectId</span><span class="sxs-lookup"><span data-stu-id="319f4-244">subjectId</span></span>        | <span data-ttu-id="319f4-245">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-245">String</span></span>                                                   | <span data-ttu-id="319f4-246">是</span><span class="sxs-lookup"><span data-stu-id="319f4-246">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="319f4-247">assignmentState</span><span class="sxs-lookup"><span data-stu-id="319f4-247">assignmentState</span></span>  | <span data-ttu-id="319f4-248">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-248">String</span></span>                                                   | <span data-ttu-id="319f4-249">是</span><span class="sxs-lookup"><span data-stu-id="319f4-249">Yes</span></span>                      | <span data-ttu-id="319f4-250">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="319f4-250">Eligible / Active</span></span> |
| <span data-ttu-id="319f4-251">type</span><span class="sxs-lookup"><span data-stu-id="319f4-251">type</span></span>             | <span data-ttu-id="319f4-252">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-252">String</span></span>                                                   | <span data-ttu-id="319f4-253">是</span><span class="sxs-lookup"><span data-stu-id="319f4-253">Yes</span></span>                      | <span data-ttu-id="319f4-254">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="319f4-254">AdminAdd</span></span> |
| <span data-ttu-id="319f4-255">reason</span><span class="sxs-lookup"><span data-stu-id="319f4-255">reason</span></span>           | <span data-ttu-id="319f4-256">String</span><span class="sxs-lookup"><span data-stu-id="319f4-256">String</span></span>                                                   | <span data-ttu-id="319f4-257">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="319f4-257">depends on role Settings</span></span> |   |
| <span data-ttu-id="319f4-258">schedule</span><span class="sxs-lookup"><span data-stu-id="319f4-258">schedule</span></span>         | [<span data-ttu-id="319f4-259">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="319f4-259">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="319f4-260">是</span><span class="sxs-lookup"><span data-stu-id="319f4-260">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="319f4-261">请求</span><span class="sxs-lookup"><span data-stu-id="319f4-261">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="319f4-262">HTTP</span><span class="sxs-lookup"><span data-stu-id="319f4-262">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="319f4-263">C#</span><span class="sxs-lookup"><span data-stu-id="319f4-263">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="319f4-264">JavaScript</span><span class="sxs-lookup"><span data-stu-id="319f4-264">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="319f4-265">Objective-C</span><span class="sxs-lookup"><span data-stu-id="319f4-265">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="319f4-266">响应</span><span class="sxs-lookup"><span data-stu-id="319f4-266">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="319f4-267">示例2：用户激活符合条件的角色</span><span class="sxs-lookup"><span data-stu-id="319f4-267">Example 2: User activates eligible role</span></span>

<span data-ttu-id="319f4-268">在此示例中，用户 nawu@fimdev.net 激活符合条件的计费阅读者角色。</span><span class="sxs-lookup"><span data-stu-id="319f4-268">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="319f4-269">属性</span><span class="sxs-lookup"><span data-stu-id="319f4-269">Property</span></span>         | <span data-ttu-id="319f4-270">类型</span><span class="sxs-lookup"><span data-stu-id="319f4-270">Type</span></span>                                                     | <span data-ttu-id="319f4-271">必需</span><span class="sxs-lookup"><span data-stu-id="319f4-271">Required</span></span>                 | <span data-ttu-id="319f4-272">值</span><span class="sxs-lookup"><span data-stu-id="319f4-272">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="319f4-273">resourceId</span><span class="sxs-lookup"><span data-stu-id="319f4-273">resourceId</span></span>       | <span data-ttu-id="319f4-274">String</span><span class="sxs-lookup"><span data-stu-id="319f4-274">String</span></span>                                                   | <span data-ttu-id="319f4-275">是</span><span class="sxs-lookup"><span data-stu-id="319f4-275">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="319f4-276">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="319f4-276">roleDefinitionId</span></span> | <span data-ttu-id="319f4-277">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-277">String</span></span>                                                   | <span data-ttu-id="319f4-278">是</span><span class="sxs-lookup"><span data-stu-id="319f4-278">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="319f4-279">subjectId</span><span class="sxs-lookup"><span data-stu-id="319f4-279">subjectId</span></span>        | <span data-ttu-id="319f4-280">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-280">String</span></span>                                                   | <span data-ttu-id="319f4-281">是</span><span class="sxs-lookup"><span data-stu-id="319f4-281">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="319f4-282">assignmentState</span><span class="sxs-lookup"><span data-stu-id="319f4-282">assignmentState</span></span>  | <span data-ttu-id="319f4-283">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-283">String</span></span>                                                   | <span data-ttu-id="319f4-284">是</span><span class="sxs-lookup"><span data-stu-id="319f4-284">Yes</span></span>                      | <span data-ttu-id="319f4-285">活动</span><span class="sxs-lookup"><span data-stu-id="319f4-285">Active</span></span> |
| <span data-ttu-id="319f4-286">type</span><span class="sxs-lookup"><span data-stu-id="319f4-286">type</span></span>             | <span data-ttu-id="319f4-287">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-287">String</span></span>                                                   | <span data-ttu-id="319f4-288">是</span><span class="sxs-lookup"><span data-stu-id="319f4-288">Yes</span></span>                      | <span data-ttu-id="319f4-289">UserAdd</span><span class="sxs-lookup"><span data-stu-id="319f4-289">UserAdd</span></span> |
| <span data-ttu-id="319f4-290">reason</span><span class="sxs-lookup"><span data-stu-id="319f4-290">reason</span></span>           | <span data-ttu-id="319f4-291">String</span><span class="sxs-lookup"><span data-stu-id="319f4-291">String</span></span>                                                   | <span data-ttu-id="319f4-292">取决于角色设置</span><span class="sxs-lookup"><span data-stu-id="319f4-292">depends on role Settings</span></span> |   |
| <span data-ttu-id="319f4-293">schedule</span><span class="sxs-lookup"><span data-stu-id="319f4-293">schedule</span></span>         | [<span data-ttu-id="319f4-294">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="319f4-294">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="319f4-295">是</span><span class="sxs-lookup"><span data-stu-id="319f4-295">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="319f4-296">请求</span><span class="sxs-lookup"><span data-stu-id="319f4-296">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="319f4-297">响应</span><span class="sxs-lookup"><span data-stu-id="319f4-297">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="319f4-298">示例3：用户停用分配的角色</span><span class="sxs-lookup"><span data-stu-id="319f4-298">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="319f4-299">在此示例中，用户 nawu@fimdev.net 停用活动的帐单阅读者角色。</span><span class="sxs-lookup"><span data-stu-id="319f4-299">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="319f4-300">属性</span><span class="sxs-lookup"><span data-stu-id="319f4-300">Property</span></span>         | <span data-ttu-id="319f4-301">类型</span><span class="sxs-lookup"><span data-stu-id="319f4-301">Type</span></span>                                                     | <span data-ttu-id="319f4-302">必需</span><span class="sxs-lookup"><span data-stu-id="319f4-302">Required</span></span> | <span data-ttu-id="319f4-303">值</span><span class="sxs-lookup"><span data-stu-id="319f4-303">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="319f4-304">resourceId</span><span class="sxs-lookup"><span data-stu-id="319f4-304">resourceId</span></span>       | <span data-ttu-id="319f4-305">String</span><span class="sxs-lookup"><span data-stu-id="319f4-305">String</span></span>                                                   | <span data-ttu-id="319f4-306">是</span><span class="sxs-lookup"><span data-stu-id="319f4-306">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="319f4-307">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="319f4-307">roleDefinitionId</span></span> | <span data-ttu-id="319f4-308">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-308">String</span></span>                                                   | <span data-ttu-id="319f4-309">是</span><span class="sxs-lookup"><span data-stu-id="319f4-309">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="319f4-310">subjectId</span><span class="sxs-lookup"><span data-stu-id="319f4-310">subjectId</span></span>        | <span data-ttu-id="319f4-311">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-311">String</span></span>                                                   | <span data-ttu-id="319f4-312">是</span><span class="sxs-lookup"><span data-stu-id="319f4-312">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="319f4-313">assignmentState</span><span class="sxs-lookup"><span data-stu-id="319f4-313">assignmentState</span></span>  | <span data-ttu-id="319f4-314">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-314">String</span></span>                                                   | <span data-ttu-id="319f4-315">是</span><span class="sxs-lookup"><span data-stu-id="319f4-315">Yes</span></span>      | <span data-ttu-id="319f4-316">活动</span><span class="sxs-lookup"><span data-stu-id="319f4-316">Active</span></span> |
| <span data-ttu-id="319f4-317">type</span><span class="sxs-lookup"><span data-stu-id="319f4-317">type</span></span>             | <span data-ttu-id="319f4-318">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-318">String</span></span>                                                   | <span data-ttu-id="319f4-319">是</span><span class="sxs-lookup"><span data-stu-id="319f4-319">Yes</span></span>      | <span data-ttu-id="319f4-320">UserRemove</span><span class="sxs-lookup"><span data-stu-id="319f4-320">UserRemove</span></span> |
| <span data-ttu-id="319f4-321">reason</span><span class="sxs-lookup"><span data-stu-id="319f4-321">reason</span></span>           | <span data-ttu-id="319f4-322">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-322">String</span></span>                                                   | <span data-ttu-id="319f4-323">否</span><span class="sxs-lookup"><span data-stu-id="319f4-323">No</span></span>       |   |
| <span data-ttu-id="319f4-324">schedule</span><span class="sxs-lookup"><span data-stu-id="319f4-324">schedule</span></span>         | [<span data-ttu-id="319f4-325">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="319f4-325">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="319f4-326">否</span><span class="sxs-lookup"><span data-stu-id="319f4-326">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="319f4-327">请求</span><span class="sxs-lookup"><span data-stu-id="319f4-327">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="319f4-328">响应</span><span class="sxs-lookup"><span data-stu-id="319f4-328">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="319f4-329">示例4：管理员从角色中删除用户</span><span class="sxs-lookup"><span data-stu-id="319f4-329">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="319f4-330">在此示例中，管理员从 "计费读者" 角色中删除用户 nawu@fimdev.net。</span><span class="sxs-lookup"><span data-stu-id="319f4-330">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="319f4-331">**注意：** 除了权限之外，本示例还要求请求者在资源上至少有一个 `Active` 管理员角色分配 (`owner` 或 `user access administrator`) 。</span><span class="sxs-lookup"><span data-stu-id="319f4-331">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="319f4-332">属性</span><span class="sxs-lookup"><span data-stu-id="319f4-332">Property</span></span>         | <span data-ttu-id="319f4-333">类型</span><span class="sxs-lookup"><span data-stu-id="319f4-333">Type</span></span>                                                     | <span data-ttu-id="319f4-334">必需</span><span class="sxs-lookup"><span data-stu-id="319f4-334">Required</span></span> | <span data-ttu-id="319f4-335">值</span><span class="sxs-lookup"><span data-stu-id="319f4-335">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="319f4-336">resourceId</span><span class="sxs-lookup"><span data-stu-id="319f4-336">resourceId</span></span>       | <span data-ttu-id="319f4-337">String</span><span class="sxs-lookup"><span data-stu-id="319f4-337">String</span></span>                                                   | <span data-ttu-id="319f4-338">是</span><span class="sxs-lookup"><span data-stu-id="319f4-338">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="319f4-339">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="319f4-339">roleDefinitionId</span></span> | <span data-ttu-id="319f4-340">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-340">String</span></span>                                                   | <span data-ttu-id="319f4-341">是</span><span class="sxs-lookup"><span data-stu-id="319f4-341">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="319f4-342">subjectId</span><span class="sxs-lookup"><span data-stu-id="319f4-342">subjectId</span></span>        | <span data-ttu-id="319f4-343">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-343">String</span></span>                                                   | <span data-ttu-id="319f4-344">是</span><span class="sxs-lookup"><span data-stu-id="319f4-344">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="319f4-345">assignmentState</span><span class="sxs-lookup"><span data-stu-id="319f4-345">assignmentState</span></span>  | <span data-ttu-id="319f4-346">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-346">String</span></span>                                                   | <span data-ttu-id="319f4-347">是</span><span class="sxs-lookup"><span data-stu-id="319f4-347">Yes</span></span>      | <span data-ttu-id="319f4-348">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="319f4-348">Eligible / Active</span></span> |
| <span data-ttu-id="319f4-349">type</span><span class="sxs-lookup"><span data-stu-id="319f4-349">type</span></span>             | <span data-ttu-id="319f4-350">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-350">String</span></span>                                                   | <span data-ttu-id="319f4-351">是</span><span class="sxs-lookup"><span data-stu-id="319f4-351">Yes</span></span>      | <span data-ttu-id="319f4-352">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="319f4-352">AdminRemove</span></span> |
| <span data-ttu-id="319f4-353">reason</span><span class="sxs-lookup"><span data-stu-id="319f4-353">reason</span></span>           | <span data-ttu-id="319f4-354">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-354">String</span></span>                                                   | <span data-ttu-id="319f4-355">否</span><span class="sxs-lookup"><span data-stu-id="319f4-355">No</span></span>       |   |
| <span data-ttu-id="319f4-356">schedule</span><span class="sxs-lookup"><span data-stu-id="319f4-356">schedule</span></span>         | [<span data-ttu-id="319f4-357">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="319f4-357">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="319f4-358">否</span><span class="sxs-lookup"><span data-stu-id="319f4-358">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="319f4-359">请求</span><span class="sxs-lookup"><span data-stu-id="319f4-359">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="319f4-360">响应</span><span class="sxs-lookup"><span data-stu-id="319f4-360">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="319f4-361">示例5：管理员更新角色分配</span><span class="sxs-lookup"><span data-stu-id="319f4-361">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="319f4-362">在此示例中，管理员将用户 nawu@fimdev.net 的角色分配更新为 "所有者"。</span><span class="sxs-lookup"><span data-stu-id="319f4-362">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="319f4-363">**注意：** 除了权限之外，本示例还要求请求者在资源上至少有一个 `Active` 管理员角色分配 (`owner` 或 `user access administrator`) 。</span><span class="sxs-lookup"><span data-stu-id="319f4-363">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="319f4-364">属性</span><span class="sxs-lookup"><span data-stu-id="319f4-364">Property</span></span>         | <span data-ttu-id="319f4-365">类型</span><span class="sxs-lookup"><span data-stu-id="319f4-365">Type</span></span>                                                     | <span data-ttu-id="319f4-366">必需</span><span class="sxs-lookup"><span data-stu-id="319f4-366">Required</span></span>                | <span data-ttu-id="319f4-367">值</span><span class="sxs-lookup"><span data-stu-id="319f4-367">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="319f4-368">resourceId</span><span class="sxs-lookup"><span data-stu-id="319f4-368">resourceId</span></span>       | <span data-ttu-id="319f4-369">String</span><span class="sxs-lookup"><span data-stu-id="319f4-369">String</span></span>                                                   | <span data-ttu-id="319f4-370">是</span><span class="sxs-lookup"><span data-stu-id="319f4-370">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="319f4-371">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="319f4-371">roleDefinitionId</span></span> | <span data-ttu-id="319f4-372">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-372">String</span></span>                                                   | <span data-ttu-id="319f4-373">是</span><span class="sxs-lookup"><span data-stu-id="319f4-373">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="319f4-374">subjectId</span><span class="sxs-lookup"><span data-stu-id="319f4-374">subjectId</span></span>        | <span data-ttu-id="319f4-375">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-375">String</span></span>                                                   | <span data-ttu-id="319f4-376">是</span><span class="sxs-lookup"><span data-stu-id="319f4-376">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="319f4-377">assignmentState</span><span class="sxs-lookup"><span data-stu-id="319f4-377">assignmentState</span></span>  | <span data-ttu-id="319f4-378">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-378">String</span></span>                                                   | <span data-ttu-id="319f4-379">是</span><span class="sxs-lookup"><span data-stu-id="319f4-379">Yes</span></span>                     | <span data-ttu-id="319f4-380">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="319f4-380">Eligible / Active</span></span> |
| <span data-ttu-id="319f4-381">type</span><span class="sxs-lookup"><span data-stu-id="319f4-381">type</span></span>             | <span data-ttu-id="319f4-382">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-382">String</span></span>                                                   | <span data-ttu-id="319f4-383">是</span><span class="sxs-lookup"><span data-stu-id="319f4-383">Yes</span></span>                     | <span data-ttu-id="319f4-384">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="319f4-384">AdminUpdate</span></span> |
| <span data-ttu-id="319f4-385">reason</span><span class="sxs-lookup"><span data-stu-id="319f4-385">reason</span></span>           | <span data-ttu-id="319f4-386">String</span><span class="sxs-lookup"><span data-stu-id="319f4-386">String</span></span>                                                   | <span data-ttu-id="319f4-387">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="319f4-387">depends on roleSettings</span></span> |   |
| <span data-ttu-id="319f4-388">schedule</span><span class="sxs-lookup"><span data-stu-id="319f4-388">schedule</span></span>         | [<span data-ttu-id="319f4-389">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="319f4-389">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="319f4-390">是</span><span class="sxs-lookup"><span data-stu-id="319f4-390">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="319f4-391">请求</span><span class="sxs-lookup"><span data-stu-id="319f4-391">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="319f4-392">响应</span><span class="sxs-lookup"><span data-stu-id="319f4-392">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="319f4-393">示例6：管理员扩展了即将过期的角色分配</span><span class="sxs-lookup"><span data-stu-id="319f4-393">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="319f4-394">此示例将用户 ANUJCUSER 的过期角色分配扩展到 API Management Service 参与者。</span><span class="sxs-lookup"><span data-stu-id="319f4-394">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="319f4-395">**注意：** 除了权限之外，本示例还要求请求者在资源上至少有一个 `Active` 管理员角色分配 (`owner` 或 `user access administrator`) 。</span><span class="sxs-lookup"><span data-stu-id="319f4-395">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="319f4-396">属性</span><span class="sxs-lookup"><span data-stu-id="319f4-396">Property</span></span>         | <span data-ttu-id="319f4-397">类型</span><span class="sxs-lookup"><span data-stu-id="319f4-397">Type</span></span>                                                     | <span data-ttu-id="319f4-398">必需</span><span class="sxs-lookup"><span data-stu-id="319f4-398">Required</span></span>                | <span data-ttu-id="319f4-399">值</span><span class="sxs-lookup"><span data-stu-id="319f4-399">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="319f4-400">resourceId</span><span class="sxs-lookup"><span data-stu-id="319f4-400">resourceId</span></span>       | <span data-ttu-id="319f4-401">String</span><span class="sxs-lookup"><span data-stu-id="319f4-401">String</span></span>                                                   | <span data-ttu-id="319f4-402">是</span><span class="sxs-lookup"><span data-stu-id="319f4-402">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="319f4-403">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="319f4-403">roleDefinitionId</span></span> | <span data-ttu-id="319f4-404">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-404">String</span></span>                                                   | <span data-ttu-id="319f4-405">是</span><span class="sxs-lookup"><span data-stu-id="319f4-405">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="319f4-406">subjectId</span><span class="sxs-lookup"><span data-stu-id="319f4-406">subjectId</span></span>        | <span data-ttu-id="319f4-407">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-407">String</span></span>                                                   | <span data-ttu-id="319f4-408">是</span><span class="sxs-lookup"><span data-stu-id="319f4-408">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="319f4-409">assignmentState</span><span class="sxs-lookup"><span data-stu-id="319f4-409">assignmentState</span></span>  | <span data-ttu-id="319f4-410">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-410">String</span></span>                                                   | <span data-ttu-id="319f4-411">是</span><span class="sxs-lookup"><span data-stu-id="319f4-411">Yes</span></span>                     | <span data-ttu-id="319f4-412">符合条件/活动</span><span class="sxs-lookup"><span data-stu-id="319f4-412">Eligible / Active</span></span> |
| <span data-ttu-id="319f4-413">type</span><span class="sxs-lookup"><span data-stu-id="319f4-413">type</span></span>             | <span data-ttu-id="319f4-414">字符串</span><span class="sxs-lookup"><span data-stu-id="319f4-414">String</span></span>                                                   | <span data-ttu-id="319f4-415">是</span><span class="sxs-lookup"><span data-stu-id="319f4-415">Yes</span></span>                     | <span data-ttu-id="319f4-416">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="319f4-416">AdminExtend</span></span> |
| <span data-ttu-id="319f4-417">reason</span><span class="sxs-lookup"><span data-stu-id="319f4-417">reason</span></span>           | <span data-ttu-id="319f4-418">String</span><span class="sxs-lookup"><span data-stu-id="319f4-418">String</span></span>                                                   | <span data-ttu-id="319f4-419">取决于 roleSettings</span><span class="sxs-lookup"><span data-stu-id="319f4-419">depends on roleSettings</span></span> |   |
| <span data-ttu-id="319f4-420">schedule</span><span class="sxs-lookup"><span data-stu-id="319f4-420">schedule</span></span>         | [<span data-ttu-id="319f4-421">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="319f4-421">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="319f4-422">是</span><span class="sxs-lookup"><span data-stu-id="319f4-422">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="319f4-423">请求</span><span class="sxs-lookup"><span data-stu-id="319f4-423">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="319f4-424">响应</span><span class="sxs-lookup"><span data-stu-id="319f4-424">Response</span></span>

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


