---
title: 列出 privilegedRoleAssignmentRequests
description: '检索 privilegedRoleAssignmentRequest 的集合。 '
localization_priority: Normal
ms.openlocfilehash: 4451eedf072be4f2b35a7524e4f7e5393c4326e8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444902"
---
# <a name="list-privilegedroleassignmentrequests"></a><span data-ttu-id="44198-103">列出 privilegedRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="44198-103">List privilegedRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44198-104">检索[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="44198-104">Retrieve a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span> 

<span data-ttu-id="44198-105">**注意:** 此请求者必须至少具有对资源的一个角色分配。</span><span class="sxs-lookup"><span data-stu-id="44198-105">**Note:** This requester must have at least one role assignment on the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="44198-106">权限</span><span class="sxs-lookup"><span data-stu-id="44198-106">Permissions</span></span>
<span data-ttu-id="44198-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44198-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44198-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="44198-109">Permission type</span></span>                        | <span data-ttu-id="44198-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44198-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="44198-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44198-111">Delegated (work or school account)</span></span> | <span data-ttu-id="44198-112">PrivilegedAccess、AzureAD、Directory.accessasuser.all、All 和</span><span class="sxs-lookup"><span data-stu-id="44198-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="44198-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44198-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44198-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="44198-114">Not supported.</span></span> |
|<span data-ttu-id="44198-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="44198-115">Application</span></span>                            | <span data-ttu-id="44198-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="44198-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44198-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44198-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="44198-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="44198-118">Optional query parameters</span></span>
<span data-ttu-id="44198-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="44198-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44198-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="44198-120">Request headers</span></span>
| <span data-ttu-id="44198-121">名称</span><span class="sxs-lookup"><span data-stu-id="44198-121">Name</span></span>      |<span data-ttu-id="44198-122">说明</span><span class="sxs-lookup"><span data-stu-id="44198-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="44198-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44198-123">Authorization</span></span>  | <span data-ttu-id="44198-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="44198-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44198-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="44198-126">Request body</span></span>
<span data-ttu-id="44198-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="44198-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44198-128">响应</span><span class="sxs-lookup"><span data-stu-id="44198-128">Response</span></span>
<span data-ttu-id="44198-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="44198-129">If successful, this method returns a `200 OK` response code and a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44198-130">示例</span><span class="sxs-lookup"><span data-stu-id="44198-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44198-131">请求</span><span class="sxs-lookup"><span data-stu-id="44198-131">Request</span></span>
<span data-ttu-id="44198-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="44198-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="44198-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="44198-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="44198-134">C#</span><span class="sxs-lookup"><span data-stu-id="44198-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="44198-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="44198-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="44198-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="44198-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="44198-137">响应</span><span class="sxs-lookup"><span data-stu-id="44198-137">Response</span></span>
<span data-ttu-id="44198-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="44198-138">The following is an example of the response.</span></span> <span data-ttu-id="44198-139">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="44198-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="44198-140">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="44198-140">All of the properties will be returned from an actual call.</span></span>
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
      },"id":"03ea0c3d-90a0-42d4-b220-11c049c506fb","userId": "Self","roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","evaluateOnly":false,"type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-02-07T22:17:37.2215343Z","status":"ApprovalAborted","duration":"1","reason":"Activate for testing","ticketNumber":"222","ticketSystem":"222"
    },{
      "schedule":{
        "type":"assignment","startDateTime":"2018-01-23T02:43:15.258242Z","endDateTime":null,"duration" : null
      },"id":"fe4450bb-6d28-4583-8fc4-25b0ea91daf5","userId": "Self","roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","evaluateOnly":false,"type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-01-23T02:42:55.628338Z","status":"Completed","duration":"1","reason":"asdf","ticketNumber":null,"ticketSystem":null
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
