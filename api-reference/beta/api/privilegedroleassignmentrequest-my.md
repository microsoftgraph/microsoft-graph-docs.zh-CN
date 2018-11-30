---
title: privilegedRoleAssignmentRequest： 我
description: 获取请求者的特权的角色分配请求。
ms.openlocfilehash: a2e6ca655359594480e09127721813f73726e2e8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047924"
---
# <a name="privilegedroleassignmentrequest-my"></a><span data-ttu-id="8140d-103">privilegedRoleAssignmentRequest： 我</span><span class="sxs-lookup"><span data-stu-id="8140d-103">privilegedRoleAssignmentRequest: my</span></span>

> <span data-ttu-id="8140d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8140d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8140d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8140d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8140d-106">获取请求者的特权的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="8140d-106">Get the requester's privileged role assignment requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="8140d-107">权限</span><span class="sxs-lookup"><span data-stu-id="8140d-107">Permissions</span></span>
<span data-ttu-id="8140d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8140d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8140d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8140d-110">Permission type</span></span>                        | <span data-ttu-id="8140d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8140d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8140d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8140d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8140d-113">PrivilegedAccess.ReadWrite.AzureAD，Directory.Read.All，Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8140d-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8140d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8140d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8140d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8140d-115">Not supported.</span></span> |
|<span data-ttu-id="8140d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8140d-116">Application</span></span>                            | <span data-ttu-id="8140d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8140d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8140d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8140d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests/my
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8140d-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8140d-119">Optional query parameters</span></span>
<span data-ttu-id="8140d-120">此方法支持 [OData 查询参数](http://graph.microsoft.io/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8140d-120">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8140d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8140d-121">Request headers</span></span>
| <span data-ttu-id="8140d-122">名称</span><span class="sxs-lookup"><span data-stu-id="8140d-122">Name</span></span>      |<span data-ttu-id="8140d-123">说明</span><span class="sxs-lookup"><span data-stu-id="8140d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8140d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8140d-124">Authorization</span></span>  | <span data-ttu-id="8140d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8140d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8140d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8140d-127">Request body</span></span>
<span data-ttu-id="8140d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8140d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8140d-129">响应</span><span class="sxs-lookup"><span data-stu-id="8140d-129">Response</span></span>
<span data-ttu-id="8140d-130">如果成功，此方法返回`200 OK`响应正文中的响应代码和[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)集合的对象。</span><span class="sxs-lookup"><span data-stu-id="8140d-130">If successful, this method returns `200 OK` response code and [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8140d-131">示例</span><span class="sxs-lookup"><span data-stu-id="8140d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8140d-132">请求</span><span class="sxs-lookup"><span data-stu-id="8140d-132">Request</span></span>
<span data-ttu-id="8140d-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8140d-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_my)"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/my
```

##### <a name="response"></a><span data-ttu-id="8140d-134">响应</span><span class="sxs-lookup"><span data-stu-id="8140d-134">Response</span></span>
<span data-ttu-id="8140d-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8140d-135">The following is an example of the response.</span></span> <span data-ttu-id="8140d-136">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8140d-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8140d-137">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8140d-137">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests",
    "@odata.count": 4,
    "value": [{
        "schedule": {
            "type": "activation",
            "startDateTime": "2018-02-08T02:35:17.903Z",
            "endDateTime": null,
            "duration" : null
        },
        "id": "e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1",
         "userId": "Self"，
         "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
        "evaluateOnly": false,
        "type": "UserAdd",
        "assignmentState": "Active",
        "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
        "status": "RequestedApproval",
        "duration": "2",
        "reason": "Activate the role for business purpose",
        "ticketNumber": "234",
        "ticketSystem": "system",
        "roleInfo@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests('e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1')/roleInfo/$entity",
        "roleInfo": {
            "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
            "name": "Directory Readers"
        }
    }, {
        "schedule": {
            "type": "activation",
            "startDateTime": "2018-02-07T22:55:00Z",
            "endDateTime": null,
            "duration" : null
        },
        "id": "03ea0c3d-90a0-42d4-b220-11c049c506fb",
        "userId": "Self"，
        "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
        "evaluateOnly": false,
        "type": "UserAdd",
        "assignmentState": "Active",
        "requestedDateTime": "2018-02-07T22:17:37.2215343Z",
        "status": "ApprovalAborted",
        "duration": "1",
        "reason": "Activate for testing",
        "ticketNumber": "222",
        "ticketSystem": "222",
        "roleInfo@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests('03ea0c3d-90a0-42d4-b220-11c049c506fb')/roleInfo/$entity",
        "roleInfo": {
            "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
            "name": "Directory Readers"
        }
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
