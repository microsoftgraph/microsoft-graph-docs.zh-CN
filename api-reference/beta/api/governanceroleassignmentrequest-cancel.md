---
title: 取消 governanceRoleAssignmentRequest
description: 取消 governanceRoleAssignmentRequest。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 043eeb41f61dc08dffe5a3608bd3d8f7a2fae232
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350983"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="e3b4c-103">取消 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="e3b4c-103">Cancel governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="e3b4c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3b4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3b4c-105">取消 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="e3b4c-105">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3b4c-106">权限</span><span class="sxs-lookup"><span data-stu-id="e3b4c-106">Permissions</span></span>
<span data-ttu-id="e3b4c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="e3b4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="e3b4c-109">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="e3b4c-109">Azure resources</span></span>

| <span data-ttu-id="e3b4c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3b4c-110">Permission type</span></span> | <span data-ttu-id="e3b4c-111">权限</span><span class="sxs-lookup"><span data-stu-id="e3b4c-111">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="e3b4c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3b4c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e3b4c-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e3b4c-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="e3b4c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3b4c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3b4c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3b4c-115">Not supported.</span></span> |
| <span data-ttu-id="e3b4c-116">Application</span><span class="sxs-lookup"><span data-stu-id="e3b4c-116">Application</span></span> | <span data-ttu-id="e3b4c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3b4c-117">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="e3b4c-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="e3b4c-118">Azure AD</span></span>

| <span data-ttu-id="e3b4c-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3b4c-119">Permission type</span></span> | <span data-ttu-id="e3b4c-120">权限</span><span class="sxs-lookup"><span data-stu-id="e3b4c-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="e3b4c-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3b4c-121">Delegated (work or school account)</span></span> | <span data-ttu-id="e3b4c-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="e3b4c-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="e3b4c-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3b4c-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3b4c-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3b4c-124">Not supported.</span></span> |
| <span data-ttu-id="e3b4c-125">Application</span><span class="sxs-lookup"><span data-stu-id="e3b4c-125">Application</span></span> | <span data-ttu-id="e3b4c-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3b4c-126">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="e3b4c-127">组</span><span class="sxs-lookup"><span data-stu-id="e3b4c-127">Groups</span></span>

|<span data-ttu-id="e3b4c-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3b4c-128">Permission type</span></span> | <span data-ttu-id="e3b4c-129">权限</span><span class="sxs-lookup"><span data-stu-id="e3b4c-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="e3b4c-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3b4c-130">Delegated (work or school account)</span></span> | <span data-ttu-id="e3b4c-131">PrivilegedAccess.ReadWrite.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="e3b4c-131">PrivilegedAccess.ReadWrite.AzureADGroup</span></span> |
| <span data-ttu-id="e3b4c-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3b4c-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3b4c-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3b4c-133">Not supported.</span></span> |
| <span data-ttu-id="e3b4c-134">Application</span><span class="sxs-lookup"><span data-stu-id="e3b4c-134">Application</span></span> | <span data-ttu-id="e3b4c-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3b4c-135">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="e3b4c-136">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e3b4c-136">Optional query parameters</span></span>
<span data-ttu-id="e3b4c-137">此方法 **不支持**[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e3b4c-137">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="e3b4c-138">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3b4c-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="e3b4c-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3b4c-139">Request headers</span></span>
| <span data-ttu-id="e3b4c-140">名称</span><span class="sxs-lookup"><span data-stu-id="e3b4c-140">Name</span></span>       | <span data-ttu-id="e3b4c-141">说明</span><span class="sxs-lookup"><span data-stu-id="e3b4c-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e3b4c-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3b4c-142">Authorization</span></span>  | <span data-ttu-id="e3b4c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e3b4c-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="e3b4c-145">Content-type</span><span class="sxs-lookup"><span data-stu-id="e3b4c-145">Content-type</span></span>  | <span data-ttu-id="e3b4c-146">application/json</span><span class="sxs-lookup"><span data-stu-id="e3b4c-146">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3b4c-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3b4c-147">Request body</span></span>
<span data-ttu-id="e3b4c-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e3b4c-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3b4c-149">响应</span><span class="sxs-lookup"><span data-stu-id="e3b4c-149">Response</span></span>
<span data-ttu-id="e3b4c-p103">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e3b4c-p103">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="e3b4c-152">错误代码</span><span class="sxs-lookup"><span data-stu-id="e3b4c-152">Error codes</span></span>
<span data-ttu-id="e3b4c-153">此 API 遵循 HTTP 代码的标准。</span><span class="sxs-lookup"><span data-stu-id="e3b4c-153">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="e3b4c-154">此外，自定义错误代码如下所示。</span><span class="sxs-lookup"><span data-stu-id="e3b4c-154">Besides, the custom error codes are shown below.</span></span>

| <span data-ttu-id="e3b4c-155">错误代码</span><span class="sxs-lookup"><span data-stu-id="e3b4c-155">Error code</span></span> | <span data-ttu-id="e3b4c-156">错误消息</span><span class="sxs-lookup"><span data-stu-id="e3b4c-156">Error message</span></span> | <span data-ttu-id="e3b4c-157">详细信息</span><span class="sxs-lookup"><span data-stu-id="e3b4c-157">Details</span></span> |
|:---------- |:------------- |:------- |
| <span data-ttu-id="e3b4c-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e3b4c-158">400 BadRequest</span></span> | <span data-ttu-id="e3b4c-159">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="e3b4c-159">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="e3b4c-160">governanceRoleAssignmentRequest 在系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="e3b4c-160">The governanceRoleAssignmentRequest does not exist in system.</span></span> |
| <span data-ttu-id="e3b4c-161">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e3b4c-161">400 BadRequest</span></span> | <span data-ttu-id="e3b4c-162">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="e3b4c-162">RequestCannotBeCancelled</span></span> | <span data-ttu-id="e3b4c-163">仅状态为 、 `Granted` `PendingApproval` 和 `PendingApprovalProvisioning` `PendingAdminDecision` 的请求可以取消。</span><span class="sxs-lookup"><span data-stu-id="e3b4c-163">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span> |

## <a name="example"></a><span data-ttu-id="e3b4c-164">示例</span><span class="sxs-lookup"><span data-stu-id="e3b4c-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3b4c-165">请求</span><span class="sxs-lookup"><span data-stu-id="e3b4c-165">Request</span></span>
<span data-ttu-id="e3b4c-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e3b4c-166">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e3b4c-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3b4c-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="c"></a>[<span data-ttu-id="e3b4c-168">C#</span><span class="sxs-lookup"><span data-stu-id="e3b4c-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3b4c-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3b4c-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3b4c-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3b4c-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3b4c-171">Java</span><span class="sxs-lookup"><span data-stu-id="e3b4c-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cancel-governanceroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e3b4c-172">响应</span><span class="sxs-lookup"><span data-stu-id="e3b4c-172">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
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


