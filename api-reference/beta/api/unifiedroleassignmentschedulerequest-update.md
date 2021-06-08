---
title: 更新 unifiedRoleAssignmentScheduleRequest
description: 更新 unifiedRoleAssignmentScheduleRequest 对象的属性。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1e83981246974cb785b9792b08a04866366cf2dc
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786444"
---
# <a name="update-unifiedroleassignmentschedulerequest"></a><span data-ttu-id="2b6c7-103">更新 unifiedRoleAssignmentScheduleRequest</span><span class="sxs-lookup"><span data-stu-id="2b6c7-103">Update unifiedRoleAssignmentScheduleRequest</span></span>
<span data-ttu-id="2b6c7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b6c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b6c7-105">更新 [unifiedRoleAssignmentScheduleRequest 对象](../resources/unifiedroleassignmentschedulerequest.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-105">Update the properties of an [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b6c7-106">权限</span><span class="sxs-lookup"><span data-stu-id="2b6c7-106">Permissions</span></span>
<span data-ttu-id="2b6c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b6c7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b6c7-109">Permission type</span></span>|<span data-ttu-id="2b6c7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b6c7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b6c7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b6c7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2b6c7-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="2b6c7-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="2b6c7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b6c7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b6c7-114">不支持</span><span class="sxs-lookup"><span data-stu-id="2b6c7-114">Not supported</span></span>|
|<span data-ttu-id="2b6c7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b6c7-115">Application</span></span>|<span data-ttu-id="2b6c7-116">不支持</span><span class="sxs-lookup"><span data-stu-id="2b6c7-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b6c7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b6c7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}
```

## <a name="request-headers"></a><span data-ttu-id="2b6c7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b6c7-118">Request headers</span></span>
|<span data-ttu-id="2b6c7-119">名称</span><span class="sxs-lookup"><span data-stu-id="2b6c7-119">Name</span></span>|<span data-ttu-id="2b6c7-120">说明</span><span class="sxs-lookup"><span data-stu-id="2b6c7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2b6c7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b6c7-121">Authorization</span></span>|<span data-ttu-id="2b6c7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2b6c7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b6c7-124">Content-Type</span></span>|<span data-ttu-id="2b6c7-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2b6c7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b6c7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b6c7-127">Request body</span></span>
<span data-ttu-id="2b6c7-128">在请求正文中，提供 [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-128">In the request body, supply a JSON representation of the [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) object.</span></span>

<span data-ttu-id="2b6c7-129">下表显示更新 [unifiedRoleAssignmentScheduleRequest 时所需的属性](../resources/unifiedroleassignmentschedulerequest.md)。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-129">The following table shows the properties that are required when you update the [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md).</span></span>

|<span data-ttu-id="2b6c7-130">属性</span><span class="sxs-lookup"><span data-stu-id="2b6c7-130">Property</span></span>|<span data-ttu-id="2b6c7-131">类型</span><span class="sxs-lookup"><span data-stu-id="2b6c7-131">Type</span></span>|<span data-ttu-id="2b6c7-132">说明</span><span class="sxs-lookup"><span data-stu-id="2b6c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b6c7-133">id</span><span class="sxs-lookup"><span data-stu-id="2b6c7-133">id</span></span>|<span data-ttu-id="2b6c7-134">String</span><span class="sxs-lookup"><span data-stu-id="2b6c7-134">String</span></span>|<span data-ttu-id="2b6c7-135">unifiedRoleAssignmentScheduleRequest 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-135">The unique identifier for the unifiedRoleAssignmentScheduleRequest.</span></span> <span data-ttu-id="2b6c7-136">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-136">Key, not nullable, Read-only.</span></span>|
|<span data-ttu-id="2b6c7-137">action</span><span class="sxs-lookup"><span data-stu-id="2b6c7-137">action</span></span>|<span data-ttu-id="2b6c7-138">String</span><span class="sxs-lookup"><span data-stu-id="2b6c7-138">String</span></span>|<span data-ttu-id="2b6c7-139">表示对项目执行的操作角色分配。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-139">Representing the type of the operation on the role assignment.</span></span> <span data-ttu-id="2b6c7-140">值可以是</span><span class="sxs-lookup"><span data-stu-id="2b6c7-140">The value can be</span></span> <ul><li><span data-ttu-id="2b6c7-141">`AdminAdd`：管理员将用户/组分配给角色;</span><span class="sxs-lookup"><span data-stu-id="2b6c7-141">`AdminAdd`: Administrators assign users/groups to roles;</span></span></li><li><span data-ttu-id="2b6c7-142">`UserAdd`：用户激活符合条件的分配;</span><span class="sxs-lookup"><span data-stu-id="2b6c7-142">`UserAdd`: Users activate eligible assignments;</span></span></li><li> <span data-ttu-id="2b6c7-143">`AdminUpdate`：管理员更改现有角色分配</span><span class="sxs-lookup"><span data-stu-id="2b6c7-143">`AdminUpdate`: Administrators change existing role assignments</span></span></li><li><span data-ttu-id="2b6c7-144">`AdminRemove`：管理员从角色中删除用户/组;</span><span class="sxs-lookup"><span data-stu-id="2b6c7-144">`AdminRemove`: Administrators remove users/groups from roles;</span></span><li><span data-ttu-id="2b6c7-145">`UserRemove`：用户停用活动分配;</span><span class="sxs-lookup"><span data-stu-id="2b6c7-145">`UserRemove`: Users deactivate active assignments;</span></span><li><span data-ttu-id="2b6c7-146">`UserExtend`：用户请求延长其过期分配;</span><span class="sxs-lookup"><span data-stu-id="2b6c7-146">`UserExtend`: Users request to extend their expiring assignments;</span></span></li><li><span data-ttu-id="2b6c7-147">`AdminExtend`：管理员扩展即将过期的工作分配。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-147">`AdminExtend`: Administrators extend expiring assignments.</span></span></li><li><span data-ttu-id="2b6c7-148">`UserRenew`：用户请求续订其已过期的工作分配;</span><span class="sxs-lookup"><span data-stu-id="2b6c7-148">`UserRenew`: Users request to renew their expired assignments;</span></span></li><li><span data-ttu-id="2b6c7-149">`AdminRenew`：管理员扩展即将过期的工作分配。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-149">`AdminRenew`: Administrators extend expiring assignments.</span></span></li></ul>|
|<span data-ttu-id="2b6c7-150">principalId</span><span class="sxs-lookup"><span data-stu-id="2b6c7-150">principalId</span></span>|<span data-ttu-id="2b6c7-151">String</span><span class="sxs-lookup"><span data-stu-id="2b6c7-151">String</span></span>|<span data-ttu-id="2b6c7-152">要授予分配的主体的 Objectid。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-152">Objectid of the principal to which the assignment is being granted to.</span></span>|
|<span data-ttu-id="2b6c7-153">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2b6c7-153">roleDefinitionId</span></span>|<span data-ttu-id="2b6c7-154">String</span><span class="sxs-lookup"><span data-stu-id="2b6c7-154">String</span></span>|<span data-ttu-id="2b6c7-155">分配所针对的 unifiedRoleDefinition 的 ID。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-155">ID of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="2b6c7-156">只读。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-156">Read only.</span></span>|
|<span data-ttu-id="2b6c7-157">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="2b6c7-157">directoryScopeId</span></span>|<span data-ttu-id="2b6c7-158">String</span><span class="sxs-lookup"><span data-stu-id="2b6c7-158">String</span></span>|<span data-ttu-id="2b6c7-159">表示工作分配范围的目录对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-159">Id of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="2b6c7-160">工作分配的范围决定了已授予主体访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-160">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="2b6c7-161">目录作用域是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="2b6c7-162">应用程序作用域是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-162">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="2b6c7-163">appScopeId</span><span class="sxs-lookup"><span data-stu-id="2b6c7-163">appScopeId</span></span>|<span data-ttu-id="2b6c7-164">String</span><span class="sxs-lookup"><span data-stu-id="2b6c7-164">String</span></span>|<span data-ttu-id="2b6c7-165">当分配范围特定于应用时，特定于应用的范围的 ID。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-165">Id of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="2b6c7-166">工作分配的范围决定了已授予主体访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-166">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="2b6c7-167">目录作用域是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-167">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="2b6c7-168">对租户范围范围使用"/"。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-168">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="2b6c7-169">应用程序作用域是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-169">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="2b6c7-170">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="2b6c7-170">isValidationOnly</span></span>|<span data-ttu-id="2b6c7-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b6c7-171">Boolean</span></span>|<span data-ttu-id="2b6c7-172">确定调用是验证还是实际调用的布尔值。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-172">A boolean that determines whether the call is a validation or an actual call.</span></span> <span data-ttu-id="2b6c7-173">仅在要检查激活是否受 MFA 等其他规则限制，然后再实际提交请求时设置此属性。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-173">Only set this property if you want to check whether an activation is subject to additional rules like MFA before actually submitting the request.</span></span>|
|<span data-ttu-id="2b6c7-174">targetScheduleId</span><span class="sxs-lookup"><span data-stu-id="2b6c7-174">targetScheduleId</span></span>|<span data-ttu-id="2b6c7-175">String</span><span class="sxs-lookup"><span data-stu-id="2b6c7-175">String</span></span>|<span data-ttu-id="2b6c7-176">附加到工作分配的计划对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-176">ID of the schedule object attached to the assignment.</span></span>|
|<span data-ttu-id="2b6c7-177">justification</span><span class="sxs-lookup"><span data-stu-id="2b6c7-177">justification</span></span>|<span data-ttu-id="2b6c7-178">String</span><span class="sxs-lookup"><span data-stu-id="2b6c7-178">String</span></span>|<span data-ttu-id="2b6c7-179">创建请求时由用户和管理员提供的消息，说明为什么需要该请求。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-179">A message provided by users and administrators when create the request about why it is needed.</span></span>|
|<span data-ttu-id="2b6c7-180">scheduleInfo</span><span class="sxs-lookup"><span data-stu-id="2b6c7-180">scheduleInfo</span></span>|[<span data-ttu-id="2b6c7-181">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="2b6c7-181">requestSchedule</span></span>](../resources/requestschedule.md)|<span data-ttu-id="2b6c7-182">请求的计划角色分配对象。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-182">The schedule object of the role assignment request.</span></span>|
|<span data-ttu-id="2b6c7-183">ticketInfo</span><span class="sxs-lookup"><span data-stu-id="2b6c7-183">ticketInfo</span></span>|[<span data-ttu-id="2b6c7-184">ticketInfo</span><span class="sxs-lookup"><span data-stu-id="2b6c7-184">ticketInfo</span></span>](../resources/ticketinfo.md)|<span data-ttu-id="2b6c7-185">附加到请求的 ticketInfo 角色分配，其中包含票证编号和票证系统的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-185">The ticketInfo object attached to the role assignment request which includes details of the ticket number and ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="2b6c7-186">响应</span><span class="sxs-lookup"><span data-stu-id="2b6c7-186">Response</span></span>

<span data-ttu-id="2b6c7-187">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-187">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2b6c7-188">示例</span><span class="sxs-lookup"><span data-stu-id="2b6c7-188">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2b6c7-189">请求</span><span class="sxs-lookup"><span data-stu-id="2b6c7-189">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2b6c7-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b6c7-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleassignmentschedulerequest"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}
Content-Type: application/json
Content-length: 466

{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentScheduleRequest",
  "action": "String",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "isValidationOnly": "Boolean",
  "targetScheduleId": "String",
  "justification": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "ticketInfo": {
    "@odata.type": "microsoft.graph.ticketInfo"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="2b6c7-191">C#</span><span class="sxs-lookup"><span data-stu-id="2b6c7-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentschedulerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b6c7-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b6c7-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentschedulerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b6c7-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b6c7-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentschedulerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b6c7-194">Java</span><span class="sxs-lookup"><span data-stu-id="2b6c7-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleassignmentschedulerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2b6c7-195">响应</span><span class="sxs-lookup"><span data-stu-id="2b6c7-195">Response</span></span>
<span data-ttu-id="2b6c7-196">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2b6c7-196">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
```http
HTTP/1.1 204 OK

```

<!--
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentScheduleRequest",
  "id": "c13ee236-e236-c13e-36e2-3ec136e23ec1",
  "action": "String",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "isValidationOnly": "Boolean",
  "targetScheduleId": "String",
  "justification": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "ticketInfo": {
    "@odata.type": "microsoft.graph.ticketInfo"
  }
}
```-->

