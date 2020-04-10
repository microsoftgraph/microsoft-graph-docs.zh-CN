---
title: 'privilegedRole: selfDeactivate'
description: 停用分配给请求者的角色。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: ea2d8f9a34b2cf4defad6865518044d7908266d4
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218743"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="9c90b-103">privilegedRole: selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="9c90b-103">privilegedRole: selfDeactivate</span></span>

<span data-ttu-id="9c90b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c90b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c90b-105">停用分配给请求者的角色。</span><span class="sxs-lookup"><span data-stu-id="9c90b-105">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="9c90b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9c90b-106">Permissions</span></span>
<span data-ttu-id="9c90b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c90b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9c90b-109">请求者只能调用```selfDeactivate```分配给他的角色。</span><span class="sxs-lookup"><span data-stu-id="9c90b-109">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="9c90b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c90b-110">Permission type</span></span>      | <span data-ttu-id="9c90b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c90b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c90b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c90b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9c90b-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9c90b-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9c90b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c90b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c90b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c90b-115">Not supported.</span></span>    |
|<span data-ttu-id="9c90b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c90b-116">Application</span></span> | <span data-ttu-id="9c90b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c90b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c90b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c90b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="9c90b-119">请注意``{id}`` ，它是目标角色 id。</span><span class="sxs-lookup"><span data-stu-id="9c90b-119">Note that ``{id}`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9c90b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c90b-120">Request headers</span></span>
| <span data-ttu-id="9c90b-121">名称</span><span class="sxs-lookup"><span data-stu-id="9c90b-121">Name</span></span>       | <span data-ttu-id="9c90b-122">说明</span><span class="sxs-lookup"><span data-stu-id="9c90b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9c90b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c90b-123">Authorization</span></span>  | <span data-ttu-id="9c90b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9c90b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c90b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c90b-126">Request body</span></span>
<span data-ttu-id="9c90b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9c90b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c90b-128">响应</span><span class="sxs-lookup"><span data-stu-id="9c90b-128">Response</span></span>

<span data-ttu-id="9c90b-129">如果成功，此方法在`200 OK`响应正文中返回响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9c90b-129">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="9c90b-130">请注意，需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="9c90b-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="9c90b-131">否则，将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="9c90b-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="9c90b-132">示例</span><span class="sxs-lookup"><span data-stu-id="9c90b-132">Example</span></span>
<span data-ttu-id="9c90b-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="9c90b-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9c90b-134">请求</span><span class="sxs-lookup"><span data-stu-id="9c90b-134">Request</span></span>
<span data-ttu-id="9c90b-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c90b-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9c90b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c90b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```
# <a name="c"></a>[<span data-ttu-id="9c90b-137">C#</span><span class="sxs-lookup"><span data-stu-id="9c90b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfdeactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c90b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c90b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfdeactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c90b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c90b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfdeactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9c90b-140">响应</span><span class="sxs-lookup"><span data-stu-id="9c90b-140">Response</span></span>
<span data-ttu-id="9c90b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9c90b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
