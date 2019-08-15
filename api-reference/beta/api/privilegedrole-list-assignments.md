---
title: 列出作业
description: 检索与角色关联的 privilegedRoleAssignment 对象的列表。 每个 privilegedRoleAssignment 表示为用户分配的角色。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2ba85e34a3ce89c072f6a2d955c10505e30eb318
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412801"
---
# <a name="list-assignments"></a><span data-ttu-id="48b00-104">列出作业</span><span class="sxs-lookup"><span data-stu-id="48b00-104">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48b00-105">检索与角色关联的[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="48b00-105">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="48b00-106">每个[privilegedRoleAssignment](../resources/privilegedroleassignment.md)代表一个用户的角色分配。</span><span class="sxs-lookup"><span data-stu-id="48b00-106">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="48b00-107">权限</span><span class="sxs-lookup"><span data-stu-id="48b00-107">Permissions</span></span>
<span data-ttu-id="48b00-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="48b00-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="48b00-110">请求者需要具有以下角色之一:_特权角色管理员_、_全局管理员_、_安全管理员_或_安全读者_。</span><span class="sxs-lookup"><span data-stu-id="48b00-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="48b00-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="48b00-111">Permission type</span></span>      | <span data-ttu-id="48b00-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="48b00-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48b00-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48b00-113">Delegated (work or school account)</span></span> | <span data-ttu-id="48b00-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="48b00-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="48b00-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48b00-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48b00-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="48b00-116">Not supported.</span></span>    |
|<span data-ttu-id="48b00-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="48b00-117">Application</span></span> | <span data-ttu-id="48b00-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="48b00-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48b00-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48b00-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="48b00-120">请注意``{id}`` , 它是目标角色 id。</span><span class="sxs-lookup"><span data-stu-id="48b00-120">Note that ``{id}`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="48b00-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="48b00-121">Optional query parameters</span></span>
<span data-ttu-id="48b00-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="48b00-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48b00-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="48b00-123">Request headers</span></span>
| <span data-ttu-id="48b00-124">名称</span><span class="sxs-lookup"><span data-stu-id="48b00-124">Name</span></span>      |<span data-ttu-id="48b00-125">说明</span><span class="sxs-lookup"><span data-stu-id="48b00-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="48b00-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="48b00-126">Authorization</span></span>  | <span data-ttu-id="48b00-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="48b00-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48b00-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="48b00-129">Request body</span></span>
<span data-ttu-id="48b00-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="48b00-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48b00-131">响应</span><span class="sxs-lookup"><span data-stu-id="48b00-131">Response</span></span>

<span data-ttu-id="48b00-132">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="48b00-132">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="48b00-133">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="48b00-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="48b00-134">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="48b00-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="48b00-135">示例</span><span class="sxs-lookup"><span data-stu-id="48b00-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48b00-136">请求</span><span class="sxs-lookup"><span data-stu-id="48b00-136">Request</span></span>
<span data-ttu-id="48b00-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="48b00-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="48b00-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="48b00-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="48b00-139">C#</span><span class="sxs-lookup"><span data-stu-id="48b00-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-assignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48b00-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48b00-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-assignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="48b00-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="48b00-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-assignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="48b00-142">响应</span><span class="sxs-lookup"><span data-stu-id="48b00-142">Response</span></span>
<span data-ttu-id="48b00-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="48b00-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
