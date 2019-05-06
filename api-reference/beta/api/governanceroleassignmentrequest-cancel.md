---
title: 取消 governanceRoleAssignmentRequest
description: 取消 governanceRoleAssignmentRequest。
localization_priority: Normal
ms.openlocfilehash: 4972c1f283c08b1304c6a01fdc0acc1d6942aec1
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593512"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="5c3d7-103">取消 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="5c3d7-103">Cancel governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c3d7-104">取消[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="5c3d7-104">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5c3d7-105">权限</span><span class="sxs-lookup"><span data-stu-id="5c3d7-105">Permissions</span></span>
<span data-ttu-id="5c3d7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c3d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c3d7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c3d7-108">Permission type</span></span>      | <span data-ttu-id="5c3d7-109">权限</span><span class="sxs-lookup"><span data-stu-id="5c3d7-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c3d7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c3d7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5c3d7-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="5c3d7-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="5c3d7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c3d7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c3d7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c3d7-113">Not supported.</span></span>    |
|<span data-ttu-id="5c3d7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c3d7-114">Application</span></span> | <span data-ttu-id="5c3d7-115">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="5c3d7-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="5c3d7-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5c3d7-116">Optional query parameters</span></span>
<span data-ttu-id="5c3d7-117">此方法**不**支持[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5c3d7-117">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="5c3d7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c3d7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="5c3d7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c3d7-119">Request headers</span></span>
| <span data-ttu-id="5c3d7-120">名称</span><span class="sxs-lookup"><span data-stu-id="5c3d7-120">Name</span></span>       | <span data-ttu-id="5c3d7-121">说明</span><span class="sxs-lookup"><span data-stu-id="5c3d7-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5c3d7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c3d7-122">Authorization</span></span>  | <span data-ttu-id="5c3d7-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5c3d7-123">Bearer {code}</span></span>|
| <span data-ttu-id="5c3d7-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="5c3d7-124">Content-type</span></span>  | <span data-ttu-id="5c3d7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5c3d7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c3d7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c3d7-126">Request body</span></span>
<span data-ttu-id="5c3d7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5c3d7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c3d7-128">响应</span><span class="sxs-lookup"><span data-stu-id="5c3d7-128">Response</span></span>
<span data-ttu-id="5c3d7-p102">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5c3d7-p102">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="5c3d7-131">错误代码</span><span class="sxs-lookup"><span data-stu-id="5c3d7-131">Error codes</span></span>
<span data-ttu-id="5c3d7-132">此 API 遵循 HTTP 代码的标准。</span><span class="sxs-lookup"><span data-stu-id="5c3d7-132">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="5c3d7-133">此外, 自定义错误代码如下所示。</span><span class="sxs-lookup"><span data-stu-id="5c3d7-133">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="5c3d7-134">错误代码</span><span class="sxs-lookup"><span data-stu-id="5c3d7-134">Error code</span></span>     | <span data-ttu-id="5c3d7-135">错误消息</span><span class="sxs-lookup"><span data-stu-id="5c3d7-135">Error message</span></span>              | <span data-ttu-id="5c3d7-136">详细信息</span><span class="sxs-lookup"><span data-stu-id="5c3d7-136">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="5c3d7-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="5c3d7-137">400 BadRequest</span></span> | <span data-ttu-id="5c3d7-138">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="5c3d7-138">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="5c3d7-139">GovernanceRoleAssignmentRequest 在系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="5c3d7-139">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="5c3d7-140">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="5c3d7-140">400 BadRequest</span></span> | <span data-ttu-id="5c3d7-141">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="5c3d7-141">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="5c3d7-142">仅`Granted`可以取消、 `PendingApproval` `PendingApprovalProvisioning`和和`PendingAdminDecision`的状态的请求。</span><span class="sxs-lookup"><span data-stu-id="5c3d7-142">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="5c3d7-143">示例</span><span class="sxs-lookup"><span data-stu-id="5c3d7-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c3d7-144">请求</span><span class="sxs-lookup"><span data-stu-id="5c3d7-144">Request</span></span>
<span data-ttu-id="5c3d7-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5c3d7-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a><span data-ttu-id="5c3d7-146">响应</span><span class="sxs-lookup"><span data-stu-id="5c3d7-146">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5c3d7-147">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5c3d7-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5c3d7-148">语言</span><span class="sxs-lookup"><span data-stu-id="5c3d7-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/cancel_governanceroleassignmentrequest-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5c3d7-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="5c3d7-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/cancel_governanceroleassignmentrequest-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-cancel.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-cancel.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
