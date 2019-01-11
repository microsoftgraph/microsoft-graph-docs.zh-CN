---
title: 创建 privilegedRoleAssignmentRequest
description: 创建一个 privilegedroleassignmentrequest 对象。
localization_priority: Normal
ms.openlocfilehash: 3f1b88415e5671e38ad557cc28200569a42a9630
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847766"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="f2528-103">创建 privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f2528-103">Create privilegedRoleAssignmentRequest</span></span>

> <span data-ttu-id="f2528-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f2528-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2528-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f2528-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2528-106">创建一个[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f2528-106">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2528-107">权限</span><span class="sxs-lookup"><span data-stu-id="f2528-107">Permissions</span></span>
<span data-ttu-id="f2528-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2528-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2528-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2528-110">Permission type</span></span>                        | <span data-ttu-id="f2528-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2528-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2528-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2528-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f2528-113">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f2528-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f2528-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2528-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2528-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2528-115">Not supported.</span></span> |
|<span data-ttu-id="f2528-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2528-116">Application</span></span>                            | <span data-ttu-id="f2528-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2528-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2528-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2528-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="f2528-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2528-119">Request headers</span></span>
| <span data-ttu-id="f2528-120">名称</span><span class="sxs-lookup"><span data-stu-id="f2528-120">Name</span></span>      |<span data-ttu-id="f2528-121">说明</span><span class="sxs-lookup"><span data-stu-id="f2528-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f2528-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2528-122">Authorization</span></span>  | <span data-ttu-id="f2528-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2528-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2528-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2528-125">Request body</span></span>
<span data-ttu-id="f2528-126">在请求正文中，提供[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2528-126">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="f2528-127">属性</span><span class="sxs-lookup"><span data-stu-id="f2528-127">Property</span></span>     | <span data-ttu-id="f2528-128">类型</span><span class="sxs-lookup"><span data-stu-id="f2528-128">Type</span></span>    |  <span data-ttu-id="f2528-129">Description</span><span class="sxs-lookup"><span data-stu-id="f2528-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2528-130">roleId</span><span class="sxs-lookup"><span data-stu-id="f2528-130">roleId</span></span>|<span data-ttu-id="f2528-131">字符串</span><span class="sxs-lookup"><span data-stu-id="f2528-131">String</span></span>|<span data-ttu-id="f2528-132">角色的 ID。</span><span class="sxs-lookup"><span data-stu-id="f2528-132">The ID of the role.</span></span> <span data-ttu-id="f2528-133">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="f2528-133">Required.</span></span>|
|<span data-ttu-id="f2528-134">type</span><span class="sxs-lookup"><span data-stu-id="f2528-134">type</span></span>|<span data-ttu-id="f2528-135">字符串</span><span class="sxs-lookup"><span data-stu-id="f2528-135">String</span></span>|<span data-ttu-id="f2528-136">表示的角色分配操作的类型。</span><span class="sxs-lookup"><span data-stu-id="f2528-136">Represents the the type of the operation on the role assignment.</span></span> <span data-ttu-id="f2528-137">值可以是`AdminAdd`： 管理员将用户添加到角色;`UserAdd`： 用户将添加角色分配。</span><span class="sxs-lookup"><span data-stu-id="f2528-137">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="f2528-138">必填。</span><span class="sxs-lookup"><span data-stu-id="f2528-138">Required.</span></span>|
|<span data-ttu-id="f2528-139">assignmentState</span><span class="sxs-lookup"><span data-stu-id="f2528-139">assignmentState</span></span>|<span data-ttu-id="f2528-140">字符串</span><span class="sxs-lookup"><span data-stu-id="f2528-140">String</span></span>|<span data-ttu-id="f2528-141">工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="f2528-141">The state of the assignment.</span></span> <span data-ttu-id="f2528-142">值可以是`Eligible`合格分配`Active`-如果直接分配`Active`由管理员、 或激活合格工作分配的用户。</span><span class="sxs-lookup"><span data-stu-id="f2528-142">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="f2528-143">可取值为：``NotStarted``、`Completed`、`RequestedApproval`、`Scheduled`、`Approved`、`ApprovalDenied`、`ApprovalAborted`、`Cancelling`、`Cancelled`、`Revoked`、`RequestExpired`。</span><span class="sxs-lookup"><span data-stu-id="f2528-143">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="f2528-144">必填。</span><span class="sxs-lookup"><span data-stu-id="f2528-144">Required.</span></span>|
|<span data-ttu-id="f2528-145">原因</span><span class="sxs-lookup"><span data-stu-id="f2528-145">reason</span></span>|<span data-ttu-id="f2528-146">字符串</span><span class="sxs-lookup"><span data-stu-id="f2528-146">String</span></span>|<span data-ttu-id="f2528-147">原因需要提供角色分配请求的审核和查看用途。</span><span class="sxs-lookup"><span data-stu-id="f2528-147">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="f2528-148">计划</span><span class="sxs-lookup"><span data-stu-id="f2528-148">schedule</span></span>|[<span data-ttu-id="f2528-149">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="f2528-149">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="f2528-150">角色分配请求的时间表。</span><span class="sxs-lookup"><span data-stu-id="f2528-150">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="f2528-151">响应</span><span class="sxs-lookup"><span data-stu-id="f2528-151">Response</span></span>
<span data-ttu-id="f2528-152">如果成功，此方法返回`201 Created`响应代码和响应正文中的[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f2528-152">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="f2528-153">错误代码</span><span class="sxs-lookup"><span data-stu-id="f2528-153">Error codes</span></span>
<span data-ttu-id="f2528-154">此 API 返回的标准 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="f2528-154">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="f2528-155">此外，它可以返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="f2528-155">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="f2528-156">错误代码</span><span class="sxs-lookup"><span data-stu-id="f2528-156">Error code</span></span>     | <span data-ttu-id="f2528-157">错误消息</span><span class="sxs-lookup"><span data-stu-id="f2528-157">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="f2528-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2528-158">400 BadRequest</span></span> | <span data-ttu-id="f2528-159">RoleAssignmentRequest 属性为 NULL</span><span class="sxs-lookup"><span data-stu-id="f2528-159">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="f2528-160">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2528-160">400 BadRequest</span></span> | <span data-ttu-id="f2528-161">无法反序列化 roleAssignmentRequest 对象。</span><span class="sxs-lookup"><span data-stu-id="f2528-161">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="f2528-162">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2528-162">400 BadRequest</span></span> | <span data-ttu-id="f2528-163">RoleId 是必需的。</span><span class="sxs-lookup"><span data-stu-id="f2528-163">RoleId is required.</span></span> |
| <span data-ttu-id="f2528-164">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2528-164">400 BadRequest</span></span> | <span data-ttu-id="f2528-165">必须指定的计划开始日期和应大于立即。</span><span class="sxs-lookup"><span data-stu-id="f2528-165">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="f2528-166">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2528-166">400 BadRequest</span></span> | <span data-ttu-id="f2528-167">计划已存在此用户、 角色和计划的类型。</span><span class="sxs-lookup"><span data-stu-id="f2528-167">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="f2528-168">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2528-168">400 BadRequest</span></span> | <span data-ttu-id="f2528-169">挂起的审批已存在此用户、 角色和审批类型。</span><span class="sxs-lookup"><span data-stu-id="f2528-169">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="f2528-170">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2528-170">400 BadRequest</span></span> | <span data-ttu-id="f2528-171">找不到请求程序原因。</span><span class="sxs-lookup"><span data-stu-id="f2528-171">Requestor reason is missing.</span></span> |
| <span data-ttu-id="f2528-172">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2528-172">400 BadRequest</span></span> | <span data-ttu-id="f2528-173">请求程序原因应小于 500 个字符。</span><span class="sxs-lookup"><span data-stu-id="f2528-173">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="f2528-174">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2528-174">400 BadRequest</span></span> | <span data-ttu-id="f2528-175">特权提升持续时间必须 0.5 之间以及 {从设置}。</span><span class="sxs-lookup"><span data-stu-id="f2528-175">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="f2528-176">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2528-176">400 BadRequest</span></span> | <span data-ttu-id="f2528-177">没有计划的激活和请求之间的重叠。</span><span class="sxs-lookup"><span data-stu-id="f2528-177">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="f2528-178">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2528-178">400 BadRequest</span></span> | <span data-ttu-id="f2528-179">已激活的角色。</span><span class="sxs-lookup"><span data-stu-id="f2528-179">The role is already activated.</span></span> |
| <span data-ttu-id="f2528-180">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2528-180">400 BadRequest</span></span> | <span data-ttu-id="f2528-181">GenericElevateUserToRoleAssignments: Tickting 信息是所需和激活过程中未提供。</span><span class="sxs-lookup"><span data-stu-id="f2528-181">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="f2528-182">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f2528-182">400 BadRequest</span></span> | <span data-ttu-id="f2528-183">没有计划的激活和请求之间的重叠。</span><span class="sxs-lookup"><span data-stu-id="f2528-183">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="f2528-184">未经授权的 403</span><span class="sxs-lookup"><span data-stu-id="f2528-184">403 UnAuthorized</span></span> | <span data-ttu-id="f2528-185">特权提升需要多因素身份验证。</span><span class="sxs-lookup"><span data-stu-id="f2528-185">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="f2528-186">未经授权的 403</span><span class="sxs-lookup"><span data-stu-id="f2528-186">403 UnAuthorized</span></span> | <span data-ttu-id="f2528-187">不允许代表提升。</span><span class="sxs-lookup"><span data-stu-id="f2528-187">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="f2528-188">示例</span><span class="sxs-lookup"><span data-stu-id="f2528-188">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2528-189">请求</span><span class="sxs-lookup"><span data-stu-id="f2528-189">Request</span></span>
<span data-ttu-id="f2528-190">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f2528-190">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="f2528-191">响应</span><span class="sxs-lookup"><span data-stu-id="f2528-191">Response</span></span>
<span data-ttu-id="f2528-192">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f2528-192">The following is an example of the response.</span></span> <span data-ttu-id="f2528-193">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f2528-193">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f2528-194">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2528-194">All of the properties will be returned from an actual call.</span></span>
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
    "userId": "Self"，
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Post privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
