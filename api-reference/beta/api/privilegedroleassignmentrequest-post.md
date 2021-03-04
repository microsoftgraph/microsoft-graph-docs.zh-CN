---
title: 创建 privilegedRoleAssignmentRequest
description: 创建 privilegedroleassignmentrequest 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 8899aa70125809f73e2f247a8cf5b83cad0c7731
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441142"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="4e146-103">创建 privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="4e146-103">Create privilegedRoleAssignmentRequest</span></span>

<span data-ttu-id="4e146-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e146-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e146-105">创建 [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4e146-105">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e146-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4e146-106">Permissions</span></span>
<span data-ttu-id="4e146-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e146-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e146-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e146-109">Permission type</span></span>                        | <span data-ttu-id="4e146-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e146-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e146-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e146-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4e146-112">PrivilegedAccess.ReadWrite.AzureAD、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4e146-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4e146-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e146-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e146-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e146-114">Not supported.</span></span> |
|<span data-ttu-id="4e146-115">Application</span><span class="sxs-lookup"><span data-stu-id="4e146-115">Application</span></span>                            | <span data-ttu-id="4e146-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e146-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e146-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e146-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="4e146-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e146-118">Request headers</span></span>
| <span data-ttu-id="4e146-119">名称</span><span class="sxs-lookup"><span data-stu-id="4e146-119">Name</span></span>      |<span data-ttu-id="4e146-120">说明</span><span class="sxs-lookup"><span data-stu-id="4e146-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4e146-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e146-121">Authorization</span></span>  | <span data-ttu-id="4e146-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e146-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e146-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e146-124">Request body</span></span>
<span data-ttu-id="4e146-125">在请求正文中，提供 [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e146-125">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="4e146-126">属性</span><span class="sxs-lookup"><span data-stu-id="4e146-126">Property</span></span>     | <span data-ttu-id="4e146-127">类型</span><span class="sxs-lookup"><span data-stu-id="4e146-127">Type</span></span>    |  <span data-ttu-id="4e146-128">说明</span><span class="sxs-lookup"><span data-stu-id="4e146-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e146-129">roleId</span><span class="sxs-lookup"><span data-stu-id="4e146-129">roleId</span></span>|<span data-ttu-id="4e146-130">String</span><span class="sxs-lookup"><span data-stu-id="4e146-130">String</span></span>|<span data-ttu-id="4e146-131">角色的 ID。</span><span class="sxs-lookup"><span data-stu-id="4e146-131">The ID of the role.</span></span> <span data-ttu-id="4e146-132">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="4e146-132">Required.</span></span>|
|<span data-ttu-id="4e146-133">type</span><span class="sxs-lookup"><span data-stu-id="4e146-133">type</span></span>|<span data-ttu-id="4e146-134">String</span><span class="sxs-lookup"><span data-stu-id="4e146-134">String</span></span>|<span data-ttu-id="4e146-135">表示对项目执行的操作角色分配。</span><span class="sxs-lookup"><span data-stu-id="4e146-135">Represents the type of the operation on the role assignment.</span></span> <span data-ttu-id="4e146-136">值可以是 `AdminAdd` ：管理员将用户添加到角色 `UserAdd` ;：用户添加角色分配。</span><span class="sxs-lookup"><span data-stu-id="4e146-136">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="4e146-137">必需。</span><span class="sxs-lookup"><span data-stu-id="4e146-137">Required.</span></span>|
|<span data-ttu-id="4e146-138">assignmentState</span><span class="sxs-lookup"><span data-stu-id="4e146-138">assignmentState</span></span>|<span data-ttu-id="4e146-139">String</span><span class="sxs-lookup"><span data-stu-id="4e146-139">String</span></span>|<span data-ttu-id="4e146-140">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="4e146-140">The state of the assignment.</span></span> <span data-ttu-id="4e146-141">该值可用于符合条件的分配-如果直接由管理员分配，或由用户激活在符合条件的分配 `Eligible` `Active` `Active` 上。</span><span class="sxs-lookup"><span data-stu-id="4e146-141">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="4e146-142">可取值为：``NotStarted``、`Completed`、`RequestedApproval`、`Scheduled`、`Approved`、`ApprovalDenied`、`ApprovalAborted`、`Cancelling`、`Cancelled`、`Revoked`、`RequestExpired`。</span><span class="sxs-lookup"><span data-stu-id="4e146-142">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="4e146-143">必需。</span><span class="sxs-lookup"><span data-stu-id="4e146-143">Required.</span></span>|
|<span data-ttu-id="4e146-144">reason</span><span class="sxs-lookup"><span data-stu-id="4e146-144">reason</span></span>|<span data-ttu-id="4e146-145">String</span><span class="sxs-lookup"><span data-stu-id="4e146-145">String</span></span>|<span data-ttu-id="4e146-146">需要为审核和审核角色分配请求提供原因。</span><span class="sxs-lookup"><span data-stu-id="4e146-146">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="4e146-147">schedule</span><span class="sxs-lookup"><span data-stu-id="4e146-147">schedule</span></span>|[<span data-ttu-id="4e146-148">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="4e146-148">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="4e146-149">请求角色分配计划。</span><span class="sxs-lookup"><span data-stu-id="4e146-149">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="4e146-150">响应</span><span class="sxs-lookup"><span data-stu-id="4e146-150">Response</span></span>
<span data-ttu-id="4e146-151">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4e146-151">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="4e146-152">错误代码</span><span class="sxs-lookup"><span data-stu-id="4e146-152">Error codes</span></span>
<span data-ttu-id="4e146-153">此 API 返回该标准 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="4e146-153">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="4e146-154">此外，它可以返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="4e146-154">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="4e146-155">错误代码</span><span class="sxs-lookup"><span data-stu-id="4e146-155">Error code</span></span>     | <span data-ttu-id="4e146-156">错误消息</span><span class="sxs-lookup"><span data-stu-id="4e146-156">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="4e146-157">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4e146-157">400 BadRequest</span></span> | <span data-ttu-id="4e146-158">RoleAssignmentRequest 属性为 NULL</span><span class="sxs-lookup"><span data-stu-id="4e146-158">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="4e146-159">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4e146-159">400 BadRequest</span></span> | <span data-ttu-id="4e146-160">无法反初始化 roleAssignmentRequest 对象。</span><span class="sxs-lookup"><span data-stu-id="4e146-160">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="4e146-161">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4e146-161">400 BadRequest</span></span> | <span data-ttu-id="4e146-162">RoleId 是必需的。</span><span class="sxs-lookup"><span data-stu-id="4e146-162">RoleId is required.</span></span> |
| <span data-ttu-id="4e146-163">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4e146-163">400 BadRequest</span></span> | <span data-ttu-id="4e146-164">必须指定计划开始日期，并且应大于"现在"。</span><span class="sxs-lookup"><span data-stu-id="4e146-164">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="4e146-165">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4e146-165">400 BadRequest</span></span> | <span data-ttu-id="4e146-166">此用户、角色和计划类型已存在计划。</span><span class="sxs-lookup"><span data-stu-id="4e146-166">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="4e146-167">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4e146-167">400 BadRequest</span></span> | <span data-ttu-id="4e146-168">此用户、角色和审批类型已存在待审批。</span><span class="sxs-lookup"><span data-stu-id="4e146-168">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="4e146-169">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4e146-169">400 BadRequest</span></span> | <span data-ttu-id="4e146-170">请求者原因缺失。</span><span class="sxs-lookup"><span data-stu-id="4e146-170">Requestor reason is missing.</span></span> |
| <span data-ttu-id="4e146-171">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4e146-171">400 BadRequest</span></span> | <span data-ttu-id="4e146-172">请求者原因应小于 500 个字符。</span><span class="sxs-lookup"><span data-stu-id="4e146-172">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="4e146-173">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4e146-173">400 BadRequest</span></span> | <span data-ttu-id="4e146-174">提升持续时间必须介于 0.5 和 {from setting}之间。</span><span class="sxs-lookup"><span data-stu-id="4e146-174">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="4e146-175">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4e146-175">400 BadRequest</span></span> | <span data-ttu-id="4e146-176">计划激活和请求之间存在重叠。</span><span class="sxs-lookup"><span data-stu-id="4e146-176">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="4e146-177">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4e146-177">400 BadRequest</span></span> | <span data-ttu-id="4e146-178">角色已激活。</span><span class="sxs-lookup"><span data-stu-id="4e146-178">The role is already activated.</span></span> |
| <span data-ttu-id="4e146-179">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4e146-179">400 BadRequest</span></span> | <span data-ttu-id="4e146-180">GenericElevateUserToRoleAssignments：滴答信息是必需的，在激活过程中不提供。</span><span class="sxs-lookup"><span data-stu-id="4e146-180">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="4e146-181">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4e146-181">400 BadRequest</span></span> | <span data-ttu-id="4e146-182">计划激活和请求之间存在重叠。</span><span class="sxs-lookup"><span data-stu-id="4e146-182">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="4e146-183">403 UnAuthorized</span><span class="sxs-lookup"><span data-stu-id="4e146-183">403 UnAuthorized</span></span> | <span data-ttu-id="4e146-184">提升需要多重身份验证。</span><span class="sxs-lookup"><span data-stu-id="4e146-184">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="4e146-185">403 UnAuthorized</span><span class="sxs-lookup"><span data-stu-id="4e146-185">403 UnAuthorized</span></span> | <span data-ttu-id="4e146-186">不允许代表提升。</span><span class="sxs-lookup"><span data-stu-id="4e146-186">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="4e146-187">示例</span><span class="sxs-lookup"><span data-stu-id="4e146-187">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e146-188">请求</span><span class="sxs-lookup"><span data-stu-id="4e146-188">Request</span></span>
<span data-ttu-id="4e146-189">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4e146-189">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4e146-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e146-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_privilegedroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
Content-type: application/json

{
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "schedule": {
        "startDateTime": "2018-02-08T02:35:17.903Z"
    },
    "type": "UserAdd",
    "assignmentState": "Active",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```
# <a name="c"></a>[<span data-ttu-id="4e146-191">C#</span><span class="sxs-lookup"><span data-stu-id="4e146-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e146-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e146-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e146-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e146-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e146-194">Java</span><span class="sxs-lookup"><span data-stu-id="4e146-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-privilegedroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4e146-195">响应</span><span class="sxs-lookup"><span data-stu-id="4e146-195">Response</span></span>
<span data-ttu-id="4e146-196">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4e146-196">The following is an example of the response.</span></span> <span data-ttu-id="4e146-197">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4e146-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4e146-198">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4e146-198">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests/$entity",
    "schedule": {
        "type": "activation",
        "startDateTime": "2018-02-08T02:35:17.903Z",
        "endDateTime": null,
        "duration" : null
    },
    "id": "e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1",
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
    "status": "NotStarted",
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "userId": "Self",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Post privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


