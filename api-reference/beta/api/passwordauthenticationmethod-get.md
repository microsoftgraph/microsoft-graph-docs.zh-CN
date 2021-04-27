---
title: 获取 passwordAuthenticationMethod
description: 检索 passwordauthentication 方法对象的属性和关系。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 32aad6e260b0eeb4df87cd9daa51f59d0fa82416
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049175"
---
# <a name="get-passwordauthenticationmethod"></a><span data-ttu-id="d33e7-103">获取 passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d33e7-103">Get passwordAuthenticationMethod</span></span>

<span data-ttu-id="d33e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d33e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d33e7-105">检索密码身份验证方法 [对象的属性和](../resources/passwordauthenticationmethod.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="d33e7-105">Retrieve the properties and relationships of a [password authentication method](../resources/passwordauthenticationmethod.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d33e7-106">权限</span><span class="sxs-lookup"><span data-stu-id="d33e7-106">Permissions</span></span>

<span data-ttu-id="d33e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d33e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="d33e7-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="d33e7-109">Permissions acting on self</span></span>

|<span data-ttu-id="d33e7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d33e7-110">Permission type</span></span>      | <span data-ttu-id="d33e7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d33e7-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="d33e7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d33e7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d33e7-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d33e7-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="d33e7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d33e7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d33e7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d33e7-115">Not supported.</span></span> |
| <span data-ttu-id="d33e7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d33e7-116">Application</span></span>                            | <span data-ttu-id="d33e7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d33e7-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="d33e7-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="d33e7-118">Permissions acting on other users</span></span>

|<span data-ttu-id="d33e7-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="d33e7-119">Permission type</span></span>      | <span data-ttu-id="d33e7-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d33e7-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="d33e7-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d33e7-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="d33e7-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d33e7-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="d33e7-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d33e7-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d33e7-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="d33e7-124">Not supported.</span></span> |
| <span data-ttu-id="d33e7-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="d33e7-125">Application</span></span>                            | <span data-ttu-id="d33e7-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d33e7-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="d33e7-127">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="d33e7-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="d33e7-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="d33e7-128">Global admin</span></span>
* <span data-ttu-id="d33e7-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="d33e7-129">Global reader</span></span>
* <span data-ttu-id="d33e7-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="d33e7-130">Privileged authentication admin</span></span>
* <span data-ttu-id="d33e7-131">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="d33e7-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="d33e7-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d33e7-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d33e7-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d33e7-133">Optional query parameters</span></span>

<span data-ttu-id="d33e7-134">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="d33e7-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d33e7-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="d33e7-135">Request headers</span></span>

| <span data-ttu-id="d33e7-136">名称</span><span class="sxs-lookup"><span data-stu-id="d33e7-136">Name</span></span>      |<span data-ttu-id="d33e7-137">说明</span><span class="sxs-lookup"><span data-stu-id="d33e7-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d33e7-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="d33e7-138">Authorization</span></span> | <span data-ttu-id="d33e7-139">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="d33e7-139">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d33e7-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="d33e7-140">Request body</span></span>

<span data-ttu-id="d33e7-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d33e7-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d33e7-142">响应</span><span class="sxs-lookup"><span data-stu-id="d33e7-142">Response</span></span>

<span data-ttu-id="d33e7-143">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d33e7-143">If successful, this method returns a `200 OK` response code and the requested [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d33e7-144">示例</span><span class="sxs-lookup"><span data-stu-id="d33e7-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d33e7-145">请求</span><span class="sxs-lookup"><span data-stu-id="d33e7-145">Request</span></span>

<span data-ttu-id="d33e7-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d33e7-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d33e7-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="d33e7-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods/{id}
```
# <a name="c"></a>[<span data-ttu-id="d33e7-148">C#</span><span class="sxs-lookup"><span data-stu-id="d33e7-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d33e7-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d33e7-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d33e7-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d33e7-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d33e7-151">Java</span><span class="sxs-lookup"><span data-stu-id="d33e7-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d33e7-152">响应</span><span class="sxs-lookup"><span data-stu-id="d33e7-152">Response</span></span>

<span data-ttu-id="d33e7-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d33e7-153">The following is an example of the response.</span></span>

> <span data-ttu-id="d33e7-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d33e7-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "28c10230-6103-485e-b985-444c60001490",
  "password": null,
  "creationDateTime": null
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get passwordAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
