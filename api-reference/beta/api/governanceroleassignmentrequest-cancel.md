---
title: 取消 governanceRoleAssignmentRequest
description: 取消 governanceRoleAssignmentRequest。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: e2f245766c826b8776504f0835a79a33b370aaba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421121"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="9dff8-103">取消 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="9dff8-103">Cancel governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="9dff8-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9dff8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dff8-105">取消[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="9dff8-105">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9dff8-106">权限</span><span class="sxs-lookup"><span data-stu-id="9dff8-106">Permissions</span></span>
<span data-ttu-id="9dff8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9dff8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dff8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9dff8-109">Permission type</span></span>      | <span data-ttu-id="9dff8-110">权限</span><span class="sxs-lookup"><span data-stu-id="9dff8-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9dff8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9dff8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9dff8-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9dff8-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="9dff8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9dff8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9dff8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9dff8-114">Not supported.</span></span>    |
|<span data-ttu-id="9dff8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9dff8-115">Application</span></span> | <span data-ttu-id="9dff8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9dff8-116">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="9dff8-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9dff8-117">Optional query parameters</span></span>
<span data-ttu-id="9dff8-118">此方法**不**支持[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9dff8-118">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="9dff8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9dff8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="9dff8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9dff8-120">Request headers</span></span>
| <span data-ttu-id="9dff8-121">名称</span><span class="sxs-lookup"><span data-stu-id="9dff8-121">Name</span></span>       | <span data-ttu-id="9dff8-122">说明</span><span class="sxs-lookup"><span data-stu-id="9dff8-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9dff8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9dff8-123">Authorization</span></span>  | <span data-ttu-id="9dff8-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9dff8-124">Bearer {code}</span></span>|
| <span data-ttu-id="9dff8-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="9dff8-125">Content-type</span></span>  | <span data-ttu-id="9dff8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9dff8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dff8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9dff8-127">Request body</span></span>
<span data-ttu-id="9dff8-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9dff8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9dff8-129">响应</span><span class="sxs-lookup"><span data-stu-id="9dff8-129">Response</span></span>
<span data-ttu-id="9dff8-p102">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9dff8-p102">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="9dff8-132">错误代码</span><span class="sxs-lookup"><span data-stu-id="9dff8-132">Error codes</span></span>
<span data-ttu-id="9dff8-133">此 API 遵循 HTTP 代码的标准。</span><span class="sxs-lookup"><span data-stu-id="9dff8-133">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="9dff8-134">此外，自定义错误代码如下所示。</span><span class="sxs-lookup"><span data-stu-id="9dff8-134">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="9dff8-135">错误代码</span><span class="sxs-lookup"><span data-stu-id="9dff8-135">Error code</span></span>     | <span data-ttu-id="9dff8-136">错误消息</span><span class="sxs-lookup"><span data-stu-id="9dff8-136">Error message</span></span>              | <span data-ttu-id="9dff8-137">详细信息</span><span class="sxs-lookup"><span data-stu-id="9dff8-137">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="9dff8-138">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9dff8-138">400 BadRequest</span></span> | <span data-ttu-id="9dff8-139">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="9dff8-139">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="9dff8-140">GovernanceRoleAssignmentRequest 在系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="9dff8-140">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="9dff8-141">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9dff8-141">400 BadRequest</span></span> | <span data-ttu-id="9dff8-142">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="9dff8-142">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="9dff8-143">仅`Granted`可以取消、 `PendingApproval` `PendingApprovalProvisioning`和和`PendingAdminDecision`的状态的请求。</span><span class="sxs-lookup"><span data-stu-id="9dff8-143">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="9dff8-144">示例</span><span class="sxs-lookup"><span data-stu-id="9dff8-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9dff8-145">请求</span><span class="sxs-lookup"><span data-stu-id="9dff8-145">Request</span></span>
<span data-ttu-id="9dff8-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9dff8-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9dff8-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="9dff8-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="c"></a>[<span data-ttu-id="9dff8-148">C#</span><span class="sxs-lookup"><span data-stu-id="9dff8-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9dff8-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9dff8-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9dff8-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9dff8-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9dff8-151">响应</span><span class="sxs-lookup"><span data-stu-id="9dff8-151">Response</span></span>
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
