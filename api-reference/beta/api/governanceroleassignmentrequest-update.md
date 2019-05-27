---
title: 更新 governanceRoleAssignmentRequests
description: 使管理员能够更新状态为的`AdminApproved` `PendingAdminDecision`governanceRoleAssignmentRequests `AdminDenied`上的决策 (或)。
localization_priority: Normal
ms.openlocfilehash: b123345ed14bfe3f12471f70a24df5e02aca0f11
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422337"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="8d19f-103">更新 governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="8d19f-103">Update governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d19f-104">使管理员能够更新状态为的`AdminApproved` `AdminDenied` `PendingAdminDecision` [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)上的决策 (或)。</span><span class="sxs-lookup"><span data-stu-id="8d19f-104">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d19f-105">权限</span><span class="sxs-lookup"><span data-stu-id="8d19f-105">Permissions</span></span>
<span data-ttu-id="8d19f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d19f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="8d19f-108">**注意:** 此 API 还要求请求者在[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)所属的资源`Active`中至少有一个`owner`管理员`user access administrator`角色分配 (或)。</span><span class="sxs-lookup"><span data-stu-id="8d19f-108">**Note:** This API also requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="8d19f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d19f-109">Permission type</span></span>      | <span data-ttu-id="8d19f-110">权限</span><span class="sxs-lookup"><span data-stu-id="8d19f-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d19f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d19f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8d19f-112">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="8d19f-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="8d19f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d19f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d19f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d19f-114">Not supported.</span></span>    |
|<span data-ttu-id="8d19f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d19f-115">Application</span></span> | <span data-ttu-id="8d19f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d19f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d19f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d19f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="8d19f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d19f-118">Request headers</span></span>
| <span data-ttu-id="8d19f-119">名称</span><span class="sxs-lookup"><span data-stu-id="8d19f-119">Name</span></span>           | <span data-ttu-id="8d19f-120">说明</span><span class="sxs-lookup"><span data-stu-id="8d19f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8d19f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d19f-121">Authorization</span></span>  | <span data-ttu-id="8d19f-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8d19f-122">Bearer {code}</span></span>|
| <span data-ttu-id="8d19f-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="8d19f-123">Content-type</span></span>  | <span data-ttu-id="8d19f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8d19f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d19f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d19f-125">Request body</span></span>

|<span data-ttu-id="8d19f-126">参数</span><span class="sxs-lookup"><span data-stu-id="8d19f-126">Parameters</span></span>      |<span data-ttu-id="8d19f-127">类型</span><span class="sxs-lookup"><span data-stu-id="8d19f-127">Type</span></span>                   |<span data-ttu-id="8d19f-128">必需</span><span class="sxs-lookup"><span data-stu-id="8d19f-128">Required</span></span> |<span data-ttu-id="8d19f-129">说明</span><span class="sxs-lookup"><span data-stu-id="8d19f-129">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="8d19f-130">在于</span><span class="sxs-lookup"><span data-stu-id="8d19f-130">reason</span></span>        |<span data-ttu-id="8d19f-131">String</span><span class="sxs-lookup"><span data-stu-id="8d19f-131">String</span></span>                 |<span data-ttu-id="8d19f-132">✓</span><span class="sxs-lookup"><span data-stu-id="8d19f-132">✓</span></span>        |<span data-ttu-id="8d19f-133">管理员为自己的决定提供的原因。</span><span class="sxs-lookup"><span data-stu-id="8d19f-133">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="8d19f-134">权</span><span class="sxs-lookup"><span data-stu-id="8d19f-134">decision</span></span>        |<span data-ttu-id="8d19f-135">String</span><span class="sxs-lookup"><span data-stu-id="8d19f-135">String</span></span>                 |<span data-ttu-id="8d19f-136">✓</span><span class="sxs-lookup"><span data-stu-id="8d19f-136">✓</span></span>        |<span data-ttu-id="8d19f-137">角色分配请求的管理员决定。</span><span class="sxs-lookup"><span data-stu-id="8d19f-137">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="8d19f-138">应将值更新为`AdminApproved`或。 `AdminDenied`</span><span class="sxs-lookup"><span data-stu-id="8d19f-138">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="8d19f-139">schedule</span><span class="sxs-lookup"><span data-stu-id="8d19f-139">schedule</span></span>      |[<span data-ttu-id="8d19f-140">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8d19f-140">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="8d19f-141">角色分配请求的日程安排。</span><span class="sxs-lookup"><span data-stu-id="8d19f-141">The schedule of the role assignment request.</span></span> <span data-ttu-id="8d19f-142">对于的状态`AdminApproved`, 是必需的。</span><span class="sxs-lookup"><span data-stu-id="8d19f-142">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="8d19f-143">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8d19f-143">assignmentState</span></span>      |<span data-ttu-id="8d19f-144">String</span><span class="sxs-lookup"><span data-stu-id="8d19f-144">String</span></span>|         | <span data-ttu-id="8d19f-145">工作分配的状态, 值可以是`Eligible`或。 `Active`</span><span class="sxs-lookup"><span data-stu-id="8d19f-145">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="8d19f-146">有关的决策`AdminApproved`, 则是必需的。</span><span class="sxs-lookup"><span data-stu-id="8d19f-146">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="8d19f-147">响应</span><span class="sxs-lookup"><span data-stu-id="8d19f-147">Response</span></span>
<span data-ttu-id="8d19f-148">此方法仅适用于状态为的`PendingAdminDecision`请求。</span><span class="sxs-lookup"><span data-stu-id="8d19f-148">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="8d19f-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8d19f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d19f-151">示例</span><span class="sxs-lookup"><span data-stu-id="8d19f-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d19f-152">请求</span><span class="sxs-lookup"><span data-stu-id="8d19f-152">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
##### <a name="request-body"></a><span data-ttu-id="8d19f-153">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d19f-153">Request body</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8d19f-154">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="8d19f-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8d19f-155">C#</span><span class="sxs-lookup"><span data-stu-id="8d19f-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/updaterequest_governanceroleassignmentrequest-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8d19f-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="8d19f-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/updaterequest_governanceroleassignmentrequest-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="response"></a><span data-ttu-id="8d19f-157">响应</span><span class="sxs-lookup"><span data-stu-id="8d19f-157">Response</span></span>
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
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
