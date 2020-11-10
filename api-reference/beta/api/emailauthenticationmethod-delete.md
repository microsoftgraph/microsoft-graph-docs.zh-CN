---
title: 删除 emailAuthenticationMethod
description: 删除一个 emailAuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b95f602c9b4180696b43753ba564f3604ce05846
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955120"
---
# <a name="delete-emailauthenticationmethod"></a><span data-ttu-id="94e09-103">删除 emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="94e09-103">Delete emailAuthenticationMethod</span></span>
<span data-ttu-id="94e09-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94e09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94e09-105">删除用户的 [电子邮件身份验证方法](../resources/emailauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94e09-105">Deletes a user's [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="94e09-106">权限</span><span class="sxs-lookup"><span data-stu-id="94e09-106">Permissions</span></span>
<span data-ttu-id="94e09-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94e09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94e09-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="94e09-109">Permission type</span></span>|<span data-ttu-id="94e09-110">从最高特权到最少特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="94e09-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="94e09-111">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="94e09-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="94e09-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94e09-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94e09-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="94e09-113">Not supported.</span></span>|<span data-ttu-id="94e09-114">UserAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="94e09-114">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="94e09-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94e09-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94e09-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="94e09-116">Not supported.</span></span>|<span data-ttu-id="94e09-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="94e09-117">Not supported.</span></span>
|<span data-ttu-id="94e09-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="94e09-118">Application</span></span>|<span data-ttu-id="94e09-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="94e09-119">Not supported.</span></span>|<span data-ttu-id="94e09-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="94e09-120">Not supported.</span></span>

<span data-ttu-id="94e09-121">对于在其他用户上执行管理的委派方案，管理员需要 [以下角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="94e09-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="94e09-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="94e09-122">Global admin</span></span>
* <span data-ttu-id="94e09-123">全局读取者</span><span class="sxs-lookup"><span data-stu-id="94e09-123">Global reader</span></span>
* <span data-ttu-id="94e09-124">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="94e09-124">Privileged authentication admin</span></span>
* <span data-ttu-id="94e09-125">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="94e09-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="94e09-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94e09-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="94e09-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="94e09-127">Request headers</span></span>
|<span data-ttu-id="94e09-128">名称</span><span class="sxs-lookup"><span data-stu-id="94e09-128">Name</span></span>|<span data-ttu-id="94e09-129">说明</span><span class="sxs-lookup"><span data-stu-id="94e09-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="94e09-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="94e09-130">Authorization</span></span>|<span data-ttu-id="94e09-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94e09-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94e09-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="94e09-133">Request body</span></span>
<span data-ttu-id="94e09-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="94e09-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94e09-135">响应</span><span class="sxs-lookup"><span data-stu-id="94e09-135">Response</span></span>

<span data-ttu-id="94e09-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="94e09-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94e09-138">示例</span><span class="sxs-lookup"><span data-stu-id="94e09-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94e09-139">请求</span><span class="sxs-lookup"><span data-stu-id="94e09-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="94e09-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="94e09-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```
# <a name="c"></a>[<span data-ttu-id="94e09-141">C#</span><span class="sxs-lookup"><span data-stu-id="94e09-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94e09-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94e09-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94e09-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94e09-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94e09-144">Java</span><span class="sxs-lookup"><span data-stu-id="94e09-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="94e09-145">响应</span><span class="sxs-lookup"><span data-stu-id="94e09-145">Response</span></span>
<span data-ttu-id="94e09-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="94e09-146">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

