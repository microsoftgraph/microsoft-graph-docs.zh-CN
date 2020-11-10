---
title: 取消 governanceRoleAssignmentRequest
description: 取消 governanceRoleAssignmentRequest。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 45894f30f9d88a45227c3d0098b00329678f35aa
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965502"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="e113d-103">取消 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="e113d-103">Cancel governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="e113d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e113d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e113d-105">取消 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="e113d-105">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e113d-106">权限</span><span class="sxs-lookup"><span data-stu-id="e113d-106">Permissions</span></span>
<span data-ttu-id="e113d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="e113d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="e113d-109">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="e113d-109">Azure resources</span></span>

| <span data-ttu-id="e113d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e113d-110">Permission type</span></span> | <span data-ttu-id="e113d-111">权限</span><span class="sxs-lookup"><span data-stu-id="e113d-111">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="e113d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e113d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e113d-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e113d-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="e113d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e113d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e113d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e113d-115">Not supported.</span></span> |
| <span data-ttu-id="e113d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e113d-116">Application</span></span> | <span data-ttu-id="e113d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e113d-117">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="e113d-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="e113d-118">Azure AD</span></span>

| <span data-ttu-id="e113d-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="e113d-119">Permission type</span></span> | <span data-ttu-id="e113d-120">权限</span><span class="sxs-lookup"><span data-stu-id="e113d-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="e113d-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e113d-121">Delegated (work or school account)</span></span> | <span data-ttu-id="e113d-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="e113d-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="e113d-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e113d-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e113d-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="e113d-124">Not supported.</span></span> |
| <span data-ttu-id="e113d-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="e113d-125">Application</span></span> | <span data-ttu-id="e113d-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="e113d-126">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="e113d-127">组</span><span class="sxs-lookup"><span data-stu-id="e113d-127">Groups</span></span>

|<span data-ttu-id="e113d-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="e113d-128">Permission type</span></span> | <span data-ttu-id="e113d-129">权限</span><span class="sxs-lookup"><span data-stu-id="e113d-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="e113d-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e113d-130">Delegated (work or school account)</span></span> | <span data-ttu-id="e113d-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="e113d-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="e113d-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e113d-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e113d-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="e113d-133">Not supported.</span></span> |
| <span data-ttu-id="e113d-134">应用程序</span><span class="sxs-lookup"><span data-stu-id="e113d-134">Application</span></span> | <span data-ttu-id="e113d-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="e113d-135">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="e113d-136">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e113d-136">Optional query parameters</span></span>
<span data-ttu-id="e113d-137">此方法 **不** 支持 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e113d-137">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="e113d-138">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e113d-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="e113d-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="e113d-139">Request headers</span></span>
| <span data-ttu-id="e113d-140">名称</span><span class="sxs-lookup"><span data-stu-id="e113d-140">Name</span></span>       | <span data-ttu-id="e113d-141">说明</span><span class="sxs-lookup"><span data-stu-id="e113d-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e113d-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="e113d-142">Authorization</span></span>  | <span data-ttu-id="e113d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e113d-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="e113d-145">Content-type</span><span class="sxs-lookup"><span data-stu-id="e113d-145">Content-type</span></span>  | <span data-ttu-id="e113d-146">application/json</span><span class="sxs-lookup"><span data-stu-id="e113d-146">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e113d-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="e113d-147">Request body</span></span>
<span data-ttu-id="e113d-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e113d-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e113d-149">响应</span><span class="sxs-lookup"><span data-stu-id="e113d-149">Response</span></span>
<span data-ttu-id="e113d-p103">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e113d-p103">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="e113d-152">错误代码</span><span class="sxs-lookup"><span data-stu-id="e113d-152">Error codes</span></span>
<span data-ttu-id="e113d-153">此 API 遵循 HTTP 代码的标准。</span><span class="sxs-lookup"><span data-stu-id="e113d-153">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="e113d-154">此外，自定义错误代码如下所示。</span><span class="sxs-lookup"><span data-stu-id="e113d-154">Besides, the custom error codes are shown below.</span></span>
| <span data-ttu-id="e113d-155">错误代码</span><span class="sxs-lookup"><span data-stu-id="e113d-155">Error code</span></span> | <span data-ttu-id="e113d-156">错误消息</span><span class="sxs-lookup"><span data-stu-id="e113d-156">Error message</span></span> | <span data-ttu-id="e113d-157">详细信息</span><span class="sxs-lookup"><span data-stu-id="e113d-157">Details</span></span> |
|:---------- |:------------- |:------- |
| <span data-ttu-id="e113d-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e113d-158">400 BadRequest</span></span> | <span data-ttu-id="e113d-159">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="e113d-159">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="e113d-160">GovernanceRoleAssignmentRequest 在系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="e113d-160">The governanceRoleAssignmentRequest does not exist in system.</span></span> |
| <span data-ttu-id="e113d-161">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e113d-161">400 BadRequest</span></span> | <span data-ttu-id="e113d-162">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="e113d-162">RequestCannotBeCancelled</span></span> | <span data-ttu-id="e113d-163">仅 `Granted` `PendingApproval` `PendingApprovalProvisioning` 可以取消、和和的状态的请求 `PendingAdminDecision` 。</span><span class="sxs-lookup"><span data-stu-id="e113d-163">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span> |

## <a name="example"></a><span data-ttu-id="e113d-164">示例</span><span class="sxs-lookup"><span data-stu-id="e113d-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="e113d-165">请求</span><span class="sxs-lookup"><span data-stu-id="e113d-165">Request</span></span>
<span data-ttu-id="e113d-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e113d-166">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e113d-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="e113d-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="c"></a>[<span data-ttu-id="e113d-168">C#</span><span class="sxs-lookup"><span data-stu-id="e113d-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e113d-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e113d-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e113d-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e113d-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e113d-171">Java</span><span class="sxs-lookup"><span data-stu-id="e113d-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cancel-governanceroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e113d-172">响应</span><span class="sxs-lookup"><span data-stu-id="e113d-172">Response</span></span>
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


