---
title: 创建 privilegedRoleAssignmentRequest
description: 创建 privilegedroleassignmentrequest 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: afc7251bafdb6570eca801abc41ff39216d7381b
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218666"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="979f0-103">创建 privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="979f0-103">Create privilegedRoleAssignmentRequest</span></span>

<span data-ttu-id="979f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="979f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="979f0-105">创建[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="979f0-105">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="979f0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="979f0-106">Permissions</span></span>
<span data-ttu-id="979f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="979f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="979f0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="979f0-109">Permission type</span></span>                        | <span data-ttu-id="979f0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="979f0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="979f0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="979f0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="979f0-112">PrivilegedAccess 的 AzureAD、Directory.accessasuser.all</span><span class="sxs-lookup"><span data-stu-id="979f0-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="979f0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="979f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="979f0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="979f0-114">Not supported.</span></span> |
|<span data-ttu-id="979f0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="979f0-115">Application</span></span>                            | <span data-ttu-id="979f0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="979f0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="979f0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="979f0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="979f0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="979f0-118">Request headers</span></span>
| <span data-ttu-id="979f0-119">名称</span><span class="sxs-lookup"><span data-stu-id="979f0-119">Name</span></span>      |<span data-ttu-id="979f0-120">说明</span><span class="sxs-lookup"><span data-stu-id="979f0-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="979f0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="979f0-121">Authorization</span></span>  | <span data-ttu-id="979f0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="979f0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="979f0-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="979f0-124">Request body</span></span>
<span data-ttu-id="979f0-125">在请求正文中，提供[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="979f0-125">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="979f0-126">属性</span><span class="sxs-lookup"><span data-stu-id="979f0-126">Property</span></span>     | <span data-ttu-id="979f0-127">类型</span><span class="sxs-lookup"><span data-stu-id="979f0-127">Type</span></span>    |  <span data-ttu-id="979f0-128">说明</span><span class="sxs-lookup"><span data-stu-id="979f0-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="979f0-129">roleId</span><span class="sxs-lookup"><span data-stu-id="979f0-129">roleId</span></span>|<span data-ttu-id="979f0-130">字符串</span><span class="sxs-lookup"><span data-stu-id="979f0-130">String</span></span>|<span data-ttu-id="979f0-131">角色的 ID。</span><span class="sxs-lookup"><span data-stu-id="979f0-131">The ID of the role.</span></span> <span data-ttu-id="979f0-132">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="979f0-132">Required.</span></span>|
|<span data-ttu-id="979f0-133">type</span><span class="sxs-lookup"><span data-stu-id="979f0-133">type</span></span>|<span data-ttu-id="979f0-134">字符串</span><span class="sxs-lookup"><span data-stu-id="979f0-134">String</span></span>|<span data-ttu-id="979f0-135">表示角色分配上的操作的类型。</span><span class="sxs-lookup"><span data-stu-id="979f0-135">Represents the type of the operation on the role assignment.</span></span> <span data-ttu-id="979f0-136">值可以是`AdminAdd`： Administrators 将用户添加到角色;`UserAdd`：用户添加角色分配。</span><span class="sxs-lookup"><span data-stu-id="979f0-136">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="979f0-137">必需。</span><span class="sxs-lookup"><span data-stu-id="979f0-137">Required.</span></span>|
|<span data-ttu-id="979f0-138">assignmentState</span><span class="sxs-lookup"><span data-stu-id="979f0-138">assignmentState</span></span>|<span data-ttu-id="979f0-139">字符串</span><span class="sxs-lookup"><span data-stu-id="979f0-139">String</span></span>|<span data-ttu-id="979f0-140">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="979f0-140">The state of the assignment.</span></span> <span data-ttu-id="979f0-141">此值可`Eligible`用于符合条件的`Active`工作分配-如果是由`Active`管理员直接分配的，或者是由用户的符合条件的工作分配激活的。</span><span class="sxs-lookup"><span data-stu-id="979f0-141">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="979f0-142">可取值为：``NotStarted``、`Completed`、`RequestedApproval`、`Scheduled`、`Approved`、`ApprovalDenied`、`ApprovalAborted`、`Cancelling`、`Cancelled`、`Revoked`、`RequestExpired`。</span><span class="sxs-lookup"><span data-stu-id="979f0-142">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="979f0-143">必需。</span><span class="sxs-lookup"><span data-stu-id="979f0-143">Required.</span></span>|
|<span data-ttu-id="979f0-144">reason</span><span class="sxs-lookup"><span data-stu-id="979f0-144">reason</span></span>|<span data-ttu-id="979f0-145">字符串</span><span class="sxs-lookup"><span data-stu-id="979f0-145">String</span></span>|<span data-ttu-id="979f0-146">需要为角色分配请求提供审核和审阅目的的原因。</span><span class="sxs-lookup"><span data-stu-id="979f0-146">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="979f0-147">schedule</span><span class="sxs-lookup"><span data-stu-id="979f0-147">schedule</span></span>|[<span data-ttu-id="979f0-148">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="979f0-148">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="979f0-149">角色分配请求的日程安排。</span><span class="sxs-lookup"><span data-stu-id="979f0-149">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="979f0-150">响应</span><span class="sxs-lookup"><span data-stu-id="979f0-150">Response</span></span>
<span data-ttu-id="979f0-151">如果成功，此方法在响应`201 Created`正文中返回响应代码和[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="979f0-151">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="979f0-152">错误代码</span><span class="sxs-lookup"><span data-stu-id="979f0-152">Error codes</span></span>
<span data-ttu-id="979f0-153">此 API 返回该标准 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="979f0-153">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="979f0-154">此外，它还可以返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="979f0-154">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="979f0-155">错误代码</span><span class="sxs-lookup"><span data-stu-id="979f0-155">Error code</span></span>     | <span data-ttu-id="979f0-156">错误消息</span><span class="sxs-lookup"><span data-stu-id="979f0-156">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="979f0-157">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="979f0-157">400 BadRequest</span></span> | <span data-ttu-id="979f0-158">RoleAssignmentRequest 属性为 NULL</span><span class="sxs-lookup"><span data-stu-id="979f0-158">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="979f0-159">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="979f0-159">400 BadRequest</span></span> | <span data-ttu-id="979f0-160">无法反序列化 roleAssignmentRequest 对象。</span><span class="sxs-lookup"><span data-stu-id="979f0-160">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="979f0-161">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="979f0-161">400 BadRequest</span></span> | <span data-ttu-id="979f0-162">RoleId 是必需的。</span><span class="sxs-lookup"><span data-stu-id="979f0-162">RoleId is required.</span></span> |
| <span data-ttu-id="979f0-163">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="979f0-163">400 BadRequest</span></span> | <span data-ttu-id="979f0-164">必须指定计划开始日期，并且该日期应晚于现在。</span><span class="sxs-lookup"><span data-stu-id="979f0-164">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="979f0-165">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="979f0-165">400 BadRequest</span></span> | <span data-ttu-id="979f0-166">此用户、角色和计划类型的计划已存在。</span><span class="sxs-lookup"><span data-stu-id="979f0-166">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="979f0-167">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="979f0-167">400 BadRequest</span></span> | <span data-ttu-id="979f0-168">此用户、角色和审批类型已存在待批准的审批。</span><span class="sxs-lookup"><span data-stu-id="979f0-168">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="979f0-169">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="979f0-169">400 BadRequest</span></span> | <span data-ttu-id="979f0-170">请求者原因缺失。</span><span class="sxs-lookup"><span data-stu-id="979f0-170">Requestor reason is missing.</span></span> |
| <span data-ttu-id="979f0-171">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="979f0-171">400 BadRequest</span></span> | <span data-ttu-id="979f0-172">请求者原因不应超过500个字符。</span><span class="sxs-lookup"><span data-stu-id="979f0-172">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="979f0-173">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="979f0-173">400 BadRequest</span></span> | <span data-ttu-id="979f0-174">提升持续时间必须介于0.5 和 {from setting} 之间。</span><span class="sxs-lookup"><span data-stu-id="979f0-174">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="979f0-175">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="979f0-175">400 BadRequest</span></span> | <span data-ttu-id="979f0-176">计划激活和请求之间存在重叠。</span><span class="sxs-lookup"><span data-stu-id="979f0-176">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="979f0-177">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="979f0-177">400 BadRequest</span></span> | <span data-ttu-id="979f0-178">角色已激活。</span><span class="sxs-lookup"><span data-stu-id="979f0-178">The role is already activated.</span></span> |
| <span data-ttu-id="979f0-179">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="979f0-179">400 BadRequest</span></span> | <span data-ttu-id="979f0-180">GenericElevateUserToRoleAssignments： Tickting 信息是必需的，并且在激活过程中不提供。</span><span class="sxs-lookup"><span data-stu-id="979f0-180">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="979f0-181">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="979f0-181">400 BadRequest</span></span> | <span data-ttu-id="979f0-182">计划激活和请求之间存在重叠。</span><span class="sxs-lookup"><span data-stu-id="979f0-182">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="979f0-183">403未经授权</span><span class="sxs-lookup"><span data-stu-id="979f0-183">403 UnAuthorized</span></span> | <span data-ttu-id="979f0-184">提升需要多因素身份验证。</span><span class="sxs-lookup"><span data-stu-id="979f0-184">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="979f0-185">403未经授权</span><span class="sxs-lookup"><span data-stu-id="979f0-185">403 UnAuthorized</span></span> | <span data-ttu-id="979f0-186">代表提升是不允许的。</span><span class="sxs-lookup"><span data-stu-id="979f0-186">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="979f0-187">示例</span><span class="sxs-lookup"><span data-stu-id="979f0-187">Example</span></span>
##### <a name="request"></a><span data-ttu-id="979f0-188">请求</span><span class="sxs-lookup"><span data-stu-id="979f0-188">Request</span></span>
<span data-ttu-id="979f0-189">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="979f0-189">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="979f0-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="979f0-190">HTTP</span></span>](#tab/http)
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
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```
# <a name="c"></a>[<span data-ttu-id="979f0-191">C#</span><span class="sxs-lookup"><span data-stu-id="979f0-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="979f0-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="979f0-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="979f0-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="979f0-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="979f0-194">响应</span><span class="sxs-lookup"><span data-stu-id="979f0-194">Response</span></span>
<span data-ttu-id="979f0-195">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="979f0-195">The following is an example of the response.</span></span> <span data-ttu-id="979f0-196">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="979f0-196">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="979f0-197">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="979f0-197">All of the properties will be returned from an actual call.</span></span>
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
    "evaluateOnly": false,
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
