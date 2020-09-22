---
title: 取消 privilegedRoleAssignmentRequest
description: 取消 privilegedRoleAssignmentRequest。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: abb1bbd8c7d8c866ab1149d7a3c2ed810dcc4fde
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034985"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="5b6d1-103">取消 privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="5b6d1-103">Cancel privilegedRoleAssignmentRequest</span></span>

<span data-ttu-id="5b6d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b6d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b6d1-105">取消 [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="5b6d1-105">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b6d1-106">权限</span><span class="sxs-lookup"><span data-stu-id="5b6d1-106">Permissions</span></span>
<span data-ttu-id="5b6d1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b6d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b6d1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b6d1-109">Permission type</span></span>                        | <span data-ttu-id="5b6d1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5b6d1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b6d1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b6d1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5b6d1-112">PrivilegedAccess 的 AzureAD、Directory.accessasuser.all</span><span class="sxs-lookup"><span data-stu-id="5b6d1-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5b6d1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b6d1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b6d1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b6d1-114">Not supported.</span></span> |
|<span data-ttu-id="5b6d1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b6d1-115">Application</span></span>                            | <span data-ttu-id="5b6d1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b6d1-116">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="5b6d1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b6d1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="5b6d1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b6d1-118">Request headers</span></span>
| <span data-ttu-id="5b6d1-119">名称</span><span class="sxs-lookup"><span data-stu-id="5b6d1-119">Name</span></span>      |<span data-ttu-id="5b6d1-120">说明</span><span class="sxs-lookup"><span data-stu-id="5b6d1-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5b6d1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b6d1-121">Authorization</span></span>  | <span data-ttu-id="5b6d1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5b6d1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b6d1-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b6d1-124">Request body</span></span>
<span data-ttu-id="5b6d1-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5b6d1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b6d1-126">响应</span><span class="sxs-lookup"><span data-stu-id="5b6d1-126">Response</span></span>
<span data-ttu-id="5b6d1-127">如果成功，此方法返回 `200 Ok` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5b6d1-127">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="5b6d1-128">它在响应正文中返回 [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) 。</span><span class="sxs-lookup"><span data-stu-id="5b6d1-128">It returns [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="5b6d1-129">错误代码</span><span class="sxs-lookup"><span data-stu-id="5b6d1-129">Error codes</span></span>
<span data-ttu-id="5b6d1-130">此 API 返回标准的 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="5b6d1-130">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="5b6d1-131">此外，它还返回下表中列出的自定义错误代码。</span><span class="sxs-lookup"><span data-stu-id="5b6d1-131">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="5b6d1-132">错误代码</span><span class="sxs-lookup"><span data-stu-id="5b6d1-132">Error code</span></span>     | <span data-ttu-id="5b6d1-133">错误消息</span><span class="sxs-lookup"><span data-stu-id="5b6d1-133">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="5b6d1-134">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="5b6d1-134">400 BadRequest</span></span> | <span data-ttu-id="5b6d1-135">RequestId 不能为 Null。</span><span class="sxs-lookup"><span data-stu-id="5b6d1-135">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="5b6d1-136">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="5b6d1-136">400 BadRequest</span></span> | <span data-ttu-id="5b6d1-137">找不到请求 ID 的请求。</span><span class="sxs-lookup"><span data-stu-id="5b6d1-137">Request with request ID not found.</span></span> |
| <span data-ttu-id="5b6d1-138">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="5b6d1-138">400 BadRequest</span></span> | <span data-ttu-id="5b6d1-139">只能在状态为 "已计划" 和 "PendingApproval" 时执行取消。</span><span class="sxs-lookup"><span data-stu-id="5b6d1-139">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="5b6d1-140">403未经授权</span><span class="sxs-lookup"><span data-stu-id="5b6d1-140">403 UnAuthorized</span></span> | <span data-ttu-id="5b6d1-141">不允许请求者进行取消呼叫或找不到请求。</span><span class="sxs-lookup"><span data-stu-id="5b6d1-141">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="5b6d1-142">示例</span><span class="sxs-lookup"><span data-stu-id="5b6d1-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b6d1-143">请求</span><span class="sxs-lookup"><span data-stu-id="5b6d1-143">Request</span></span>
<span data-ttu-id="5b6d1-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5b6d1-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5b6d1-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b6d1-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="c"></a>[<span data-ttu-id="5b6d1-146">C#</span><span class="sxs-lookup"><span data-stu-id="5b6d1-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-privilegedroleassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b6d1-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b6d1-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-privilegedroleassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b6d1-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b6d1-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-privilegedroleassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5b6d1-149">响应</span><span class="sxs-lookup"><span data-stu-id="5b6d1-149">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
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
    "userId": "Self",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Cancel privilegedRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


