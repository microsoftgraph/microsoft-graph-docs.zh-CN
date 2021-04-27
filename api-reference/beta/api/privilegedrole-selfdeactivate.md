---
title: privilegedRole： selfDeactivate
description: 停用分配给请求者的角色。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 5c2b2bbd11308f4a593dce3709581b8facb8516d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055244"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="64e14-103">privilegedRole： selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="64e14-103">privilegedRole: selfDeactivate</span></span>

<span data-ttu-id="64e14-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64e14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64e14-105">停用分配给请求者的角色。</span><span class="sxs-lookup"><span data-stu-id="64e14-105">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="64e14-106">权限</span><span class="sxs-lookup"><span data-stu-id="64e14-106">Permissions</span></span>
<span data-ttu-id="64e14-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64e14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="64e14-109">请求者只能 ```selfDeactivate``` 调用分配给他的角色。</span><span class="sxs-lookup"><span data-stu-id="64e14-109">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="64e14-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="64e14-110">Permission type</span></span>      | <span data-ttu-id="64e14-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="64e14-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64e14-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64e14-112">Delegated (work or school account)</span></span> | <span data-ttu-id="64e14-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64e14-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="64e14-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64e14-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64e14-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="64e14-115">Not supported.</span></span>    |
|<span data-ttu-id="64e14-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="64e14-116">Application</span></span> | <span data-ttu-id="64e14-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="64e14-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64e14-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64e14-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="64e14-119">请注意， ``{id}`` 这是目标角色 ID。</span><span class="sxs-lookup"><span data-stu-id="64e14-119">Note that ``{id}`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="64e14-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="64e14-120">Request headers</span></span>
| <span data-ttu-id="64e14-121">名称</span><span class="sxs-lookup"><span data-stu-id="64e14-121">Name</span></span>       | <span data-ttu-id="64e14-122">说明</span><span class="sxs-lookup"><span data-stu-id="64e14-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="64e14-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="64e14-123">Authorization</span></span>  | <span data-ttu-id="64e14-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="64e14-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64e14-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="64e14-126">Request body</span></span>
<span data-ttu-id="64e14-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="64e14-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64e14-128">响应</span><span class="sxs-lookup"><span data-stu-id="64e14-128">Response</span></span>

<span data-ttu-id="64e14-129">如果成功，此方法在 `200 OK` 响应正文中返回 [响应代码和 privilegedRoleAssignment](../resources/privilegedroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="64e14-129">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="64e14-130">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="64e14-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="64e14-131">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="64e14-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="64e14-132">示例</span><span class="sxs-lookup"><span data-stu-id="64e14-132">Example</span></span>
<span data-ttu-id="64e14-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="64e14-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="64e14-134">请求</span><span class="sxs-lookup"><span data-stu-id="64e14-134">Request</span></span>
<span data-ttu-id="64e14-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="64e14-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64e14-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="64e14-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```
# <a name="c"></a>[<span data-ttu-id="64e14-137">C#</span><span class="sxs-lookup"><span data-stu-id="64e14-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfdeactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64e14-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64e14-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfdeactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64e14-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64e14-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfdeactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64e14-140">Java</span><span class="sxs-lookup"><span data-stu-id="64e14-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedrole-selfdeactivate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="64e14-141">响应</span><span class="sxs-lookup"><span data-stu-id="64e14-141">Response</span></span>
<span data-ttu-id="64e14-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="64e14-142">Here is an example of the response.</span></span> <span data-ttu-id="64e14-143">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="64e14-143">Note: The response object shown here might be shortened for readability.</span></span>
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


