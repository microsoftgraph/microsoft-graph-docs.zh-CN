---
title: 取消 governanceRoleAssignmentRequest
description: 取消 governanceRoleAssignmentRequest。
localization_priority: Normal
ms.openlocfilehash: 0437051a3d2550da8a8fe3e9984214ff7c885e3a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521731"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="9e072-103">取消 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="9e072-103">Cancel governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e072-104">取消[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="9e072-104">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9e072-105">权限</span><span class="sxs-lookup"><span data-stu-id="9e072-105">Permissions</span></span>
<span data-ttu-id="9e072-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9e072-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e072-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e072-108">Permission type</span></span>      | <span data-ttu-id="9e072-109">权限</span><span class="sxs-lookup"><span data-stu-id="9e072-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e072-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e072-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9e072-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9e072-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="9e072-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e072-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e072-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e072-113">Not supported.</span></span>    |
|<span data-ttu-id="9e072-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e072-114">Application</span></span> | <span data-ttu-id="9e072-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9e072-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="9e072-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9e072-116">Optional query parameters</span></span>
<span data-ttu-id="9e072-117">该方法**不**支持 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9e072-117">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="9e072-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e072-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="9e072-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e072-119">Request headers</span></span>
| <span data-ttu-id="9e072-120">名称</span><span class="sxs-lookup"><span data-stu-id="9e072-120">Name</span></span>       | <span data-ttu-id="9e072-121">说明</span><span class="sxs-lookup"><span data-stu-id="9e072-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9e072-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e072-122">Authorization</span></span>  | <span data-ttu-id="9e072-123">持有者 {code}</span><span class="sxs-lookup"><span data-stu-id="9e072-123">Bearer {code}</span></span>|
| <span data-ttu-id="9e072-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="9e072-124">Content-type</span></span>  | <span data-ttu-id="9e072-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e072-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e072-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e072-126">Request body</span></span>
<span data-ttu-id="9e072-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9e072-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e072-128">响应</span><span class="sxs-lookup"><span data-stu-id="9e072-128">Response</span></span>
<span data-ttu-id="9e072-p102">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9e072-p102">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="9e072-131">错误代码</span><span class="sxs-lookup"><span data-stu-id="9e072-131">Error codes</span></span>
<span data-ttu-id="9e072-132">此 API 遵循标准的 HTTP 代码。</span><span class="sxs-lookup"><span data-stu-id="9e072-132">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="9e072-133">此外，如下所示的自定义的错误代码。</span><span class="sxs-lookup"><span data-stu-id="9e072-133">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="9e072-134">错误代码</span><span class="sxs-lookup"><span data-stu-id="9e072-134">Error code</span></span>     | <span data-ttu-id="9e072-135">错误消息</span><span class="sxs-lookup"><span data-stu-id="9e072-135">Error message</span></span>              | <span data-ttu-id="9e072-136">详细信息</span><span class="sxs-lookup"><span data-stu-id="9e072-136">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="9e072-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9e072-137">400 BadRequest</span></span> | <span data-ttu-id="9e072-138">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="9e072-138">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="9e072-139">GovernanceRoleAssignmentRequest 系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="9e072-139">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="9e072-140">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9e072-140">400 BadRequest</span></span> | <span data-ttu-id="9e072-141">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="9e072-141">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="9e072-142">只请求的状态在`Granted`， `PendingApproval`，`PendingApprovalProvisioning`和`PendingAdminDecision`可以取消。</span><span class="sxs-lookup"><span data-stu-id="9e072-142">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="9e072-143">示例</span><span class="sxs-lookup"><span data-stu-id="9e072-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e072-144">请求</span><span class="sxs-lookup"><span data-stu-id="9e072-144">Request</span></span>
<span data-ttu-id="9e072-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e072-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a><span data-ttu-id="9e072-146">响应</span><span class="sxs-lookup"><span data-stu-id="9e072-146">Response</span></span>
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
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-cancel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
