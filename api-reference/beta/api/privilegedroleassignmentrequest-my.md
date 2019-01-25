---
title: privilegedRoleAssignmentRequest： 我
description: 获取请求者的特权的角色分配请求。
localization_priority: Normal
ms.openlocfilehash: 79545b5ea0ad88c55d7a09eb5c77982e812721eb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508865"
---
# <a name="privilegedroleassignmentrequest-my"></a><span data-ttu-id="f47b4-103">privilegedRoleAssignmentRequest： 我</span><span class="sxs-lookup"><span data-stu-id="f47b4-103">privilegedRoleAssignmentRequest: my</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f47b4-104">获取请求者的特权的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="f47b4-104">Get the requester's privileged role assignment requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="f47b4-105">权限</span><span class="sxs-lookup"><span data-stu-id="f47b4-105">Permissions</span></span>
<span data-ttu-id="f47b4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f47b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f47b4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f47b4-108">Permission type</span></span>                        | <span data-ttu-id="f47b4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f47b4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f47b4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f47b4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f47b4-111">PrivilegedAccess.ReadWrite.AzureAD，Directory.Read.All，Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f47b4-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f47b4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f47b4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f47b4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f47b4-113">Not supported.</span></span> |
|<span data-ttu-id="f47b4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f47b4-114">Application</span></span>                            | <span data-ttu-id="f47b4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f47b4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f47b4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f47b4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests/my
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f47b4-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f47b4-117">Optional query parameters</span></span>
<span data-ttu-id="f47b4-118">此方法支持 [OData 查询参数](http://graph.microsoft.io/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f47b4-118">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f47b4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f47b4-119">Request headers</span></span>
| <span data-ttu-id="f47b4-120">名称</span><span class="sxs-lookup"><span data-stu-id="f47b4-120">Name</span></span>      |<span data-ttu-id="f47b4-121">说明</span><span class="sxs-lookup"><span data-stu-id="f47b4-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f47b4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f47b4-122">Authorization</span></span>  | <span data-ttu-id="f47b4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f47b4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f47b4-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f47b4-125">Request body</span></span>
<span data-ttu-id="f47b4-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f47b4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f47b4-127">响应</span><span class="sxs-lookup"><span data-stu-id="f47b4-127">Response</span></span>
<span data-ttu-id="f47b4-128">如果成功，此方法返回`200 OK`响应正文中的响应代码和[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)集合的对象。</span><span class="sxs-lookup"><span data-stu-id="f47b4-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f47b4-129">示例</span><span class="sxs-lookup"><span data-stu-id="f47b4-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f47b4-130">请求</span><span class="sxs-lookup"><span data-stu-id="f47b4-130">Request</span></span>
<span data-ttu-id="f47b4-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f47b4-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_my)"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/my
```

##### <a name="response"></a><span data-ttu-id="f47b4-132">响应</span><span class="sxs-lookup"><span data-stu-id="f47b4-132">Response</span></span>
<span data-ttu-id="f47b4-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f47b4-133">The following is an example of the response.</span></span> <span data-ttu-id="f47b4-134">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f47b4-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f47b4-135">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f47b4-135">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-my.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
