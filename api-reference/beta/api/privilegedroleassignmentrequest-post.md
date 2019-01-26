---
title: 创建 privilegedRoleAssignmentRequest
description: 创建一个 privilegedroleassignmentrequest 对象。
localization_priority: Normal
ms.openlocfilehash: 69e095e13d89ed780feeb7ea32b7aa9ac10de055
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575291"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="53405-103">创建 privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="53405-103">Create privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53405-104">创建一个[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="53405-104">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="53405-105">权限</span><span class="sxs-lookup"><span data-stu-id="53405-105">Permissions</span></span>
<span data-ttu-id="53405-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53405-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53405-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="53405-108">Permission type</span></span>                        | <span data-ttu-id="53405-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53405-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="53405-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53405-110">Delegated (work or school account)</span></span> | <span data-ttu-id="53405-111">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="53405-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="53405-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53405-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53405-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="53405-113">Not supported.</span></span> |
|<span data-ttu-id="53405-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="53405-114">Application</span></span>                            | <span data-ttu-id="53405-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="53405-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53405-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53405-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="53405-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="53405-117">Request headers</span></span>
| <span data-ttu-id="53405-118">名称</span><span class="sxs-lookup"><span data-stu-id="53405-118">Name</span></span>      |<span data-ttu-id="53405-119">说明</span><span class="sxs-lookup"><span data-stu-id="53405-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="53405-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="53405-120">Authorization</span></span>  | <span data-ttu-id="53405-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53405-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53405-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="53405-123">Request body</span></span>
<span data-ttu-id="53405-124">在请求正文中，提供[privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53405-124">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="53405-125">属性</span><span class="sxs-lookup"><span data-stu-id="53405-125">Property</span></span>     | <span data-ttu-id="53405-126">类型</span><span class="sxs-lookup"><span data-stu-id="53405-126">Type</span></span>    |  <span data-ttu-id="53405-127">说明</span><span class="sxs-lookup"><span data-stu-id="53405-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53405-128">roleId</span><span class="sxs-lookup"><span data-stu-id="53405-128">roleId</span></span>|<span data-ttu-id="53405-129">String</span><span class="sxs-lookup"><span data-stu-id="53405-129">String</span></span>|<span data-ttu-id="53405-130">角色的 ID。</span><span class="sxs-lookup"><span data-stu-id="53405-130">The ID of the role.</span></span> <span data-ttu-id="53405-131">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="53405-131">Required.</span></span>|
|<span data-ttu-id="53405-132">type</span><span class="sxs-lookup"><span data-stu-id="53405-132">type</span></span>|<span data-ttu-id="53405-133">String</span><span class="sxs-lookup"><span data-stu-id="53405-133">String</span></span>|<span data-ttu-id="53405-134">表示的角色分配操作的类型。</span><span class="sxs-lookup"><span data-stu-id="53405-134">Represents the the type of the operation on the role assignment.</span></span> <span data-ttu-id="53405-135">值可以是`AdminAdd`： 管理员将用户添加到角色;`UserAdd`： 用户将添加角色分配。</span><span class="sxs-lookup"><span data-stu-id="53405-135">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="53405-136">必需。</span><span class="sxs-lookup"><span data-stu-id="53405-136">Required.</span></span>|
|<span data-ttu-id="53405-137">assignmentState</span><span class="sxs-lookup"><span data-stu-id="53405-137">assignmentState</span></span>|<span data-ttu-id="53405-138">String</span><span class="sxs-lookup"><span data-stu-id="53405-138">String</span></span>|<span data-ttu-id="53405-139">工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="53405-139">The state of the assignment.</span></span> <span data-ttu-id="53405-140">值可以是`Eligible`合格分配`Active`-如果直接分配`Active`由管理员、 或激活合格工作分配的用户。</span><span class="sxs-lookup"><span data-stu-id="53405-140">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="53405-141">可取值为：``NotStarted``、`Completed`、`RequestedApproval`、`Scheduled`、`Approved`、`ApprovalDenied`、`ApprovalAborted`、`Cancelling`、`Cancelled`、`Revoked`、`RequestExpired`。</span><span class="sxs-lookup"><span data-stu-id="53405-141">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="53405-142">必需。</span><span class="sxs-lookup"><span data-stu-id="53405-142">Required.</span></span>|
|<span data-ttu-id="53405-143">原因</span><span class="sxs-lookup"><span data-stu-id="53405-143">reason</span></span>|<span data-ttu-id="53405-144">String</span><span class="sxs-lookup"><span data-stu-id="53405-144">String</span></span>|<span data-ttu-id="53405-145">原因需要提供角色分配请求的审核和查看用途。</span><span class="sxs-lookup"><span data-stu-id="53405-145">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="53405-146">计划</span><span class="sxs-lookup"><span data-stu-id="53405-146">schedule</span></span>|[<span data-ttu-id="53405-147">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="53405-147"> microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="53405-148">角色分配请求的时间表。</span><span class="sxs-lookup"><span data-stu-id="53405-148">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="53405-149">响应</span><span class="sxs-lookup"><span data-stu-id="53405-149">Response</span></span>
<span data-ttu-id="53405-150">如果成功，此方法返回`201 Created`响应代码和响应正文中的[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="53405-150">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="53405-151">错误代码</span><span class="sxs-lookup"><span data-stu-id="53405-151">Error codes</span></span>
<span data-ttu-id="53405-152">此 API 返回的标准 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="53405-152">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="53405-153">此外，它可以返回下表中列出的错误代码。</span><span class="sxs-lookup"><span data-stu-id="53405-153">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="53405-154">错误代码</span><span class="sxs-lookup"><span data-stu-id="53405-154">Error code</span></span>     | <span data-ttu-id="53405-155">错误消息</span><span class="sxs-lookup"><span data-stu-id="53405-155">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="53405-156">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="53405-156">400 BadRequest</span></span> | <span data-ttu-id="53405-157">RoleAssignmentRequest 属性为 NULL</span><span class="sxs-lookup"><span data-stu-id="53405-157">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="53405-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="53405-158">400 BadRequest</span></span> | <span data-ttu-id="53405-159">无法反序列化 roleAssignmentRequest 对象。</span><span class="sxs-lookup"><span data-stu-id="53405-159">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="53405-160">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="53405-160">400 BadRequest</span></span> | <span data-ttu-id="53405-161">RoleId 是必需的。</span><span class="sxs-lookup"><span data-stu-id="53405-161">RoleId is required.</span></span> |
| <span data-ttu-id="53405-162">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="53405-162">400 BadRequest</span></span> | <span data-ttu-id="53405-163">必须指定的计划开始日期和应大于立即。</span><span class="sxs-lookup"><span data-stu-id="53405-163">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="53405-164">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="53405-164">400 BadRequest</span></span> | <span data-ttu-id="53405-165">计划已存在此用户、 角色和计划的类型。</span><span class="sxs-lookup"><span data-stu-id="53405-165">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="53405-166">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="53405-166">400 BadRequest</span></span> | <span data-ttu-id="53405-167">挂起的审批已存在此用户、 角色和审批类型。</span><span class="sxs-lookup"><span data-stu-id="53405-167">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="53405-168">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="53405-168">400 BadRequest</span></span> | <span data-ttu-id="53405-169">找不到请求程序原因。</span><span class="sxs-lookup"><span data-stu-id="53405-169">Requestor reason is missing.</span></span> |
| <span data-ttu-id="53405-170">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="53405-170">400 BadRequest</span></span> | <span data-ttu-id="53405-171">请求程序原因应小于 500 个字符。</span><span class="sxs-lookup"><span data-stu-id="53405-171">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="53405-172">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="53405-172">400 BadRequest</span></span> | <span data-ttu-id="53405-173">特权提升持续时间必须 0.5 之间以及 {从设置}。</span><span class="sxs-lookup"><span data-stu-id="53405-173">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="53405-174">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="53405-174">400 BadRequest</span></span> | <span data-ttu-id="53405-175">没有计划的激活和请求之间的重叠。</span><span class="sxs-lookup"><span data-stu-id="53405-175">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="53405-176">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="53405-176">400 BadRequest</span></span> | <span data-ttu-id="53405-177">已激活的角色。</span><span class="sxs-lookup"><span data-stu-id="53405-177">The role is already activated.</span></span> |
| <span data-ttu-id="53405-178">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="53405-178">400 BadRequest</span></span> | <span data-ttu-id="53405-179">GenericElevateUserToRoleAssignments: Tickting 信息是所需和激活过程中未提供。</span><span class="sxs-lookup"><span data-stu-id="53405-179">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="53405-180">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="53405-180">400 BadRequest</span></span> | <span data-ttu-id="53405-181">没有计划的激活和请求之间的重叠。</span><span class="sxs-lookup"><span data-stu-id="53405-181">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="53405-182">未经授权的 403</span><span class="sxs-lookup"><span data-stu-id="53405-182">403 UnAuthorized</span></span> | <span data-ttu-id="53405-183">特权提升需要多因素身份验证。</span><span class="sxs-lookup"><span data-stu-id="53405-183">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="53405-184">未经授权的 403</span><span class="sxs-lookup"><span data-stu-id="53405-184">403 UnAuthorized</span></span> | <span data-ttu-id="53405-185">不允许代表提升。</span><span class="sxs-lookup"><span data-stu-id="53405-185">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="53405-186">示例</span><span class="sxs-lookup"><span data-stu-id="53405-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53405-187">请求</span><span class="sxs-lookup"><span data-stu-id="53405-187">Request</span></span>
<span data-ttu-id="53405-188">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="53405-188">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="53405-189">响应</span><span class="sxs-lookup"><span data-stu-id="53405-189">Response</span></span>
<span data-ttu-id="53405-190">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="53405-190">The following is an example of the response.</span></span> <span data-ttu-id="53405-191">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="53405-191">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="53405-192">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53405-192">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
