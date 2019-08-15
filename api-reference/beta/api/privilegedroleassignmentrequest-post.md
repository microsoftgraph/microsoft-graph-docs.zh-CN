---
title: 创建 privilegedRoleAssignmentRequest
description: 创建 privilegedroleassignmentrequest 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: a6064a78accbbbd2364485c2c22fc679bc415a5a
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412605"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="9c554-103">创建 privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="9c554-103">Create privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c554-104">创建[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9c554-104">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c554-105">权限</span><span class="sxs-lookup"><span data-stu-id="9c554-105">Permissions</span></span>
<span data-ttu-id="9c554-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c554-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c554-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c554-108">Permission type</span></span>                        | <span data-ttu-id="9c554-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c554-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c554-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c554-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9c554-111">PrivilegedAccess 的 AzureAD、Directory.accessasuser.all</span><span class="sxs-lookup"><span data-stu-id="9c554-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9c554-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c554-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c554-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c554-113">Not supported.</span></span> |
|<span data-ttu-id="9c554-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c554-114">Application</span></span>                            | <span data-ttu-id="9c554-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c554-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c554-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c554-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="9c554-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c554-117">Request headers</span></span>
| <span data-ttu-id="9c554-118">名称</span><span class="sxs-lookup"><span data-stu-id="9c554-118">Name</span></span>      |<span data-ttu-id="9c554-119">说明</span><span class="sxs-lookup"><span data-stu-id="9c554-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9c554-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c554-120">Authorization</span></span>  | <span data-ttu-id="9c554-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9c554-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c554-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c554-123">Request body</span></span>
<span data-ttu-id="9c554-124">在请求正文中, 提供[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c554-124">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="9c554-125">属性</span><span class="sxs-lookup"><span data-stu-id="9c554-125">Property</span></span>     | <span data-ttu-id="9c554-126">类型</span><span class="sxs-lookup"><span data-stu-id="9c554-126">Type</span></span>    |  <span data-ttu-id="9c554-127">说明</span><span class="sxs-lookup"><span data-stu-id="9c554-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c554-128">roleId</span><span class="sxs-lookup"><span data-stu-id="9c554-128">roleId</span></span>|<span data-ttu-id="9c554-129">String</span><span class="sxs-lookup"><span data-stu-id="9c554-129">String</span></span>|<span data-ttu-id="9c554-130">角色的 ID。</span><span class="sxs-lookup"><span data-stu-id="9c554-130">The ID of the role.</span></span> <span data-ttu-id="9c554-131">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="9c554-131">Required.</span></span>|
|<span data-ttu-id="9c554-132">type</span><span class="sxs-lookup"><span data-stu-id="9c554-132">type</span></span>|<span data-ttu-id="9c554-133">String</span><span class="sxs-lookup"><span data-stu-id="9c554-133">String</span></span>|<span data-ttu-id="9c554-134">表示角色分配上的操作的类型。</span><span class="sxs-lookup"><span data-stu-id="9c554-134">Represents the type of the operation on the role assignment.</span></span> <span data-ttu-id="9c554-135">值可以是`AdminAdd`: Administrators 将用户添加到角色;`UserAdd`: 用户添加角色分配。</span><span class="sxs-lookup"><span data-stu-id="9c554-135">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="9c554-136">必需。</span><span class="sxs-lookup"><span data-stu-id="9c554-136">Required.</span></span>|
|<span data-ttu-id="9c554-137">assignmentState</span><span class="sxs-lookup"><span data-stu-id="9c554-137">assignmentState</span></span>|<span data-ttu-id="9c554-138">String</span><span class="sxs-lookup"><span data-stu-id="9c554-138">String</span></span>|<span data-ttu-id="9c554-139">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="9c554-139">The state of the assignment.</span></span> <span data-ttu-id="9c554-140">此值可`Eligible`用于符合条件的`Active`工作分配-如果是由`Active`管理员直接分配的, 或者是由用户的符合条件的工作分配激活的。</span><span class="sxs-lookup"><span data-stu-id="9c554-140">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="9c554-141">可取值为：``NotStarted``、`Completed`、`RequestedApproval`、`Scheduled`、`Approved`、`ApprovalDenied`、`ApprovalAborted`、`Cancelling`、`Cancelled`、`Revoked`、`RequestExpired`。</span><span class="sxs-lookup"><span data-stu-id="9c554-141">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="9c554-142">必需。</span><span class="sxs-lookup"><span data-stu-id="9c554-142">Required.</span></span>|
|<span data-ttu-id="9c554-143">在于</span><span class="sxs-lookup"><span data-stu-id="9c554-143">reason</span></span>|<span data-ttu-id="9c554-144">String</span><span class="sxs-lookup"><span data-stu-id="9c554-144">String</span></span>|<span data-ttu-id="9c554-145">需要为角色分配请求提供审核和审阅目的的原因。</span><span class="sxs-lookup"><span data-stu-id="9c554-145">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="9c554-146">schedule</span><span class="sxs-lookup"><span data-stu-id="9c554-146">schedule</span></span>|[<span data-ttu-id="9c554-147">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="9c554-147">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="9c554-148">角色分配请求的日程安排。</span><span class="sxs-lookup"><span data-stu-id="9c554-148">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="9c554-149">响应</span><span class="sxs-lookup"><span data-stu-id="9c554-149">Response</span></span>
<span data-ttu-id="9c554-150">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9c554-150">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="9c554-151">错误代码</span><span class="sxs-lookup"><span data-stu-id="9c554-151">Error codes</span></span>
<span data-ttu-id="9c554-152">此 API 返回该标准 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="9c554-152">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="9c554-153">此外, 它还可以返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="9c554-153">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="9c554-154">错误代码</span><span class="sxs-lookup"><span data-stu-id="9c554-154">Error code</span></span>     | <span data-ttu-id="9c554-155">错误消息</span><span class="sxs-lookup"><span data-stu-id="9c554-155">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="9c554-156">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c554-156">400 BadRequest</span></span> | <span data-ttu-id="9c554-157">RoleAssignmentRequest 属性为 NULL</span><span class="sxs-lookup"><span data-stu-id="9c554-157">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="9c554-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c554-158">400 BadRequest</span></span> | <span data-ttu-id="9c554-159">无法反序列化 roleAssignmentRequest 对象。</span><span class="sxs-lookup"><span data-stu-id="9c554-159">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="9c554-160">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c554-160">400 BadRequest</span></span> | <span data-ttu-id="9c554-161">RoleId 是必需的。</span><span class="sxs-lookup"><span data-stu-id="9c554-161">RoleId is required.</span></span> |
| <span data-ttu-id="9c554-162">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c554-162">400 BadRequest</span></span> | <span data-ttu-id="9c554-163">必须指定计划开始日期, 并且该日期应晚于现在。</span><span class="sxs-lookup"><span data-stu-id="9c554-163">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="9c554-164">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c554-164">400 BadRequest</span></span> | <span data-ttu-id="9c554-165">此用户、角色和计划类型的计划已存在。</span><span class="sxs-lookup"><span data-stu-id="9c554-165">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="9c554-166">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c554-166">400 BadRequest</span></span> | <span data-ttu-id="9c554-167">此用户、角色和审批类型已存在待批准的审批。</span><span class="sxs-lookup"><span data-stu-id="9c554-167">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="9c554-168">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c554-168">400 BadRequest</span></span> | <span data-ttu-id="9c554-169">请求者原因缺失。</span><span class="sxs-lookup"><span data-stu-id="9c554-169">Requestor reason is missing.</span></span> |
| <span data-ttu-id="9c554-170">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c554-170">400 BadRequest</span></span> | <span data-ttu-id="9c554-171">请求者原因不应超过500个字符。</span><span class="sxs-lookup"><span data-stu-id="9c554-171">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="9c554-172">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c554-172">400 BadRequest</span></span> | <span data-ttu-id="9c554-173">提升持续时间必须介于0.5 和 {from setting} 之间。</span><span class="sxs-lookup"><span data-stu-id="9c554-173">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="9c554-174">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c554-174">400 BadRequest</span></span> | <span data-ttu-id="9c554-175">计划激活和请求之间存在重叠。</span><span class="sxs-lookup"><span data-stu-id="9c554-175">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="9c554-176">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c554-176">400 BadRequest</span></span> | <span data-ttu-id="9c554-177">角色已激活。</span><span class="sxs-lookup"><span data-stu-id="9c554-177">The role is already activated.</span></span> |
| <span data-ttu-id="9c554-178">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c554-178">400 BadRequest</span></span> | <span data-ttu-id="9c554-179">GenericElevateUserToRoleAssignments: Tickting 信息是必需的, 并且在激活过程中不提供。</span><span class="sxs-lookup"><span data-stu-id="9c554-179">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="9c554-180">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9c554-180">400 BadRequest</span></span> | <span data-ttu-id="9c554-181">计划激活和请求之间存在重叠。</span><span class="sxs-lookup"><span data-stu-id="9c554-181">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="9c554-182">403未经授权</span><span class="sxs-lookup"><span data-stu-id="9c554-182">403 UnAuthorized</span></span> | <span data-ttu-id="9c554-183">提升需要多因素身份验证。</span><span class="sxs-lookup"><span data-stu-id="9c554-183">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="9c554-184">403未经授权</span><span class="sxs-lookup"><span data-stu-id="9c554-184">403 UnAuthorized</span></span> | <span data-ttu-id="9c554-185">代表提升是不允许的。</span><span class="sxs-lookup"><span data-stu-id="9c554-185">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="9c554-186">示例</span><span class="sxs-lookup"><span data-stu-id="9c554-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c554-187">请求</span><span class="sxs-lookup"><span data-stu-id="9c554-187">Request</span></span>
<span data-ttu-id="9c554-188">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9c554-188">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9c554-189">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="9c554-189">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9c554-190">C#</span><span class="sxs-lookup"><span data-stu-id="9c554-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9c554-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c554-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9c554-192">目标-C</span><span class="sxs-lookup"><span data-stu-id="9c554-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9c554-193">响应</span><span class="sxs-lookup"><span data-stu-id="9c554-193">Response</span></span>
<span data-ttu-id="9c554-194">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9c554-194">The following is an example of the response.</span></span> <span data-ttu-id="9c554-195">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9c554-195">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9c554-196">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9c554-196">All of the properties will be returned from an actual call.</span></span>
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
