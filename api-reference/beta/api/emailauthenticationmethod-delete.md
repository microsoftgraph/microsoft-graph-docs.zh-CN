---
title: 删除 emailAuthenticationMethod
description: 删除 emailAuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7fbb2f6af414da2c44ca6d68dc688973e9d34bce
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873498"
---
# <a name="delete-emailauthenticationmethod"></a><span data-ttu-id="2361c-103">删除 emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2361c-103">Delete emailAuthenticationMethod</span></span>
<span data-ttu-id="2361c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2361c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2361c-105">删除用户的电子邮件 [身份验证方法](../resources/emailauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2361c-105">Deletes a user's [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2361c-106">权限</span><span class="sxs-lookup"><span data-stu-id="2361c-106">Permissions</span></span>
<span data-ttu-id="2361c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2361c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2361c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2361c-109">Permission type</span></span>|<span data-ttu-id="2361c-110">对自身执行 (权限从最低特权到最多特权) </span><span class="sxs-lookup"><span data-stu-id="2361c-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="2361c-111">对他人的操作权限 (权限从最低特权级别) </span><span class="sxs-lookup"><span data-stu-id="2361c-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="2361c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2361c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2361c-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2361c-113">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="2361c-114">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2361c-114">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="2361c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2361c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2361c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2361c-116">Not supported.</span></span> | <span data-ttu-id="2361c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2361c-117">Not supported.</span></span> |
| <span data-ttu-id="2361c-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="2361c-118">Application</span></span>                            | <span data-ttu-id="2361c-119">不适用。</span><span class="sxs-lookup"><span data-stu-id="2361c-119">Not applicable.</span></span> | <span data-ttu-id="2361c-120">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2361c-120">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="2361c-121">对于管理员正在操作其他用户的委派方案，管理员需要以下角色 [之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="2361c-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="2361c-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="2361c-122">Global admin</span></span>
* <span data-ttu-id="2361c-123">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="2361c-123">Privileged authentication admin</span></span>
* <span data-ttu-id="2361c-124">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="2361c-124">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="2361c-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2361c-125">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2361c-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="2361c-126">Request headers</span></span>
|<span data-ttu-id="2361c-127">名称</span><span class="sxs-lookup"><span data-stu-id="2361c-127">Name</span></span>|<span data-ttu-id="2361c-128">说明</span><span class="sxs-lookup"><span data-stu-id="2361c-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2361c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="2361c-129">Authorization</span></span>|<span data-ttu-id="2361c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2361c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2361c-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="2361c-132">Request body</span></span>
<span data-ttu-id="2361c-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2361c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2361c-134">响应</span><span class="sxs-lookup"><span data-stu-id="2361c-134">Response</span></span>

<span data-ttu-id="2361c-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2361c-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2361c-137">示例</span><span class="sxs-lookup"><span data-stu-id="2361c-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2361c-138">请求</span><span class="sxs-lookup"><span data-stu-id="2361c-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2361c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="2361c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```
# <a name="c"></a>[<span data-ttu-id="2361c-140">C#</span><span class="sxs-lookup"><span data-stu-id="2361c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2361c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2361c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2361c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2361c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2361c-143">Java</span><span class="sxs-lookup"><span data-stu-id="2361c-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2361c-144">响应</span><span class="sxs-lookup"><span data-stu-id="2361c-144">Response</span></span>
<span data-ttu-id="2361c-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2361c-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

