---
title: 更新 governanceRoleAssignmentRequests
description: 使管理员能够更新 `AdminApproved` 状态为的 governanceRoleAssignmentRequests 上的决策 (或 `AdminDenied`) `PendingAdminDecision` 。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 75c6044e6fc76c0ac19e7990240b883f663cba04
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991059"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="a1749-103">更新 governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="a1749-103">Update governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="a1749-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1749-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1749-105">使管理员能够更新 `AdminApproved` `AdminDenied` 状态为的 [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) 上的决策 (或) `PendingAdminDecision` 。</span><span class="sxs-lookup"><span data-stu-id="a1749-105">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1749-106">权限</span><span class="sxs-lookup"><span data-stu-id="a1749-106">Permissions</span></span>
<span data-ttu-id="a1749-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1749-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="a1749-109">**注意：** 此 API 还要求请求者在 `Active` `owner` `user access administrator` [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 所属的资源上至少有一个管理员角色分配 (或) 。</span><span class="sxs-lookup"><span data-stu-id="a1749-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="a1749-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1749-110">Permission type</span></span>      | <span data-ttu-id="a1749-111">权限</span><span class="sxs-lookup"><span data-stu-id="a1749-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1749-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1749-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a1749-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="a1749-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="a1749-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1749-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1749-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1749-115">Not supported.</span></span>    |
|<span data-ttu-id="a1749-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1749-116">Application</span></span> | <span data-ttu-id="a1749-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1749-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1749-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1749-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="a1749-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1749-119">Request headers</span></span>
| <span data-ttu-id="a1749-120">名称</span><span class="sxs-lookup"><span data-stu-id="a1749-120">Name</span></span>           | <span data-ttu-id="a1749-121">说明</span><span class="sxs-lookup"><span data-stu-id="a1749-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a1749-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1749-122">Authorization</span></span>  | <span data-ttu-id="a1749-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a1749-123">Bearer {code}</span></span>|
| <span data-ttu-id="a1749-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="a1749-124">Content-type</span></span>  | <span data-ttu-id="a1749-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1749-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1749-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1749-126">Request body</span></span>

|<span data-ttu-id="a1749-127">参数</span><span class="sxs-lookup"><span data-stu-id="a1749-127">Parameters</span></span>      |<span data-ttu-id="a1749-128">类型</span><span class="sxs-lookup"><span data-stu-id="a1749-128">Type</span></span>                   |<span data-ttu-id="a1749-129">必需</span><span class="sxs-lookup"><span data-stu-id="a1749-129">Required</span></span> |<span data-ttu-id="a1749-130">说明</span><span class="sxs-lookup"><span data-stu-id="a1749-130">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="a1749-131">reason</span><span class="sxs-lookup"><span data-stu-id="a1749-131">reason</span></span>        |<span data-ttu-id="a1749-132">String</span><span class="sxs-lookup"><span data-stu-id="a1749-132">String</span></span>                 |<span data-ttu-id="a1749-133">✓</span><span class="sxs-lookup"><span data-stu-id="a1749-133">✓</span></span>        |<span data-ttu-id="a1749-134">管理员为自己的决定提供的原因。</span><span class="sxs-lookup"><span data-stu-id="a1749-134">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="a1749-135">权</span><span class="sxs-lookup"><span data-stu-id="a1749-135">decision</span></span>        |<span data-ttu-id="a1749-136">String</span><span class="sxs-lookup"><span data-stu-id="a1749-136">String</span></span>                 |<span data-ttu-id="a1749-137">✓</span><span class="sxs-lookup"><span data-stu-id="a1749-137">✓</span></span>        |<span data-ttu-id="a1749-138">角色分配请求的管理员决定。</span><span class="sxs-lookup"><span data-stu-id="a1749-138">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="a1749-139">应将值更新为 `AdminApproved` 或 `AdminDenied` 。</span><span class="sxs-lookup"><span data-stu-id="a1749-139">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="a1749-140">schedule</span><span class="sxs-lookup"><span data-stu-id="a1749-140">schedule</span></span>      |[<span data-ttu-id="a1749-141">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a1749-141">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="a1749-142">角色分配请求的日程安排。</span><span class="sxs-lookup"><span data-stu-id="a1749-142">The schedule of the role assignment request.</span></span> <span data-ttu-id="a1749-143">对于的状态 `AdminApproved` ，是必需的。</span><span class="sxs-lookup"><span data-stu-id="a1749-143">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="a1749-144">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a1749-144">assignmentState</span></span>      |<span data-ttu-id="a1749-145">String</span><span class="sxs-lookup"><span data-stu-id="a1749-145">String</span></span>|         | <span data-ttu-id="a1749-146">工作分配的状态，值可以是 `Eligible` 或 `Active` 。</span><span class="sxs-lookup"><span data-stu-id="a1749-146">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="a1749-147">有关的决策 `AdminApproved` ，则是必需的。</span><span class="sxs-lookup"><span data-stu-id="a1749-147">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="a1749-148">响应</span><span class="sxs-lookup"><span data-stu-id="a1749-148">Response</span></span>
<span data-ttu-id="a1749-149">此方法仅适用于状态为的请求 `PendingAdminDecision` 。</span><span class="sxs-lookup"><span data-stu-id="a1749-149">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="a1749-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a1749-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1749-152">示例</span><span class="sxs-lookup"><span data-stu-id="a1749-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1749-153">请求</span><span class="sxs-lookup"><span data-stu-id="a1749-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a1749-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1749-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="c"></a>[<span data-ttu-id="a1749-155">C#</span><span class="sxs-lookup"><span data-stu-id="a1749-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1749-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1749-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1749-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1749-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a><span data-ttu-id="a1749-158">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1749-158">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="a1749-159">响应</span><span class="sxs-lookup"><span data-stu-id="a1749-159">Response</span></span>
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
  ]
}
-->


