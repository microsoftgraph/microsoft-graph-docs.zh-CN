---
title: 取消 governanceRoleAssignmentRequest
description: 取消 governanceRoleAssignmentRequest。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identitiy-platform
ms.openlocfilehash: 576c75e88bf882d8836a0731457fc37b337b0037
ms.sourcegitcommit: d93fcc2212491567f8322b1cc0c02d37829b6051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/28/2020
ms.locfileid: "43034767"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="89512-103">取消 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="89512-103">Cancel governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="89512-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89512-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89512-105">取消[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="89512-105">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="89512-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="89512-106">Permissions</span></span>
<span data-ttu-id="89512-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89512-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89512-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="89512-109">Permission type</span></span>      | <span data-ttu-id="89512-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="89512-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89512-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89512-111">Delegated (work or school account)</span></span> | <span data-ttu-id="89512-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="89512-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="89512-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89512-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89512-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="89512-114">Not supported.</span></span>    |
|<span data-ttu-id="89512-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="89512-115">Application</span></span> | <span data-ttu-id="89512-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="89512-116">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="89512-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="89512-117">Optional query parameters</span></span>
<span data-ttu-id="89512-118">此方法**不**支持[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="89512-118">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="89512-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89512-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="89512-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="89512-120">Request headers</span></span>
| <span data-ttu-id="89512-121">名称</span><span class="sxs-lookup"><span data-stu-id="89512-121">Name</span></span>       | <span data-ttu-id="89512-122">说明</span><span class="sxs-lookup"><span data-stu-id="89512-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="89512-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="89512-123">Authorization</span></span>  | <span data-ttu-id="89512-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="89512-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="89512-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="89512-126">Content-type</span></span>  | <span data-ttu-id="89512-127">application/json</span><span class="sxs-lookup"><span data-stu-id="89512-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89512-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="89512-128">Request body</span></span>
<span data-ttu-id="89512-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="89512-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89512-130">响应</span><span class="sxs-lookup"><span data-stu-id="89512-130">Response</span></span>
<span data-ttu-id="89512-p103">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="89512-p103">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="89512-133">错误代码</span><span class="sxs-lookup"><span data-stu-id="89512-133">Error codes</span></span>
<span data-ttu-id="89512-134">此 API 遵循 HTTP 代码的标准。</span><span class="sxs-lookup"><span data-stu-id="89512-134">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="89512-135">此外，自定义错误代码如下所示。</span><span class="sxs-lookup"><span data-stu-id="89512-135">Besides, the custom error codes are shown below.</span></span>
| <span data-ttu-id="89512-136">错误代码</span><span class="sxs-lookup"><span data-stu-id="89512-136">Error code</span></span> | <span data-ttu-id="89512-137">错误消息</span><span class="sxs-lookup"><span data-stu-id="89512-137">Error message</span></span> | <span data-ttu-id="89512-138">详细信息</span><span class="sxs-lookup"><span data-stu-id="89512-138">Details</span></span> |
|:---------- |:------------- |:------- |
| <span data-ttu-id="89512-139">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="89512-139">400 BadRequest</span></span> | <span data-ttu-id="89512-140">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="89512-140">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="89512-141">GovernanceRoleAssignmentRequest 在系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="89512-141">The governanceRoleAssignmentRequest does not exist in system.</span></span> |
| <span data-ttu-id="89512-142">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="89512-142">400 BadRequest</span></span> | <span data-ttu-id="89512-143">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="89512-143">RequestCannotBeCancelled</span></span> | <span data-ttu-id="89512-144">仅`Granted`可以取消、 `PendingApproval` `PendingApprovalProvisioning`和和`PendingAdminDecision`的状态的请求。</span><span class="sxs-lookup"><span data-stu-id="89512-144">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span> |

## <a name="example"></a><span data-ttu-id="89512-145">示例</span><span class="sxs-lookup"><span data-stu-id="89512-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="89512-146">请求</span><span class="sxs-lookup"><span data-stu-id="89512-146">Request</span></span>
<span data-ttu-id="89512-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="89512-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="89512-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="89512-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="c"></a>[<span data-ttu-id="89512-149">C#</span><span class="sxs-lookup"><span data-stu-id="89512-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89512-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89512-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89512-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89512-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="89512-152">响应</span><span class="sxs-lookup"><span data-stu-id="89512-152">Response</span></span>
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
