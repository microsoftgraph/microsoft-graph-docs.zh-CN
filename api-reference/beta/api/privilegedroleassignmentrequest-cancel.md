---
title: 取消 privilegedRoleAssignmentRequest
description: 取消 privilegedRoleAssignmentRequest。
ms.openlocfilehash: 99c1102235e93ca365dcdd0e619bcceac9f396f1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046201"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="ad0e4-103">取消 privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="ad0e4-103">Cancel privilegedRoleAssignmentRequest</span></span>

> <span data-ttu-id="ad0e4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ad0e4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad0e4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ad0e4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad0e4-106">取消[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="ad0e4-106">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ad0e4-107">权限</span><span class="sxs-lookup"><span data-stu-id="ad0e4-107">Permissions</span></span>
<span data-ttu-id="ad0e4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad0e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad0e4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad0e4-110">Permission type</span></span>                        | <span data-ttu-id="ad0e4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad0e4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad0e4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad0e4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ad0e4-113">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ad0e4-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ad0e4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad0e4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad0e4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad0e4-115">Not supported.</span></span> |
|<span data-ttu-id="ad0e4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad0e4-116">Application</span></span>                            | <span data-ttu-id="ad0e4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad0e4-117">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="ad0e4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad0e4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="ad0e4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad0e4-119">Request headers</span></span>
| <span data-ttu-id="ad0e4-120">名称</span><span class="sxs-lookup"><span data-stu-id="ad0e4-120">Name</span></span>      |<span data-ttu-id="ad0e4-121">说明</span><span class="sxs-lookup"><span data-stu-id="ad0e4-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ad0e4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad0e4-122">Authorization</span></span>  | <span data-ttu-id="ad0e4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ad0e4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad0e4-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad0e4-125">Request body</span></span>
<span data-ttu-id="ad0e4-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ad0e4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad0e4-127">响应</span><span class="sxs-lookup"><span data-stu-id="ad0e4-127">Response</span></span>
<span data-ttu-id="ad0e4-128">如果成功，此方法返回 `200 Ok` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ad0e4-128">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="ad0e4-129">返回 [privilegedRoleAssignmentRequest] (.../ resources/privilegedRoleAssignmentRequest.md) 响应正文中。</span><span class="sxs-lookup"><span data-stu-id="ad0e4-129">It returns [privilegedRoleAssignmentRequest] (../resources/privilegedRoleAssignmentRequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="ad0e4-130">错误代码</span><span class="sxs-lookup"><span data-stu-id="ad0e4-130">Error codes</span></span>
<span data-ttu-id="ad0e4-131">此 API 返回的标准 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="ad0e4-131">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="ad0e4-132">此外，将返回下表中列出的自定义的错误代码。</span><span class="sxs-lookup"><span data-stu-id="ad0e4-132">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="ad0e4-133">错误代码</span><span class="sxs-lookup"><span data-stu-id="ad0e4-133">Error code</span></span>     | <span data-ttu-id="ad0e4-134">错误消息</span><span class="sxs-lookup"><span data-stu-id="ad0e4-134">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="ad0e4-135">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ad0e4-135">400 BadRequest</span></span> | <span data-ttu-id="ad0e4-136">了申请 Id 不能为 Null。</span><span class="sxs-lookup"><span data-stu-id="ad0e4-136">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="ad0e4-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ad0e4-137">400 BadRequest</span></span> | <span data-ttu-id="ad0e4-138">请求找不到请求 ID。</span><span class="sxs-lookup"><span data-stu-id="ad0e4-138">Request with request ID not found.</span></span> |
| <span data-ttu-id="ad0e4-139">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ad0e4-139">400 BadRequest</span></span> | <span data-ttu-id="ad0e4-140">计划和 PendingApproval，可以仅上状态完成取消。</span><span class="sxs-lookup"><span data-stu-id="ad0e4-140">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="ad0e4-141">未经授权的 403</span><span class="sxs-lookup"><span data-stu-id="ad0e4-141">403 UnAuthorized</span></span> | <span data-ttu-id="ad0e4-142">不允许进行取消呼叫或找不到请求的请求者。</span><span class="sxs-lookup"><span data-stu-id="ad0e4-142">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="ad0e4-143">示例</span><span class="sxs-lookup"><span data-stu-id="ad0e4-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad0e4-144">请求</span><span class="sxs-lookup"><span data-stu-id="ad0e4-144">Request</span></span>
<span data-ttu-id="ad0e4-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ad0e4-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests('7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee')/cancel
```

##### <a name="response"></a><span data-ttu-id="ad0e4-146">响应</span><span class="sxs-lookup"><span data-stu-id="ad0e4-146">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequests"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests/$entity",
    "schedule": {
        "type": "activation",
        "startDateTime": "2018-02-08T02:35:17.903Z",
        "endDateTime": null,
        "duration" : null
    },
    "id": "bcfb11e3-fc0d-49ea-b3d5-7d60a48e5043",
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
    "status": "Cancelling",
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "userId": "Self"，
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Cancel privilegedRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
