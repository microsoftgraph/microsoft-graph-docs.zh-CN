---
title: 更新 governanceRoleAssignmentRequests
description: 使管理员能够更新其决策 (`AdminApproved`或`AdminDenied`) 中的状态的 governanceRoleAssignmentRequests 上`PendingAdminDecision`。
localization_priority: Normal
ms.openlocfilehash: 01178492517ae0ce1e2ed011e749e54af8e5d805
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576526"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="81ca6-103">更新 governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="81ca6-103">Update governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81ca6-104">使管理员能够更新其决策 (`AdminApproved`或`AdminDenied`) 上[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)中的状态的`PendingAdminDecision`。</span><span class="sxs-lookup"><span data-stu-id="81ca6-104">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="81ca6-105">权限</span><span class="sxs-lookup"><span data-stu-id="81ca6-105">Permissions</span></span>
<span data-ttu-id="81ca6-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="81ca6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="81ca6-108">**注意：** 此 API 还需要请求者必须至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)所属的资源。</span><span class="sxs-lookup"><span data-stu-id="81ca6-108">**Note:** This API also requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="81ca6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="81ca6-109">Permission type</span></span>      | <span data-ttu-id="81ca6-110">权限</span><span class="sxs-lookup"><span data-stu-id="81ca6-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81ca6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81ca6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="81ca6-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="81ca6-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="81ca6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81ca6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81ca6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="81ca6-114">Not supported.</span></span>    |
|<span data-ttu-id="81ca6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="81ca6-115">Application</span></span> | <span data-ttu-id="81ca6-116">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="81ca6-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="81ca6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81ca6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="81ca6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="81ca6-118">Request headers</span></span>
| <span data-ttu-id="81ca6-119">名称</span><span class="sxs-lookup"><span data-stu-id="81ca6-119">Name</span></span>           | <span data-ttu-id="81ca6-120">说明</span><span class="sxs-lookup"><span data-stu-id="81ca6-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="81ca6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="81ca6-121">Authorization</span></span>  | <span data-ttu-id="81ca6-122">持有者 {code}</span><span class="sxs-lookup"><span data-stu-id="81ca6-122">Bearer {code}</span></span>|
| <span data-ttu-id="81ca6-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="81ca6-123">Content-type</span></span>  | <span data-ttu-id="81ca6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="81ca6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81ca6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="81ca6-125">Request body</span></span>

|<span data-ttu-id="81ca6-126">参数</span><span class="sxs-lookup"><span data-stu-id="81ca6-126">Parameters</span></span>      |<span data-ttu-id="81ca6-127">类型</span><span class="sxs-lookup"><span data-stu-id="81ca6-127">Type</span></span>                   |<span data-ttu-id="81ca6-128">必需</span><span class="sxs-lookup"><span data-stu-id="81ca6-128">Required</span></span> |<span data-ttu-id="81ca6-129">说明</span><span class="sxs-lookup"><span data-stu-id="81ca6-129">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="81ca6-130">原因</span><span class="sxs-lookup"><span data-stu-id="81ca6-130">reason</span></span>        |<span data-ttu-id="81ca6-131">String</span><span class="sxs-lookup"><span data-stu-id="81ca6-131">String</span></span>                 |<span data-ttu-id="81ca6-132">✓</span><span class="sxs-lookup"><span data-stu-id="81ca6-132">✓</span></span>        |<span data-ttu-id="81ca6-133">提供由管理员为其决策的原因。</span><span class="sxs-lookup"><span data-stu-id="81ca6-133">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="81ca6-134">决策</span><span class="sxs-lookup"><span data-stu-id="81ca6-134">decision</span></span>        |<span data-ttu-id="81ca6-135">String</span><span class="sxs-lookup"><span data-stu-id="81ca6-135">String</span></span>                 |<span data-ttu-id="81ca6-136">✓</span><span class="sxs-lookup"><span data-stu-id="81ca6-136">✓</span></span>        |<span data-ttu-id="81ca6-137">角色分配请求的管理员决策。</span><span class="sxs-lookup"><span data-stu-id="81ca6-137">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="81ca6-138">值应更新为`AdminApproved`或`AdminDenied`。</span><span class="sxs-lookup"><span data-stu-id="81ca6-138">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="81ca6-139">计划</span><span class="sxs-lookup"><span data-stu-id="81ca6-139">schedule</span></span>      |[<span data-ttu-id="81ca6-140">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="81ca6-140"> microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="81ca6-141">角色分配请求的时间表。</span><span class="sxs-lookup"><span data-stu-id="81ca6-141">The schedule of the role assignment request.</span></span> <span data-ttu-id="81ca6-142">状态的`AdminApproved`，需要。</span><span class="sxs-lookup"><span data-stu-id="81ca6-142">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="81ca6-143">assignmentState</span><span class="sxs-lookup"><span data-stu-id="81ca6-143">assignmentState</span></span>      |<span data-ttu-id="81ca6-144">String</span><span class="sxs-lookup"><span data-stu-id="81ca6-144">String</span></span>|         | <span data-ttu-id="81ca6-145">状态的工作分配，以及的值可以是`Eligible`或`Active`。</span><span class="sxs-lookup"><span data-stu-id="81ca6-145">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="81ca6-146">为决策的`AdminApproved`，需要。</span><span class="sxs-lookup"><span data-stu-id="81ca6-146">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="81ca6-147">响应</span><span class="sxs-lookup"><span data-stu-id="81ca6-147">Response</span></span>
<span data-ttu-id="81ca6-148">此方法可以仅适用于请求的状态中的`PendingAdminDecision`。</span><span class="sxs-lookup"><span data-stu-id="81ca6-148">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="81ca6-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="81ca6-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81ca6-151">示例</span><span class="sxs-lookup"><span data-stu-id="81ca6-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81ca6-152">请求</span><span class="sxs-lookup"><span data-stu-id="81ca6-152">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
##### <a name="request-body"></a><span data-ttu-id="81ca6-153">请求正文</span><span class="sxs-lookup"><span data-stu-id="81ca6-153">Request body</span></span>
```json
{
  "reason":"approve the request to extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-02-20T07:31:13.451Z",
    "stopDateTime":"2018-05-21T07:31:13.451Z",
    },
  "decision":"AdminApproved",
  "assignmentState": "Eligible"
}
```

##### <a name="response"></a><span data-ttu-id="81ca6-154">响应</span><span class="sxs-lookup"><span data-stu-id="81ca6-154">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "UpdateRequest governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
