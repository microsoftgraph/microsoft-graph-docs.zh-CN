---
title: 删除 emailAuthenticationMethod
description: 删除 emailAuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 25a05ff6b4ad6639c7be87a88135fc2cebd8c2cb
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796372"
---
# <a name="delete-emailauthenticationmethod"></a><span data-ttu-id="b1ae3-103">删除 emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b1ae3-103">Delete emailAuthenticationMethod</span></span>
<span data-ttu-id="b1ae3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1ae3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1ae3-105">删除用户的电子邮件 [身份验证方法](../resources/emailauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1ae3-105">Deletes a user's [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1ae3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b1ae3-106">Permissions</span></span>
<span data-ttu-id="b1ae3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1ae3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1ae3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1ae3-109">Permission type</span></span>|<span data-ttu-id="b1ae3-110">对自身执行 (权限从最多到最低特权) </span><span class="sxs-lookup"><span data-stu-id="b1ae3-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="b1ae3-111">对他人操作的权限 (权限从最低特权到最多特权) </span><span class="sxs-lookup"><span data-stu-id="b1ae3-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="b1ae3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1ae3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b1ae3-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1ae3-113">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="b1ae3-114">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1ae3-114">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="b1ae3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1ae3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1ae3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1ae3-116">Not supported.</span></span> | <span data-ttu-id="b1ae3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1ae3-117">Not supported.</span></span> |
| <span data-ttu-id="b1ae3-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1ae3-118">Application</span></span>                            | <span data-ttu-id="b1ae3-119">不适用</span><span class="sxs-lookup"><span data-stu-id="b1ae3-119">Not applicable.</span></span> | <span data-ttu-id="b1ae3-120">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1ae3-120">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="b1ae3-121">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="b1ae3-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="b1ae3-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="b1ae3-122">Global admin</span></span>
* <span data-ttu-id="b1ae3-123">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="b1ae3-123">Privileged authentication admin</span></span>
* <span data-ttu-id="b1ae3-124">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="b1ae3-124">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="b1ae3-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1ae3-125">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b1ae3-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1ae3-126">Request headers</span></span>
|<span data-ttu-id="b1ae3-127">名称</span><span class="sxs-lookup"><span data-stu-id="b1ae3-127">Name</span></span>|<span data-ttu-id="b1ae3-128">说明</span><span class="sxs-lookup"><span data-stu-id="b1ae3-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b1ae3-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1ae3-129">Authorization</span></span>|<span data-ttu-id="b1ae3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b1ae3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1ae3-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1ae3-132">Request body</span></span>
<span data-ttu-id="b1ae3-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b1ae3-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1ae3-134">响应</span><span class="sxs-lookup"><span data-stu-id="b1ae3-134">Response</span></span>

<span data-ttu-id="b1ae3-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b1ae3-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b1ae3-137">示例</span><span class="sxs-lookup"><span data-stu-id="b1ae3-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b1ae3-138">请求</span><span class="sxs-lookup"><span data-stu-id="b1ae3-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b1ae3-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1ae3-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```
# <a name="c"></a>[<span data-ttu-id="b1ae3-140">C#</span><span class="sxs-lookup"><span data-stu-id="b1ae3-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b1ae3-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1ae3-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1ae3-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1ae3-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b1ae3-143">Java</span><span class="sxs-lookup"><span data-stu-id="b1ae3-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b1ae3-144">响应</span><span class="sxs-lookup"><span data-stu-id="b1ae3-144">Response</span></span>
<span data-ttu-id="b1ae3-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b1ae3-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

