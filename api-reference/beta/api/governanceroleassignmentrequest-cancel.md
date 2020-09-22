---
title: 取消 governanceRoleAssignmentRequest
description: 取消 governanceRoleAssignmentRequest。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 942ff054ab3465077bf4ace0f267121e8b7ce8e4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991129"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="f4975-103">取消 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f4975-103">Cancel governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="f4975-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4975-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4975-105">取消 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="f4975-105">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f4975-106">权限</span><span class="sxs-lookup"><span data-stu-id="f4975-106">Permissions</span></span>
<span data-ttu-id="f4975-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4975-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4975-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4975-109">Permission type</span></span>      | <span data-ttu-id="f4975-110">权限</span><span class="sxs-lookup"><span data-stu-id="f4975-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4975-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4975-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f4975-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f4975-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="f4975-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4975-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4975-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4975-114">Not supported.</span></span>    |
|<span data-ttu-id="f4975-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4975-115">Application</span></span> | <span data-ttu-id="f4975-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4975-116">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="f4975-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f4975-117">Optional query parameters</span></span>
<span data-ttu-id="f4975-118">此方法 **不** 支持 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f4975-118">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="f4975-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4975-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="f4975-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4975-120">Request headers</span></span>
| <span data-ttu-id="f4975-121">名称</span><span class="sxs-lookup"><span data-stu-id="f4975-121">Name</span></span>       | <span data-ttu-id="f4975-122">说明</span><span class="sxs-lookup"><span data-stu-id="f4975-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f4975-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4975-123">Authorization</span></span>  | <span data-ttu-id="f4975-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f4975-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="f4975-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="f4975-126">Content-type</span></span>  | <span data-ttu-id="f4975-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f4975-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4975-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4975-128">Request body</span></span>
<span data-ttu-id="f4975-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f4975-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4975-130">响应</span><span class="sxs-lookup"><span data-stu-id="f4975-130">Response</span></span>
<span data-ttu-id="f4975-p103">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f4975-p103">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="f4975-133">错误代码</span><span class="sxs-lookup"><span data-stu-id="f4975-133">Error codes</span></span>
<span data-ttu-id="f4975-134">此 API 遵循 HTTP 代码的标准。</span><span class="sxs-lookup"><span data-stu-id="f4975-134">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="f4975-135">此外，自定义错误代码如下所示。</span><span class="sxs-lookup"><span data-stu-id="f4975-135">Besides, the custom error codes are shown below.</span></span>
| <span data-ttu-id="f4975-136">错误代码</span><span class="sxs-lookup"><span data-stu-id="f4975-136">Error code</span></span> | <span data-ttu-id="f4975-137">错误消息</span><span class="sxs-lookup"><span data-stu-id="f4975-137">Error message</span></span> | <span data-ttu-id="f4975-138">详细信息</span><span class="sxs-lookup"><span data-stu-id="f4975-138">Details</span></span> |
|:---------- |:------------- |:------- |
| <span data-ttu-id="f4975-139">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f4975-139">400 BadRequest</span></span> | <span data-ttu-id="f4975-140">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="f4975-140">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="f4975-141">GovernanceRoleAssignmentRequest 在系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="f4975-141">The governanceRoleAssignmentRequest does not exist in system.</span></span> |
| <span data-ttu-id="f4975-142">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f4975-142">400 BadRequest</span></span> | <span data-ttu-id="f4975-143">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="f4975-143">RequestCannotBeCancelled</span></span> | <span data-ttu-id="f4975-144">仅 `Granted` `PendingApproval` `PendingApprovalProvisioning` 可以取消、和和的状态的请求 `PendingAdminDecision` 。</span><span class="sxs-lookup"><span data-stu-id="f4975-144">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span> |

## <a name="example"></a><span data-ttu-id="f4975-145">示例</span><span class="sxs-lookup"><span data-stu-id="f4975-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="f4975-146">请求</span><span class="sxs-lookup"><span data-stu-id="f4975-146">Request</span></span>
<span data-ttu-id="f4975-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f4975-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f4975-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4975-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="c"></a>[<span data-ttu-id="f4975-149">C#</span><span class="sxs-lookup"><span data-stu-id="f4975-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4975-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4975-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4975-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4975-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f4975-152">响应</span><span class="sxs-lookup"><span data-stu-id="f4975-152">Response</span></span>
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


