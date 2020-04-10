---
title: 更新 governanceRoleAssignmentRequests
description: 使管理员能够更新状态为的`AdminApproved` `PendingAdminDecision`governanceRoleAssignmentRequests `AdminDenied`上的决策（或）。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: b726903082d8a3302e2be386206b76d741d89928
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218862"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="492c0-103">更新 governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="492c0-103">Update governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="492c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="492c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="492c0-105">使管理员能够更新状态为的`AdminApproved` `AdminDenied` `PendingAdminDecision` [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)上的决策（或）。</span><span class="sxs-lookup"><span data-stu-id="492c0-105">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="492c0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="492c0-106">Permissions</span></span>
<span data-ttu-id="492c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="492c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="492c0-109">**注意：** 此 API 还要求请求者在[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)所属的资源`Active`中至少有一个`owner`管理员`user access administrator`角色分配（或）。</span><span class="sxs-lookup"><span data-stu-id="492c0-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="492c0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="492c0-110">Permission type</span></span>      | <span data-ttu-id="492c0-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="492c0-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="492c0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="492c0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="492c0-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="492c0-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="492c0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="492c0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="492c0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="492c0-115">Not supported.</span></span>    |
|<span data-ttu-id="492c0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="492c0-116">Application</span></span> | <span data-ttu-id="492c0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="492c0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="492c0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="492c0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="492c0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="492c0-119">Request headers</span></span>
| <span data-ttu-id="492c0-120">名称</span><span class="sxs-lookup"><span data-stu-id="492c0-120">Name</span></span>           | <span data-ttu-id="492c0-121">说明</span><span class="sxs-lookup"><span data-stu-id="492c0-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="492c0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="492c0-122">Authorization</span></span>  | <span data-ttu-id="492c0-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="492c0-123">Bearer {code}</span></span>|
| <span data-ttu-id="492c0-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="492c0-124">Content-type</span></span>  | <span data-ttu-id="492c0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="492c0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="492c0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="492c0-126">Request body</span></span>

|<span data-ttu-id="492c0-127">参数</span><span class="sxs-lookup"><span data-stu-id="492c0-127">Parameters</span></span>      |<span data-ttu-id="492c0-128">类型</span><span class="sxs-lookup"><span data-stu-id="492c0-128">Type</span></span>                   |<span data-ttu-id="492c0-129">必需</span><span class="sxs-lookup"><span data-stu-id="492c0-129">Required</span></span> |<span data-ttu-id="492c0-130">说明</span><span class="sxs-lookup"><span data-stu-id="492c0-130">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="492c0-131">reason</span><span class="sxs-lookup"><span data-stu-id="492c0-131">reason</span></span>        |<span data-ttu-id="492c0-132">字符串</span><span class="sxs-lookup"><span data-stu-id="492c0-132">String</span></span>                 |<span data-ttu-id="492c0-133">✓</span><span class="sxs-lookup"><span data-stu-id="492c0-133">✓</span></span>        |<span data-ttu-id="492c0-134">管理员为自己的决定提供的原因。</span><span class="sxs-lookup"><span data-stu-id="492c0-134">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="492c0-135">权</span><span class="sxs-lookup"><span data-stu-id="492c0-135">decision</span></span>        |<span data-ttu-id="492c0-136">字符串</span><span class="sxs-lookup"><span data-stu-id="492c0-136">String</span></span>                 |<span data-ttu-id="492c0-137">✓</span><span class="sxs-lookup"><span data-stu-id="492c0-137">✓</span></span>        |<span data-ttu-id="492c0-138">角色分配请求的管理员决定。</span><span class="sxs-lookup"><span data-stu-id="492c0-138">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="492c0-139">应将值更新为`AdminApproved`或。 `AdminDenied`</span><span class="sxs-lookup"><span data-stu-id="492c0-139">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="492c0-140">schedule</span><span class="sxs-lookup"><span data-stu-id="492c0-140">schedule</span></span>      |[<span data-ttu-id="492c0-141">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="492c0-141">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="492c0-142">角色分配请求的日程安排。</span><span class="sxs-lookup"><span data-stu-id="492c0-142">The schedule of the role assignment request.</span></span> <span data-ttu-id="492c0-143">对于的状态`AdminApproved`，是必需的。</span><span class="sxs-lookup"><span data-stu-id="492c0-143">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="492c0-144">assignmentState</span><span class="sxs-lookup"><span data-stu-id="492c0-144">assignmentState</span></span>      |<span data-ttu-id="492c0-145">字符串</span><span class="sxs-lookup"><span data-stu-id="492c0-145">String</span></span>|         | <span data-ttu-id="492c0-146">工作分配的状态，值可以是`Eligible`或。 `Active`</span><span class="sxs-lookup"><span data-stu-id="492c0-146">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="492c0-147">有关的决策`AdminApproved`，则是必需的。</span><span class="sxs-lookup"><span data-stu-id="492c0-147">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="492c0-148">响应</span><span class="sxs-lookup"><span data-stu-id="492c0-148">Response</span></span>
<span data-ttu-id="492c0-149">此方法仅适用于状态为的`PendingAdminDecision`请求。</span><span class="sxs-lookup"><span data-stu-id="492c0-149">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="492c0-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="492c0-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="492c0-152">示例</span><span class="sxs-lookup"><span data-stu-id="492c0-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="492c0-153">请求</span><span class="sxs-lookup"><span data-stu-id="492c0-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="492c0-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="492c0-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="c"></a>[<span data-ttu-id="492c0-155">C#</span><span class="sxs-lookup"><span data-stu-id="492c0-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="492c0-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="492c0-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="492c0-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="492c0-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a><span data-ttu-id="492c0-158">请求正文</span><span class="sxs-lookup"><span data-stu-id="492c0-158">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="492c0-159">响应</span><span class="sxs-lookup"><span data-stu-id="492c0-159">Response</span></span>
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
