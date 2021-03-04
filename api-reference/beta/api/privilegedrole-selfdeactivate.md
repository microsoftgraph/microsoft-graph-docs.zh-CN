---
title: privilegedRole：selfDeactivate
description: 停用分配给请求者的角色。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: a50f74e928d95ba5bce5e39dc61febb30f9d67b7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441282"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="7a8b8-103">privilegedRole： selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="7a8b8-103">privilegedRole: selfDeactivate</span></span>

<span data-ttu-id="7a8b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a8b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a8b8-105">停用分配给请求者的角色。</span><span class="sxs-lookup"><span data-stu-id="7a8b8-105">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="7a8b8-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7a8b8-106">Permissions</span></span>
<span data-ttu-id="7a8b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a8b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7a8b8-109">请求者只能调用分配给他 ```selfDeactivate``` 的角色。</span><span class="sxs-lookup"><span data-stu-id="7a8b8-109">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="7a8b8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a8b8-110">Permission type</span></span>      | <span data-ttu-id="7a8b8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7a8b8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a8b8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a8b8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7a8b8-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7a8b8-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7a8b8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a8b8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a8b8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a8b8-115">Not supported.</span></span>    |
|<span data-ttu-id="7a8b8-116">Application</span><span class="sxs-lookup"><span data-stu-id="7a8b8-116">Application</span></span> | <span data-ttu-id="7a8b8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a8b8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a8b8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a8b8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="7a8b8-119">请注意 ``{id}`` ，这是目标角色 ID。</span><span class="sxs-lookup"><span data-stu-id="7a8b8-119">Note that ``{id}`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7a8b8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a8b8-120">Request headers</span></span>
| <span data-ttu-id="7a8b8-121">名称</span><span class="sxs-lookup"><span data-stu-id="7a8b8-121">Name</span></span>       | <span data-ttu-id="7a8b8-122">说明</span><span class="sxs-lookup"><span data-stu-id="7a8b8-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7a8b8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a8b8-123">Authorization</span></span>  | <span data-ttu-id="7a8b8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7a8b8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a8b8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a8b8-126">Request body</span></span>
<span data-ttu-id="7a8b8-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7a8b8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a8b8-128">响应</span><span class="sxs-lookup"><span data-stu-id="7a8b8-128">Response</span></span>

<span data-ttu-id="7a8b8-129">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [privilegedRoleAssignment](../resources/privilegedroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7a8b8-129">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="7a8b8-130">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="7a8b8-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="7a8b8-131">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="7a8b8-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="7a8b8-132">示例</span><span class="sxs-lookup"><span data-stu-id="7a8b8-132">Example</span></span>
<span data-ttu-id="7a8b8-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7a8b8-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7a8b8-134">请求</span><span class="sxs-lookup"><span data-stu-id="7a8b8-134">Request</span></span>
<span data-ttu-id="7a8b8-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7a8b8-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7a8b8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a8b8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```
# <a name="c"></a>[<span data-ttu-id="7a8b8-137">C#</span><span class="sxs-lookup"><span data-stu-id="7a8b8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfdeactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a8b8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a8b8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfdeactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a8b8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a8b8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfdeactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a8b8-140">Java</span><span class="sxs-lookup"><span data-stu-id="7a8b8-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedrole-selfdeactivate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7a8b8-141">响应</span><span class="sxs-lookup"><span data-stu-id="7a8b8-141">Response</span></span>
<span data-ttu-id="7a8b8-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7a8b8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole: selfDeactivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


