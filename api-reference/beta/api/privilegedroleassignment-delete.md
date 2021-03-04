---
title: Delete privilegedRoleAssignment
description: 删除 privilegedRoleAssignment。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: a0481108a141d41b62689de12cfaef882756fef9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441275"
---
# <a name="delete-privilegedroleassignment"></a><span data-ttu-id="fbbb6-103">Delete privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="fbbb6-103">Delete privilegedRoleAssignment</span></span>

<span data-ttu-id="fbbb6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbbb6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbbb6-105">删除 [privilegedRoleAssignment](../resources/privilegedroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="fbbb6-105">Delete [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="fbbb6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="fbbb6-106">Permissions</span></span>
<span data-ttu-id="fbbb6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fbbb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="fbbb6-109">请求者需要具有 _Privileged Role Administrator_ 角色。</span><span class="sxs-lookup"><span data-stu-id="fbbb6-109">The requestor needs to have _Privileged Role Administrator_ role.</span></span>
 

|<span data-ttu-id="fbbb6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fbbb6-110">Permission type</span></span>      | <span data-ttu-id="fbbb6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fbbb6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbbb6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fbbb6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fbbb6-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fbbb6-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fbbb6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fbbb6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbbb6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbbb6-115">Not supported.</span></span>    |
|<span data-ttu-id="fbbb6-116">Application</span><span class="sxs-lookup"><span data-stu-id="fbbb6-116">Application</span></span> | <span data-ttu-id="fbbb6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbbb6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbbb6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fbbb6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /privilegedRoleAssignments/{id}
```

<span data-ttu-id="fbbb6-119">请注意，采用"userId_roleId"格式，其中 userId 是 Azure AD 用户 ID 的 GUID 字符串，roleId 是 Azure 管理员角色 ID 的 ``{id}`` GUID 字符串。</span><span class="sxs-lookup"><span data-stu-id="fbbb6-119">Note that ``{id}`` is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fbbb6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fbbb6-120">Request headers</span></span>
| <span data-ttu-id="fbbb6-121">名称</span><span class="sxs-lookup"><span data-stu-id="fbbb6-121">Name</span></span>       | <span data-ttu-id="fbbb6-122">说明</span><span class="sxs-lookup"><span data-stu-id="fbbb6-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fbbb6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbbb6-123">Authorization</span></span>  | <span data-ttu-id="fbbb6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fbbb6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fbbb6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fbbb6-126">Request body</span></span>
<span data-ttu-id="fbbb6-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fbbb6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbbb6-128">响应</span><span class="sxs-lookup"><span data-stu-id="fbbb6-128">Response</span></span>

<span data-ttu-id="fbbb6-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fbbb6-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="fbbb6-131">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="fbbb6-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="fbbb6-132">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="fbbb6-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="fbbb6-133">示例</span><span class="sxs-lookup"><span data-stu-id="fbbb6-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fbbb6-134">请求</span><span class="sxs-lookup"><span data-stu-id="fbbb6-134">Request</span></span>
<span data-ttu-id="fbbb6-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fbbb6-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fbbb6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="fbbb6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_privilegedroleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="fbbb6-137">C#</span><span class="sxs-lookup"><span data-stu-id="fbbb6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-privilegedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fbbb6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fbbb6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-privilegedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fbbb6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fbbb6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-privilegedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fbbb6-140">Java</span><span class="sxs-lookup"><span data-stu-id="fbbb6-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-privilegedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fbbb6-141">响应</span><span class="sxs-lookup"><span data-stu-id="fbbb6-141">Response</span></span>
<span data-ttu-id="fbbb6-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fbbb6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


