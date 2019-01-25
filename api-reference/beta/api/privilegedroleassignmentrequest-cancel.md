---
title: 取消 privilegedRoleAssignmentRequest
description: 取消 privilegedRoleAssignmentRequest。
localization_priority: Normal
ms.openlocfilehash: 0cca3f33e6e027c18e24862dc4736006058f8e41
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528471"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="afe54-103">取消 privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="afe54-103">Cancel privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afe54-104">取消[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="afe54-104">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="afe54-105">权限</span><span class="sxs-lookup"><span data-stu-id="afe54-105">Permissions</span></span>
<span data-ttu-id="afe54-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="afe54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afe54-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="afe54-108">Permission type</span></span>                        | <span data-ttu-id="afe54-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="afe54-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="afe54-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="afe54-110">Delegated (work or school account)</span></span> | <span data-ttu-id="afe54-111">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="afe54-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="afe54-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="afe54-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afe54-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="afe54-113">Not supported.</span></span> |
|<span data-ttu-id="afe54-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="afe54-114">Application</span></span>                            | <span data-ttu-id="afe54-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="afe54-115">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="afe54-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="afe54-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="afe54-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="afe54-117">Request headers</span></span>
| <span data-ttu-id="afe54-118">名称</span><span class="sxs-lookup"><span data-stu-id="afe54-118">Name</span></span>      |<span data-ttu-id="afe54-119">说明</span><span class="sxs-lookup"><span data-stu-id="afe54-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="afe54-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="afe54-120">Authorization</span></span>  | <span data-ttu-id="afe54-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="afe54-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="afe54-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="afe54-123">Request body</span></span>
<span data-ttu-id="afe54-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="afe54-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afe54-125">响应</span><span class="sxs-lookup"><span data-stu-id="afe54-125">Response</span></span>
<span data-ttu-id="afe54-126">如果成功，此方法返回 `200 Ok` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="afe54-126">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="afe54-127">返回 [privilegedRoleAssignmentRequest] (.../ resources/privilegedRoleAssignmentRequest.md) 响应正文中。</span><span class="sxs-lookup"><span data-stu-id="afe54-127">It returns [privilegedRoleAssignmentRequest] (../resources/privilegedRoleAssignmentRequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="afe54-128">错误代码</span><span class="sxs-lookup"><span data-stu-id="afe54-128">Error codes</span></span>
<span data-ttu-id="afe54-129">此 API 返回的标准 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="afe54-129">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="afe54-130">此外，将返回下表中列出的自定义的错误代码。</span><span class="sxs-lookup"><span data-stu-id="afe54-130">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="afe54-131">错误代码</span><span class="sxs-lookup"><span data-stu-id="afe54-131">Error code</span></span>     | <span data-ttu-id="afe54-132">错误消息</span><span class="sxs-lookup"><span data-stu-id="afe54-132">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="afe54-133">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="afe54-133">400 BadRequest</span></span> | <span data-ttu-id="afe54-134">了申请 Id 不能为 Null。</span><span class="sxs-lookup"><span data-stu-id="afe54-134">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="afe54-135">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="afe54-135">400 BadRequest</span></span> | <span data-ttu-id="afe54-136">请求找不到请求 ID。</span><span class="sxs-lookup"><span data-stu-id="afe54-136">Request with request ID not found.</span></span> |
| <span data-ttu-id="afe54-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="afe54-137">400 BadRequest</span></span> | <span data-ttu-id="afe54-138">计划和 PendingApproval，可以仅上状态完成取消。</span><span class="sxs-lookup"><span data-stu-id="afe54-138">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="afe54-139">未经授权的 403</span><span class="sxs-lookup"><span data-stu-id="afe54-139">403 UnAuthorized</span></span> | <span data-ttu-id="afe54-140">不允许进行取消呼叫或找不到请求的请求者。</span><span class="sxs-lookup"><span data-stu-id="afe54-140">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="afe54-141">示例</span><span class="sxs-lookup"><span data-stu-id="afe54-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="afe54-142">请求</span><span class="sxs-lookup"><span data-stu-id="afe54-142">Request</span></span>
<span data-ttu-id="afe54-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="afe54-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests('7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee')/cancel
```

##### <a name="response"></a><span data-ttu-id="afe54-144">响应</span><span class="sxs-lookup"><span data-stu-id="afe54-144">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Cancel privilegedRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-cancel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
