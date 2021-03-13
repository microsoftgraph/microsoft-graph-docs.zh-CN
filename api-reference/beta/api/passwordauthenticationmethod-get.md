---
title: 获取 passwordAuthenticationMethod
description: 检索 passwordauthentication 方法对象的属性和关系。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a34939a59ca265fb7c50b82cf662095052763950
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761435"
---
# <a name="get-passwordauthenticationmethod"></a><span data-ttu-id="ce5ce-103">获取 passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ce5ce-103">Get passwordAuthenticationMethod</span></span>

<span data-ttu-id="ce5ce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce5ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce5ce-105">检索密码身份验证方法 [对象的属性和](../resources/passwordauthenticationmethod.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="ce5ce-105">Retrieve the properties and relationships of a [password authentication method](../resources/passwordauthenticationmethod.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ce5ce-106">权限</span><span class="sxs-lookup"><span data-stu-id="ce5ce-106">Permissions</span></span>

<span data-ttu-id="ce5ce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce5ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="ce5ce-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="ce5ce-109">Permissions acting on self</span></span>

|<span data-ttu-id="ce5ce-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce5ce-110">Permission type</span></span>      | <span data-ttu-id="ce5ce-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce5ce-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="ce5ce-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce5ce-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce5ce-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce5ce-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="ce5ce-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce5ce-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce5ce-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce5ce-115">Not supported.</span></span> |
| <span data-ttu-id="ce5ce-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce5ce-116">Application</span></span>                            | <span data-ttu-id="ce5ce-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce5ce-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="ce5ce-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="ce5ce-118">Permissions acting on other users</span></span>

|<span data-ttu-id="ce5ce-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce5ce-119">Permission type</span></span>      | <span data-ttu-id="ce5ce-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce5ce-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="ce5ce-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce5ce-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce5ce-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce5ce-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="ce5ce-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce5ce-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce5ce-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce5ce-124">Not supported.</span></span> |
| <span data-ttu-id="ce5ce-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce5ce-125">Application</span></span>                            | <span data-ttu-id="ce5ce-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce5ce-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="ce5ce-127">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="ce5ce-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="ce5ce-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="ce5ce-128">Global admin</span></span>
* <span data-ttu-id="ce5ce-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="ce5ce-129">Global reader</span></span>
* <span data-ttu-id="ce5ce-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="ce5ce-130">Privileged authentication admin</span></span>
* <span data-ttu-id="ce5ce-131">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="ce5ce-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="ce5ce-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce5ce-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce5ce-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ce5ce-133">Optional query parameters</span></span>

<span data-ttu-id="ce5ce-134">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="ce5ce-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce5ce-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce5ce-135">Request headers</span></span>

| <span data-ttu-id="ce5ce-136">名称</span><span class="sxs-lookup"><span data-stu-id="ce5ce-136">Name</span></span>      |<span data-ttu-id="ce5ce-137">说明</span><span class="sxs-lookup"><span data-stu-id="ce5ce-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ce5ce-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce5ce-138">Authorization</span></span> | <span data-ttu-id="ce5ce-139">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="ce5ce-139">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce5ce-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce5ce-140">Request body</span></span>

<span data-ttu-id="ce5ce-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ce5ce-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce5ce-142">响应</span><span class="sxs-lookup"><span data-stu-id="ce5ce-142">Response</span></span>

<span data-ttu-id="ce5ce-143">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ce5ce-143">If successful, this method returns a `200 OK` response code and the requested [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ce5ce-144">示例</span><span class="sxs-lookup"><span data-stu-id="ce5ce-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce5ce-145">请求</span><span class="sxs-lookup"><span data-stu-id="ce5ce-145">Request</span></span>

<span data-ttu-id="ce5ce-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ce5ce-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce5ce-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce5ce-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods/{id}
```
# <a name="c"></a>[<span data-ttu-id="ce5ce-148">C#</span><span class="sxs-lookup"><span data-stu-id="ce5ce-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce5ce-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce5ce-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce5ce-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce5ce-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce5ce-151">Java</span><span class="sxs-lookup"><span data-stu-id="ce5ce-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ce5ce-152">响应</span><span class="sxs-lookup"><span data-stu-id="ce5ce-152">Response</span></span>

<span data-ttu-id="ce5ce-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ce5ce-153">The following is an example of the response.</span></span>

> <span data-ttu-id="ce5ce-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ce5ce-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
