---
title: 列出 privilegedRoleAssignmentRequests
description: '检索 privilegedRoleAssignmentRequest 的集合。 '
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 3f9627dc19ae2646b27845ee945f9be04b9172b2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051064"
---
# <a name="list-privilegedroleassignmentrequests"></a><span data-ttu-id="e5730-103">列出 privilegedRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="e5730-103">List privilegedRoleAssignmentRequests</span></span>

<span data-ttu-id="e5730-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5730-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5730-105">检索 [privilegedRoleAssignmentRequest 的集合](../resources/privilegedroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="e5730-105">Retrieve a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span> 

<span data-ttu-id="e5730-106">**注意：** 此请求者必须对资源角色分配一个资源。</span><span class="sxs-lookup"><span data-stu-id="e5730-106">**Note:** This requester must have at least one role assignment on the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5730-107">权限</span><span class="sxs-lookup"><span data-stu-id="e5730-107">Permissions</span></span>
<span data-ttu-id="e5730-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5730-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5730-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5730-110">Permission type</span></span>                        | <span data-ttu-id="e5730-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5730-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5730-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5730-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e5730-113">PrivilegedAccess.ReadWrite.AzureAD、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5730-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e5730-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5730-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5730-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5730-115">Not supported.</span></span> |
|<span data-ttu-id="e5730-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5730-116">Application</span></span>                            | <span data-ttu-id="e5730-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5730-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5730-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5730-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5730-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e5730-119">Optional query parameters</span></span>
<span data-ttu-id="e5730-120">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e5730-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5730-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5730-121">Request headers</span></span>
| <span data-ttu-id="e5730-122">名称</span><span class="sxs-lookup"><span data-stu-id="e5730-122">Name</span></span>      |<span data-ttu-id="e5730-123">说明</span><span class="sxs-lookup"><span data-stu-id="e5730-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e5730-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5730-124">Authorization</span></span>  | <span data-ttu-id="e5730-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5730-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5730-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5730-127">Request body</span></span>
<span data-ttu-id="e5730-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e5730-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5730-129">响应</span><span class="sxs-lookup"><span data-stu-id="e5730-129">Response</span></span>
<span data-ttu-id="e5730-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e5730-130">If successful, this method returns a `200 OK` response code and a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5730-131">示例</span><span class="sxs-lookup"><span data-stu-id="e5730-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5730-132">请求</span><span class="sxs-lookup"><span data-stu-id="e5730-132">Request</span></span>
<span data-ttu-id="e5730-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e5730-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e5730-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5730-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
```
# <a name="c"></a>[<span data-ttu-id="e5730-135">C#</span><span class="sxs-lookup"><span data-stu-id="e5730-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5730-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5730-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5730-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5730-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5730-138">Java</span><span class="sxs-lookup"><span data-stu-id="e5730-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e5730-139">响应</span><span class="sxs-lookup"><span data-stu-id="e5730-139">Response</span></span>
<span data-ttu-id="e5730-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e5730-140">The following is an example of the response.</span></span> <span data-ttu-id="e5730-141">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e5730-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "@odata.context":"https://https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests",
  "value":[
    {
      "schedule":{
        "type":"activation","startDateTime":"2018-02-07T22:55:00Z","endDateTime":null,"duration" : null
      },"id":"03ea0c3d-90a0-42d4-b220-11c049c506fb","userId": "Self","roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-02-07T22:17:37.2215343Z","status":"ApprovalAborted","duration":"1","reason":"Activate for testing","ticketNumber":"222","ticketSystem":"222"
    },{
      "schedule":{
        "type":"assignment","startDateTime":"2018-01-23T02:43:15.258242Z","endDateTime":null,"duration" : null
      },"id":"fe4450bb-6d28-4583-8fc4-25b0ea91daf5","userId": "Self","roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-01-23T02:42:55.628338Z","status":"Completed","duration":"1","reason":"asdf","ticketNumber":null,"ticketSystem":null
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


