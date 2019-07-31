---
title: 取消 governanceRoleAssignmentRequest
description: 取消 governanceRoleAssignmentRequest。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 8c34e2e81882cbb9b01235c70a8e7554ea13fc53
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954212"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="93d3a-103">取消 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="93d3a-103">Cancel governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93d3a-104">取消[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="93d3a-104">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="93d3a-105">权限</span><span class="sxs-lookup"><span data-stu-id="93d3a-105">Permissions</span></span>
<span data-ttu-id="93d3a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="93d3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93d3a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="93d3a-108">Permission type</span></span>      | <span data-ttu-id="93d3a-109">权限</span><span class="sxs-lookup"><span data-stu-id="93d3a-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93d3a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93d3a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="93d3a-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="93d3a-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="93d3a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93d3a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93d3a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="93d3a-113">Not supported.</span></span>    |
|<span data-ttu-id="93d3a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="93d3a-114">Application</span></span> | <span data-ttu-id="93d3a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="93d3a-115">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="93d3a-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="93d3a-116">Optional query parameters</span></span>
<span data-ttu-id="93d3a-117">此方法**不**支持[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="93d3a-117">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="93d3a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93d3a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="93d3a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="93d3a-119">Request headers</span></span>
| <span data-ttu-id="93d3a-120">名称</span><span class="sxs-lookup"><span data-stu-id="93d3a-120">Name</span></span>       | <span data-ttu-id="93d3a-121">说明</span><span class="sxs-lookup"><span data-stu-id="93d3a-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="93d3a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="93d3a-122">Authorization</span></span>  | <span data-ttu-id="93d3a-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="93d3a-123">Bearer {code}</span></span>|
| <span data-ttu-id="93d3a-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="93d3a-124">Content-type</span></span>  | <span data-ttu-id="93d3a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="93d3a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93d3a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="93d3a-126">Request body</span></span>
<span data-ttu-id="93d3a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="93d3a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93d3a-128">响应</span><span class="sxs-lookup"><span data-stu-id="93d3a-128">Response</span></span>
<span data-ttu-id="93d3a-p102">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="93d3a-p102">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="93d3a-131">错误代码</span><span class="sxs-lookup"><span data-stu-id="93d3a-131">Error codes</span></span>
<span data-ttu-id="93d3a-132">此 API 遵循 HTTP 代码的标准。</span><span class="sxs-lookup"><span data-stu-id="93d3a-132">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="93d3a-133">此外, 自定义错误代码如下所示。</span><span class="sxs-lookup"><span data-stu-id="93d3a-133">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="93d3a-134">错误代码</span><span class="sxs-lookup"><span data-stu-id="93d3a-134">Error code</span></span>     | <span data-ttu-id="93d3a-135">错误消息</span><span class="sxs-lookup"><span data-stu-id="93d3a-135">Error message</span></span>              | <span data-ttu-id="93d3a-136">详细信息</span><span class="sxs-lookup"><span data-stu-id="93d3a-136">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="93d3a-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="93d3a-137">400 BadRequest</span></span> | <span data-ttu-id="93d3a-138">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="93d3a-138">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="93d3a-139">GovernanceRoleAssignmentRequest 在系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="93d3a-139">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="93d3a-140">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="93d3a-140">400 BadRequest</span></span> | <span data-ttu-id="93d3a-141">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="93d3a-141">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="93d3a-142">仅`Granted`可以取消、 `PendingApproval` `PendingApprovalProvisioning`和和`PendingAdminDecision`的状态的请求。</span><span class="sxs-lookup"><span data-stu-id="93d3a-142">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="93d3a-143">示例</span><span class="sxs-lookup"><span data-stu-id="93d3a-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93d3a-144">请求</span><span class="sxs-lookup"><span data-stu-id="93d3a-144">Request</span></span>
<span data-ttu-id="93d3a-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="93d3a-145">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="93d3a-146">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="93d3a-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="93d3a-147">C#</span><span class="sxs-lookup"><span data-stu-id="93d3a-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93d3a-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="93d3a-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="93d3a-149">目标-C</span><span class="sxs-lookup"><span data-stu-id="93d3a-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="93d3a-150">Java</span><span class="sxs-lookup"><span data-stu-id="93d3a-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cancel-governanceroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="93d3a-151">响应</span><span class="sxs-lookup"><span data-stu-id="93d3a-151">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
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
  "description": "Cancel governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
