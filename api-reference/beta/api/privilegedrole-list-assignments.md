---
title: 列出作业
description: 检索与角色关联的 privilegedRoleAssignment 对象列表。 每个 privilegedRoleAssignment 表示为用户分配的角色。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 298742424152f7e483d709b33a6668e61cd866c3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441320"
---
# <a name="list-assignments"></a><span data-ttu-id="2c5f5-104">列出作业</span><span class="sxs-lookup"><span data-stu-id="2c5f5-104">List assignments</span></span>

<span data-ttu-id="2c5f5-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c5f5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c5f5-106">检索与角色关联的 [privilegedRoleAssignment](../resources/privilegedroleassignment.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="2c5f5-106">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="2c5f5-107">每个 [privilegedRoleAssignment](../resources/privilegedroleassignment.md) 都角色分配用户的权限。</span><span class="sxs-lookup"><span data-stu-id="2c5f5-107">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="2c5f5-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="2c5f5-108">Permissions</span></span>
<span data-ttu-id="2c5f5-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c5f5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2c5f5-111">请求者需要具有以下角色之一 _：Privileged Role Administrator、Global_ _Administrator、Security_ _Administrator_ 或 _Security Reader。_</span><span class="sxs-lookup"><span data-stu-id="2c5f5-111">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="2c5f5-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c5f5-112">Permission type</span></span>      | <span data-ttu-id="2c5f5-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c5f5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c5f5-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c5f5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2c5f5-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2c5f5-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2c5f5-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c5f5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c5f5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c5f5-117">Not supported.</span></span>    |
|<span data-ttu-id="2c5f5-118">Application</span><span class="sxs-lookup"><span data-stu-id="2c5f5-118">Application</span></span> | <span data-ttu-id="2c5f5-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c5f5-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c5f5-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c5f5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="2c5f5-121">请注意 ``{id}`` ，这是目标角色 ID。</span><span class="sxs-lookup"><span data-stu-id="2c5f5-121">Note that ``{id}`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="2c5f5-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2c5f5-122">Optional query parameters</span></span>
<span data-ttu-id="2c5f5-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2c5f5-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c5f5-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c5f5-124">Request headers</span></span>
| <span data-ttu-id="2c5f5-125">名称</span><span class="sxs-lookup"><span data-stu-id="2c5f5-125">Name</span></span>      |<span data-ttu-id="2c5f5-126">说明</span><span class="sxs-lookup"><span data-stu-id="2c5f5-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2c5f5-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c5f5-127">Authorization</span></span>  | <span data-ttu-id="2c5f5-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2c5f5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c5f5-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c5f5-130">Request body</span></span>
<span data-ttu-id="2c5f5-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2c5f5-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c5f5-132">响应</span><span class="sxs-lookup"><span data-stu-id="2c5f5-132">Response</span></span>

<span data-ttu-id="2c5f5-133">如果成功，此方法在响应正文中返回 `200 OK` [响应代码和 privilegedRoleAssignment](../resources/privilegedroleassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2c5f5-133">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="2c5f5-134">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="2c5f5-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="2c5f5-135">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="2c5f5-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="2c5f5-136">示例</span><span class="sxs-lookup"><span data-stu-id="2c5f5-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c5f5-137">请求</span><span class="sxs-lookup"><span data-stu-id="2c5f5-137">Request</span></span>
<span data-ttu-id="2c5f5-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c5f5-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c5f5-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c5f5-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
# <a name="c"></a>[<span data-ttu-id="2c5f5-140">C#</span><span class="sxs-lookup"><span data-stu-id="2c5f5-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-assignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c5f5-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c5f5-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-assignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c5f5-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c5f5-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-assignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c5f5-143">Java</span><span class="sxs-lookup"><span data-stu-id="2c5f5-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-assignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2c5f5-144">响应</span><span class="sxs-lookup"><span data-stu-id="2c5f5-144">Response</span></span>
<span data-ttu-id="2c5f5-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2c5f5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
