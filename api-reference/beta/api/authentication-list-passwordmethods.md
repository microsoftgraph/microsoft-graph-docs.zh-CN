---
title: 列出 passwordMethods
description: 检索 passwordauthenticationmethod 对象的列表。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1184d095b5ea609dc7293948b69ac00673a07861
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438608"
---
# <a name="list-passwordmethods"></a><span data-ttu-id="2c36a-103">列出 passwordMethods</span><span class="sxs-lookup"><span data-stu-id="2c36a-103">List passwordMethods</span></span>

<span data-ttu-id="2c36a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c36a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c36a-105">检索密码 [身份验证方法对象](../resources/passwordauthenticationmethod.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="2c36a-105">Retrieve a list of [password authentication method](../resources/passwordauthenticationmethod.md) objects.</span></span> <span data-ttu-id="2c36a-106">这将返回一个对象，因为用户只能有一个密码。</span><span class="sxs-lookup"><span data-stu-id="2c36a-106">This will return exactly one object, as a user can have exactly one password.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c36a-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="2c36a-107">Permissions</span></span>

<span data-ttu-id="2c36a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c36a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="2c36a-110">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="2c36a-110">Permissions acting on self</span></span>

|<span data-ttu-id="2c36a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c36a-111">Permission type</span></span>      | <span data-ttu-id="2c36a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c36a-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="2c36a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c36a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c36a-114">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c36a-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="2c36a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c36a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c36a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c36a-116">Not supported.</span></span> |
| <span data-ttu-id="2c36a-117">Application</span><span class="sxs-lookup"><span data-stu-id="2c36a-117">Application</span></span>                            | <span data-ttu-id="2c36a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c36a-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="2c36a-119">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="2c36a-119">Permissions acting on other users</span></span>

|<span data-ttu-id="2c36a-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c36a-120">Permission type</span></span>      | <span data-ttu-id="2c36a-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c36a-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="2c36a-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c36a-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c36a-123">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c36a-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="2c36a-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c36a-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c36a-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c36a-125">Not supported.</span></span> |
| <span data-ttu-id="2c36a-126">Application</span><span class="sxs-lookup"><span data-stu-id="2c36a-126">Application</span></span>                            | <span data-ttu-id="2c36a-127">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c36a-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="2c36a-128">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="2c36a-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="2c36a-129">全局管理员</span><span class="sxs-lookup"><span data-stu-id="2c36a-129">Global admin</span></span>
* <span data-ttu-id="2c36a-130">全局读取者</span><span class="sxs-lookup"><span data-stu-id="2c36a-130">Global reader</span></span>
* <span data-ttu-id="2c36a-131">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="2c36a-131">Privileged authentication admin</span></span>
* <span data-ttu-id="2c36a-132">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="2c36a-132">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="2c36a-133">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c36a-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods
GET /users/{id | userPrincipalName}/authentication/passwordMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c36a-134">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2c36a-134">Optional query parameters</span></span>

<span data-ttu-id="2c36a-135">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="2c36a-135">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c36a-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c36a-136">Request headers</span></span>

| <span data-ttu-id="2c36a-137">名称</span><span class="sxs-lookup"><span data-stu-id="2c36a-137">Name</span></span>      |<span data-ttu-id="2c36a-138">说明</span><span class="sxs-lookup"><span data-stu-id="2c36a-138">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2c36a-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c36a-139">Authorization</span></span> | <span data-ttu-id="2c36a-140">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="2c36a-140">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c36a-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c36a-141">Request body</span></span>

<span data-ttu-id="2c36a-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2c36a-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c36a-143">响应</span><span class="sxs-lookup"><span data-stu-id="2c36a-143">Response</span></span>

<span data-ttu-id="2c36a-144">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2c36a-144">If successful, this method returns a `200 OK` response code and a collection of [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2c36a-145">示例</span><span class="sxs-lookup"><span data-stu-id="2c36a-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2c36a-146">请求</span><span class="sxs-lookup"><span data-stu-id="2c36a-146">Request</span></span>

<span data-ttu-id="2c36a-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2c36a-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c36a-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c36a-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordmethods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods
```
# <a name="c"></a>[<span data-ttu-id="2c36a-149">C#</span><span class="sxs-lookup"><span data-stu-id="2c36a-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordmethods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c36a-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c36a-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordmethods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c36a-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c36a-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordmethods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c36a-152">Java</span><span class="sxs-lookup"><span data-stu-id="2c36a-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordmethods-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2c36a-153">响应</span><span class="sxs-lookup"><span data-stu-id="2c36a-153">Response</span></span>

<span data-ttu-id="2c36a-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2c36a-154">The following is an example of the response.</span></span>

> <span data-ttu-id="2c36a-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2c36a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "28c10230-6103-485e-b985-444c60001490",
      "password": null,
      "creationDateTime": null
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List passwordMethods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
