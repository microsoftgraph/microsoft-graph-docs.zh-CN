---
title: 取消 governanceRoleAssignmentRequest
description: 取消 governanceRoleAssignmentRequest。
localization_priority: Normal
ms.openlocfilehash: f155a832a0c29935216dbc740e7db6ae8708f429
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809105"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="1bbeb-103">取消 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="1bbeb-103">Cancel governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="1bbeb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1bbeb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1bbeb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1bbeb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1bbeb-106">取消[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="1bbeb-106">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1bbeb-107">权限</span><span class="sxs-lookup"><span data-stu-id="1bbeb-107">Permissions</span></span>
<span data-ttu-id="1bbeb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1bbeb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bbeb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1bbeb-110">Permission type</span></span>      | <span data-ttu-id="1bbeb-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="1bbeb-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bbeb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1bbeb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1bbeb-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="1bbeb-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="1bbeb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1bbeb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bbeb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bbeb-115">Not supported.</span></span>    |
|<span data-ttu-id="1bbeb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1bbeb-116">Application</span></span> | <span data-ttu-id="1bbeb-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="1bbeb-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="1bbeb-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1bbeb-118">Optional query parameters</span></span>
<span data-ttu-id="1bbeb-119">该方法**不**支持 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="1bbeb-119">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="1bbeb-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1bbeb-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="1bbeb-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1bbeb-121">Request headers</span></span>
| <span data-ttu-id="1bbeb-122">名称</span><span class="sxs-lookup"><span data-stu-id="1bbeb-122">Name</span></span>       | <span data-ttu-id="1bbeb-123">说明</span><span class="sxs-lookup"><span data-stu-id="1bbeb-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1bbeb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bbeb-124">Authorization</span></span>  | <span data-ttu-id="1bbeb-125">持有者 {code}</span><span class="sxs-lookup"><span data-stu-id="1bbeb-125">Bearer {code}</span></span>|
| <span data-ttu-id="1bbeb-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="1bbeb-126">Content-type</span></span>  | <span data-ttu-id="1bbeb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1bbeb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bbeb-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1bbeb-128">Request body</span></span>
<span data-ttu-id="1bbeb-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1bbeb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bbeb-130">响应</span><span class="sxs-lookup"><span data-stu-id="1bbeb-130">Response</span></span>
<span data-ttu-id="1bbeb-p103">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1bbeb-p103">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="1bbeb-133">错误代码</span><span class="sxs-lookup"><span data-stu-id="1bbeb-133">Error codes</span></span>
<span data-ttu-id="1bbeb-134">此 API 遵循标准的 HTTP 代码。</span><span class="sxs-lookup"><span data-stu-id="1bbeb-134">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="1bbeb-135">此外，如下所示的自定义的错误代码。</span><span class="sxs-lookup"><span data-stu-id="1bbeb-135">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="1bbeb-136">错误代码</span><span class="sxs-lookup"><span data-stu-id="1bbeb-136">Error code</span></span>     | <span data-ttu-id="1bbeb-137">错误消息</span><span class="sxs-lookup"><span data-stu-id="1bbeb-137">Error message</span></span>              | <span data-ttu-id="1bbeb-138">详细信息</span><span class="sxs-lookup"><span data-stu-id="1bbeb-138">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="1bbeb-139">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="1bbeb-139">400 BadRequest</span></span> | <span data-ttu-id="1bbeb-140">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="1bbeb-140">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="1bbeb-141">GovernanceRoleAssignmentRequest 系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="1bbeb-141">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="1bbeb-142">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="1bbeb-142">400 BadRequest</span></span> | <span data-ttu-id="1bbeb-143">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="1bbeb-143">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="1bbeb-144">只请求的状态在`Granted`， `PendingApproval`，`PendingApprovalProvisioning`和`PendingAdminDecision`可以取消。</span><span class="sxs-lookup"><span data-stu-id="1bbeb-144">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="1bbeb-145">示例</span><span class="sxs-lookup"><span data-stu-id="1bbeb-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bbeb-146">请求</span><span class="sxs-lookup"><span data-stu-id="1bbeb-146">Request</span></span>
<span data-ttu-id="1bbeb-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1bbeb-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a><span data-ttu-id="1bbeb-148">响应</span><span class="sxs-lookup"><span data-stu-id="1bbeb-148">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Cancel governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
