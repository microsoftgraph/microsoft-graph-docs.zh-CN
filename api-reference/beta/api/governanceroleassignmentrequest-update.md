---
title: 更新 governanceRoleAssignmentRequests
description: 使管理员能够更新状态为的`AdminApproved` `PendingAdminDecision`governanceRoleAssignmentRequests `AdminDenied`上的决策 (或)。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 2f6581e8ea1b8823b7fa799a4eee69e00d2fc63e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419690"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="96038-103">更新 governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="96038-103">Update governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96038-104">使管理员能够更新状态为的`AdminApproved` `AdminDenied` `PendingAdminDecision` [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)上的决策 (或)。</span><span class="sxs-lookup"><span data-stu-id="96038-104">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="96038-105">权限</span><span class="sxs-lookup"><span data-stu-id="96038-105">Permissions</span></span>
<span data-ttu-id="96038-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96038-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="96038-108">**注意:** 此 API 还要求请求者在[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)所属的资源`Active`中至少有一个`owner`管理员`user access administrator`角色分配 (或)。</span><span class="sxs-lookup"><span data-stu-id="96038-108">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="96038-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="96038-109">Permission type</span></span>      | <span data-ttu-id="96038-110">权限</span><span class="sxs-lookup"><span data-stu-id="96038-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96038-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96038-111">Delegated (work or school account)</span></span> | <span data-ttu-id="96038-112">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="96038-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="96038-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96038-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96038-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="96038-114">Not supported.</span></span>    |
|<span data-ttu-id="96038-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="96038-115">Application</span></span> | <span data-ttu-id="96038-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="96038-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96038-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96038-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="96038-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="96038-118">Request headers</span></span>
| <span data-ttu-id="96038-119">名称</span><span class="sxs-lookup"><span data-stu-id="96038-119">Name</span></span>           | <span data-ttu-id="96038-120">说明</span><span class="sxs-lookup"><span data-stu-id="96038-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="96038-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="96038-121">Authorization</span></span>  | <span data-ttu-id="96038-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="96038-122">Bearer {code}</span></span>|
| <span data-ttu-id="96038-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="96038-123">Content-type</span></span>  | <span data-ttu-id="96038-124">application/json</span><span class="sxs-lookup"><span data-stu-id="96038-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96038-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="96038-125">Request body</span></span>

|<span data-ttu-id="96038-126">参数</span><span class="sxs-lookup"><span data-stu-id="96038-126">Parameters</span></span>      |<span data-ttu-id="96038-127">类型</span><span class="sxs-lookup"><span data-stu-id="96038-127">Type</span></span>                   |<span data-ttu-id="96038-128">必需</span><span class="sxs-lookup"><span data-stu-id="96038-128">Required</span></span> |<span data-ttu-id="96038-129">说明</span><span class="sxs-lookup"><span data-stu-id="96038-129">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="96038-130">在于</span><span class="sxs-lookup"><span data-stu-id="96038-130">reason</span></span>        |<span data-ttu-id="96038-131">String</span><span class="sxs-lookup"><span data-stu-id="96038-131">String</span></span>                 |<span data-ttu-id="96038-132">✓</span><span class="sxs-lookup"><span data-stu-id="96038-132">✓</span></span>        |<span data-ttu-id="96038-133">管理员为自己的决定提供的原因。</span><span class="sxs-lookup"><span data-stu-id="96038-133">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="96038-134">权</span><span class="sxs-lookup"><span data-stu-id="96038-134">decision</span></span>        |<span data-ttu-id="96038-135">String</span><span class="sxs-lookup"><span data-stu-id="96038-135">String</span></span>                 |<span data-ttu-id="96038-136">✓</span><span class="sxs-lookup"><span data-stu-id="96038-136">✓</span></span>        |<span data-ttu-id="96038-137">角色分配请求的管理员决定。</span><span class="sxs-lookup"><span data-stu-id="96038-137">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="96038-138">应将值更新为`AdminApproved`或。 `AdminDenied`</span><span class="sxs-lookup"><span data-stu-id="96038-138">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="96038-139">schedule</span><span class="sxs-lookup"><span data-stu-id="96038-139">schedule</span></span>      |[<span data-ttu-id="96038-140">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="96038-140">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="96038-141">角色分配请求的日程安排。</span><span class="sxs-lookup"><span data-stu-id="96038-141">The schedule of the role assignment request.</span></span> <span data-ttu-id="96038-142">对于的状态`AdminApproved`, 是必需的。</span><span class="sxs-lookup"><span data-stu-id="96038-142">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="96038-143">assignmentState</span><span class="sxs-lookup"><span data-stu-id="96038-143">assignmentState</span></span>      |<span data-ttu-id="96038-144">String</span><span class="sxs-lookup"><span data-stu-id="96038-144">String</span></span>|         | <span data-ttu-id="96038-145">工作分配的状态, 值可以是`Eligible`或。 `Active`</span><span class="sxs-lookup"><span data-stu-id="96038-145">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="96038-146">有关的决策`AdminApproved`, 则是必需的。</span><span class="sxs-lookup"><span data-stu-id="96038-146">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="96038-147">响应</span><span class="sxs-lookup"><span data-stu-id="96038-147">Response</span></span>
<span data-ttu-id="96038-148">此方法仅适用于状态为的`PendingAdminDecision`请求。</span><span class="sxs-lookup"><span data-stu-id="96038-148">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="96038-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="96038-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96038-151">示例</span><span class="sxs-lookup"><span data-stu-id="96038-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96038-152">请求</span><span class="sxs-lookup"><span data-stu-id="96038-152">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="96038-153">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="96038-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="96038-154">C#</span><span class="sxs-lookup"><span data-stu-id="96038-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96038-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96038-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96038-156">目标-C</span><span class="sxs-lookup"><span data-stu-id="96038-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a><span data-ttu-id="96038-157">请求正文</span><span class="sxs-lookup"><span data-stu-id="96038-157">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="96038-158">响应</span><span class="sxs-lookup"><span data-stu-id="96038-158">Response</span></span>
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
