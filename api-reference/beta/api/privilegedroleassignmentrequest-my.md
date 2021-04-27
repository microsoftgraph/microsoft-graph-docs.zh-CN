---
title: privilegedRoleAssignmentRequest： my
description: 获取请求者对请求角色分配权限。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: f627d7e6be3f79b7064370b9523c409882f5ca22
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037317"
---
# <a name="privilegedroleassignmentrequest-my"></a><span data-ttu-id="5c0c2-103">privilegedRoleAssignmentRequest： my</span><span class="sxs-lookup"><span data-stu-id="5c0c2-103">privilegedRoleAssignmentRequest: my</span></span>

<span data-ttu-id="5c0c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c0c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c0c2-105">获取请求者对请求角色分配权限。</span><span class="sxs-lookup"><span data-stu-id="5c0c2-105">Get the requester's privileged role assignment requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c0c2-106">权限</span><span class="sxs-lookup"><span data-stu-id="5c0c2-106">Permissions</span></span>
<span data-ttu-id="5c0c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c0c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c0c2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c0c2-109">Permission type</span></span>                        | <span data-ttu-id="5c0c2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5c0c2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c0c2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c0c2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5c0c2-112">PrivilegedAccess.ReadWrite.AzureAD、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5c0c2-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5c0c2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c0c2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c0c2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c0c2-114">Not supported.</span></span> |
|<span data-ttu-id="5c0c2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c0c2-115">Application</span></span>                            | <span data-ttu-id="5c0c2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c0c2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c0c2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c0c2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests/my
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5c0c2-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5c0c2-118">Optional query parameters</span></span>
<span data-ttu-id="5c0c2-119">此方法支持 [OData 查询参数](http://graph.microsoft.io/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5c0c2-119">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c0c2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c0c2-120">Request headers</span></span>
| <span data-ttu-id="5c0c2-121">名称</span><span class="sxs-lookup"><span data-stu-id="5c0c2-121">Name</span></span>      |<span data-ttu-id="5c0c2-122">说明</span><span class="sxs-lookup"><span data-stu-id="5c0c2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5c0c2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c0c2-123">Authorization</span></span>  | <span data-ttu-id="5c0c2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5c0c2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c0c2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c0c2-126">Request body</span></span>
<span data-ttu-id="5c0c2-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5c0c2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c0c2-128">响应</span><span class="sxs-lookup"><span data-stu-id="5c0c2-128">Response</span></span>
<span data-ttu-id="5c0c2-129">如果成功，此方法在 `200 OK` 响应正文中返回 [响应代码和 privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="5c0c2-129">If successful, this method returns `200 OK` response code and [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c0c2-130">示例</span><span class="sxs-lookup"><span data-stu-id="5c0c2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c0c2-131">请求</span><span class="sxs-lookup"><span data-stu-id="5c0c2-131">Request</span></span>
<span data-ttu-id="5c0c2-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5c0c2-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c0c2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c0c2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_my)"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/my
```
# <a name="c"></a>[<span data-ttu-id="5c0c2-134">C#</span><span class="sxs-lookup"><span data-stu-id="5c0c2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignmentrequest-my-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c0c2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c0c2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignmentrequest-my-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c0c2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c0c2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignmentrequest-my-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c0c2-137">Java</span><span class="sxs-lookup"><span data-stu-id="5c0c2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignmentrequest-my-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5c0c2-138">响应</span><span class="sxs-lookup"><span data-stu-id="5c0c2-138">Response</span></span>
<span data-ttu-id="5c0c2-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5c0c2-139">The following is an example of the response.</span></span> <span data-ttu-id="5c0c2-140">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5c0c2-140">Note: The response object shown here might be shortened for readability.</span></span>
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
         "userId": "Self",
         "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
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
        "userId": "Self",
        "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
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
  ]
}
-->


