---
title: 列表 privilegedRoleAssignmentRequests
description: '检索 privilegedRoleAssignmentRequest 的集合。 '
localization_priority: Normal
ms.openlocfilehash: 4bae072caeb54c513e9146fe36dfd100ce1b4360
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838701"
---
# <a name="list-privilegedroleassignmentrequests"></a><span data-ttu-id="10ec1-103">列表 privilegedRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="10ec1-103">List privilegedRoleAssignmentRequests</span></span>

> <span data-ttu-id="10ec1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="10ec1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10ec1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="10ec1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="10ec1-106">检索[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="10ec1-106">Retrieve a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span> 

<span data-ttu-id="10ec1-107">**注意：** 此请求者必须具有对资源的至少一个角色分配。</span><span class="sxs-lookup"><span data-stu-id="10ec1-107">**Note:** This requester must have at least one role assignment on the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="10ec1-108">权限</span><span class="sxs-lookup"><span data-stu-id="10ec1-108">Permissions</span></span>
<span data-ttu-id="10ec1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10ec1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10ec1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="10ec1-111">Permission type</span></span>                        | <span data-ttu-id="10ec1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="10ec1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="10ec1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10ec1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="10ec1-114">PrivilegedAccess.ReadWrite.AzureAD，Directory.Read.All，Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="10ec1-114">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="10ec1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10ec1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10ec1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="10ec1-116">Not supported.</span></span> |
|<span data-ttu-id="10ec1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="10ec1-117">Application</span></span>                            | <span data-ttu-id="10ec1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="10ec1-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="10ec1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10ec1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10ec1-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="10ec1-120">Optional query parameters</span></span>
<span data-ttu-id="10ec1-121">此方法支持[OData 查询参数](/graph/query-parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="10ec1-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10ec1-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="10ec1-122">Request headers</span></span>
| <span data-ttu-id="10ec1-123">名称</span><span class="sxs-lookup"><span data-stu-id="10ec1-123">Name</span></span>      |<span data-ttu-id="10ec1-124">说明</span><span class="sxs-lookup"><span data-stu-id="10ec1-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="10ec1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="10ec1-125">Authorization</span></span>  | <span data-ttu-id="10ec1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="10ec1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10ec1-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="10ec1-128">Request body</span></span>
<span data-ttu-id="10ec1-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="10ec1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10ec1-130">响应</span><span class="sxs-lookup"><span data-stu-id="10ec1-130">Response</span></span>
<span data-ttu-id="10ec1-131">如果成功，此方法返回`200 OK`响应代码和响应正文中的[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="10ec1-131">If successful, this method returns a `200 OK` response code and a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10ec1-132">示例</span><span class="sxs-lookup"><span data-stu-id="10ec1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10ec1-133">请求</span><span class="sxs-lookup"><span data-stu-id="10ec1-133">Request</span></span>
<span data-ttu-id="10ec1-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="10ec1-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
```
##### <a name="response"></a><span data-ttu-id="10ec1-135">响应</span><span class="sxs-lookup"><span data-stu-id="10ec1-135">Response</span></span>
<span data-ttu-id="10ec1-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="10ec1-136">The following is an example of the response.</span></span> <span data-ttu-id="10ec1-137">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="10ec1-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="10ec1-138">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="10ec1-138">All of the properties will be returned from an actual call.</span></span>
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
      },"id":"03ea0c3d-90a0-42d4-b220-11c049c506fb","userId": "Self"，"roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","evaluateOnly":false,"type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-02-07T22:17:37.2215343Z","status":"ApprovalAborted","duration":"1","reason":"Activate for testing","ticketNumber":"222","ticketSystem":"222"
    },{
      "schedule":{
        "type":"assignment","startDateTime":"2018-01-23T02:43:15.258242Z","endDateTime":null,"duration" : null
      },"id":"fe4450bb-6d28-4583-8fc4-25b0ea91daf5","userId": "Self"，"roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","evaluateOnly":false,"type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-01-23T02:42:55.628338Z","status":"Completed","duration":"1","reason":"asdf","ticketNumber":null,"ticketSystem":null
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
