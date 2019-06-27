---
title: 取消 governanceRoleAssignmentRequest
description: 取消 governanceRoleAssignmentRequest。
localization_priority: Normal
ms.openlocfilehash: 21446acdab943ac238154ee1631ccf7ffd2f8326
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263530"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="23446-103">取消 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="23446-103">Cancel governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23446-104">取消[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="23446-104">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="23446-105">权限</span><span class="sxs-lookup"><span data-stu-id="23446-105">Permissions</span></span>
<span data-ttu-id="23446-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="23446-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23446-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="23446-108">Permission type</span></span>      | <span data-ttu-id="23446-109">权限</span><span class="sxs-lookup"><span data-stu-id="23446-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23446-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23446-110">Delegated (work or school account)</span></span> | <span data-ttu-id="23446-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="23446-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="23446-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23446-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23446-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="23446-113">Not supported.</span></span>    |
|<span data-ttu-id="23446-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="23446-114">Application</span></span> | <span data-ttu-id="23446-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="23446-115">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="23446-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="23446-116">Optional query parameters</span></span>
<span data-ttu-id="23446-117">此方法**不**支持[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="23446-117">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="23446-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23446-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="23446-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="23446-119">Request headers</span></span>
| <span data-ttu-id="23446-120">名称</span><span class="sxs-lookup"><span data-stu-id="23446-120">Name</span></span>       | <span data-ttu-id="23446-121">说明</span><span class="sxs-lookup"><span data-stu-id="23446-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="23446-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="23446-122">Authorization</span></span>  | <span data-ttu-id="23446-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="23446-123">Bearer {code}</span></span>|
| <span data-ttu-id="23446-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="23446-124">Content-type</span></span>  | <span data-ttu-id="23446-125">application/json</span><span class="sxs-lookup"><span data-stu-id="23446-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23446-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="23446-126">Request body</span></span>
<span data-ttu-id="23446-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="23446-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23446-128">响应</span><span class="sxs-lookup"><span data-stu-id="23446-128">Response</span></span>
<span data-ttu-id="23446-p102">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="23446-p102">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="23446-131">错误代码</span><span class="sxs-lookup"><span data-stu-id="23446-131">Error codes</span></span>
<span data-ttu-id="23446-132">此 API 遵循 HTTP 代码的标准。</span><span class="sxs-lookup"><span data-stu-id="23446-132">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="23446-133">此外, 自定义错误代码如下所示。</span><span class="sxs-lookup"><span data-stu-id="23446-133">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="23446-134">错误代码</span><span class="sxs-lookup"><span data-stu-id="23446-134">Error code</span></span>     | <span data-ttu-id="23446-135">错误消息</span><span class="sxs-lookup"><span data-stu-id="23446-135">Error message</span></span>              | <span data-ttu-id="23446-136">详细信息</span><span class="sxs-lookup"><span data-stu-id="23446-136">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="23446-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="23446-137">400 BadRequest</span></span> | <span data-ttu-id="23446-138">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="23446-138">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="23446-139">GovernanceRoleAssignmentRequest 在系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="23446-139">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="23446-140">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="23446-140">400 BadRequest</span></span> | <span data-ttu-id="23446-141">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="23446-141">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="23446-142">仅`Granted`可以取消、 `PendingApproval` `PendingApprovalProvisioning`和和`PendingAdminDecision`的状态的请求。</span><span class="sxs-lookup"><span data-stu-id="23446-142">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="23446-143">示例</span><span class="sxs-lookup"><span data-stu-id="23446-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23446-144">请求</span><span class="sxs-lookup"><span data-stu-id="23446-144">Request</span></span>
<span data-ttu-id="23446-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="23446-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a><span data-ttu-id="23446-146">响应</span><span class="sxs-lookup"><span data-stu-id="23446-146">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="23446-147">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="23446-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="23446-148">C#</span><span class="sxs-lookup"><span data-stu-id="23446-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/cancel_governanceroleassignmentrequest-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23446-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="23446-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/cancel_governanceroleassignmentrequest-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="23446-150">目标-C</span><span class="sxs-lookup"><span data-stu-id="23446-150">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/cancel_governanceroleassignmentrequest-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-cancel.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-cancel.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-cancel.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
