---
title: 取消 governanceRoleAssignmentRequest
description: 取消 governanceRoleAssignmentRequest。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 81a2b70d171bec25af28d4929fcfd7b5cce31e59
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326819"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="90352-103">取消 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="90352-103">Cancel governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90352-104">取消[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="90352-104">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="90352-105">权限</span><span class="sxs-lookup"><span data-stu-id="90352-105">Permissions</span></span>
<span data-ttu-id="90352-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90352-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90352-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="90352-108">Permission type</span></span>      | <span data-ttu-id="90352-109">权限</span><span class="sxs-lookup"><span data-stu-id="90352-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90352-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90352-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90352-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="90352-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="90352-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90352-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90352-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="90352-113">Not supported.</span></span>    |
|<span data-ttu-id="90352-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="90352-114">Application</span></span> | <span data-ttu-id="90352-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="90352-115">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="90352-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="90352-116">Optional query parameters</span></span>
<span data-ttu-id="90352-117">此方法**不**支持[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="90352-117">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="90352-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90352-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="90352-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="90352-119">Request headers</span></span>
| <span data-ttu-id="90352-120">名称</span><span class="sxs-lookup"><span data-stu-id="90352-120">Name</span></span>       | <span data-ttu-id="90352-121">说明</span><span class="sxs-lookup"><span data-stu-id="90352-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="90352-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="90352-122">Authorization</span></span>  | <span data-ttu-id="90352-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="90352-123">Bearer {code}</span></span>|
| <span data-ttu-id="90352-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="90352-124">Content-type</span></span>  | <span data-ttu-id="90352-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90352-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90352-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="90352-126">Request body</span></span>
<span data-ttu-id="90352-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="90352-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90352-128">响应</span><span class="sxs-lookup"><span data-stu-id="90352-128">Response</span></span>
<span data-ttu-id="90352-p102">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="90352-p102">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="90352-131">错误代码</span><span class="sxs-lookup"><span data-stu-id="90352-131">Error codes</span></span>
<span data-ttu-id="90352-132">此 API 遵循 HTTP 代码的标准。</span><span class="sxs-lookup"><span data-stu-id="90352-132">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="90352-133">此外, 自定义错误代码如下所示。</span><span class="sxs-lookup"><span data-stu-id="90352-133">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="90352-134">错误代码</span><span class="sxs-lookup"><span data-stu-id="90352-134">Error code</span></span>     | <span data-ttu-id="90352-135">错误消息</span><span class="sxs-lookup"><span data-stu-id="90352-135">Error message</span></span>              | <span data-ttu-id="90352-136">详细信息</span><span class="sxs-lookup"><span data-stu-id="90352-136">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="90352-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="90352-137">400 BadRequest</span></span> | <span data-ttu-id="90352-138">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="90352-138">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="90352-139">GovernanceRoleAssignmentRequest 在系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="90352-139">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="90352-140">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="90352-140">400 BadRequest</span></span> | <span data-ttu-id="90352-141">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="90352-141">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="90352-142">仅`Granted`可以取消、 `PendingApproval` `PendingApprovalProvisioning`和和`PendingAdminDecision`的状态的请求。</span><span class="sxs-lookup"><span data-stu-id="90352-142">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="90352-143">示例</span><span class="sxs-lookup"><span data-stu-id="90352-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90352-144">请求</span><span class="sxs-lookup"><span data-stu-id="90352-144">Request</span></span>
<span data-ttu-id="90352-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90352-145">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="90352-146">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="90352-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="90352-147">C#</span><span class="sxs-lookup"><span data-stu-id="90352-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90352-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90352-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="90352-149">目标-C</span><span class="sxs-lookup"><span data-stu-id="90352-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="90352-150">Java</span><span class="sxs-lookup"><span data-stu-id="90352-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cancel-governanceroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="90352-151">响应</span><span class="sxs-lookup"><span data-stu-id="90352-151">Response</span></span>
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
