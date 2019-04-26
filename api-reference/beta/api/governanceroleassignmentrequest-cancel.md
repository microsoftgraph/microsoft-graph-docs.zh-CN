---
title: 取消 governanceRoleAssignmentRequest
description: 取消 governanceRoleAssignmentRequest。
localization_priority: Normal
ms.openlocfilehash: d4573af27def33f11c4c20e11ce99a8b309581fb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329636"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="ee79e-103">取消 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="ee79e-103">Cancel governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee79e-104">取消[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="ee79e-104">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ee79e-105">权限</span><span class="sxs-lookup"><span data-stu-id="ee79e-105">Permissions</span></span>
<span data-ttu-id="ee79e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee79e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee79e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee79e-108">Permission type</span></span>      | <span data-ttu-id="ee79e-109">权限</span><span class="sxs-lookup"><span data-stu-id="ee79e-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee79e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee79e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ee79e-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="ee79e-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="ee79e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee79e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee79e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee79e-113">Not supported.</span></span>    |
|<span data-ttu-id="ee79e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee79e-114">Application</span></span> | <span data-ttu-id="ee79e-115">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="ee79e-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="ee79e-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ee79e-116">Optional query parameters</span></span>
<span data-ttu-id="ee79e-117">此方法**不**支持[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ee79e-117">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="ee79e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee79e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="ee79e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee79e-119">Request headers</span></span>
| <span data-ttu-id="ee79e-120">名称</span><span class="sxs-lookup"><span data-stu-id="ee79e-120">Name</span></span>       | <span data-ttu-id="ee79e-121">说明</span><span class="sxs-lookup"><span data-stu-id="ee79e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ee79e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee79e-122">Authorization</span></span>  | <span data-ttu-id="ee79e-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ee79e-123">Bearer {code}</span></span>|
| <span data-ttu-id="ee79e-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="ee79e-124">Content-type</span></span>  | <span data-ttu-id="ee79e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee79e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee79e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee79e-126">Request body</span></span>
<span data-ttu-id="ee79e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ee79e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee79e-128">响应</span><span class="sxs-lookup"><span data-stu-id="ee79e-128">Response</span></span>
<span data-ttu-id="ee79e-p102">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ee79e-p102">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="ee79e-131">错误代码</span><span class="sxs-lookup"><span data-stu-id="ee79e-131">Error codes</span></span>
<span data-ttu-id="ee79e-132">此 API 遵循 HTTP 代码的标准。</span><span class="sxs-lookup"><span data-stu-id="ee79e-132">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="ee79e-133">此外, 自定义错误代码如下所示。</span><span class="sxs-lookup"><span data-stu-id="ee79e-133">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="ee79e-134">错误代码</span><span class="sxs-lookup"><span data-stu-id="ee79e-134">Error code</span></span>     | <span data-ttu-id="ee79e-135">错误消息</span><span class="sxs-lookup"><span data-stu-id="ee79e-135">Error message</span></span>              | <span data-ttu-id="ee79e-136">详细信息</span><span class="sxs-lookup"><span data-stu-id="ee79e-136">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="ee79e-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ee79e-137">400 BadRequest</span></span> | <span data-ttu-id="ee79e-138">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="ee79e-138">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="ee79e-139">governanceRoleAssignmentRequest 在系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="ee79e-139">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="ee79e-140">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ee79e-140">400 BadRequest</span></span> | <span data-ttu-id="ee79e-141">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="ee79e-141">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="ee79e-142">仅`Granted`可以取消、 `PendingApproval` `PendingApprovalProvisioning`和和`PendingAdminDecision`的状态的请求。</span><span class="sxs-lookup"><span data-stu-id="ee79e-142">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="ee79e-143">示例</span><span class="sxs-lookup"><span data-stu-id="ee79e-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee79e-144">请求</span><span class="sxs-lookup"><span data-stu-id="ee79e-144">Request</span></span>
<span data-ttu-id="ee79e-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ee79e-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a><span data-ttu-id="ee79e-146">响应</span><span class="sxs-lookup"><span data-stu-id="ee79e-146">Response</span></span>
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
  "suppressions": []
}
-->
