---
title: 获取 passwordAuthenticationMethod
description: 检索 passwordauthenticationmethod 对象的属性和关系。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2112788ce5127326e0e82ef91c1068b5b56ec14a
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515590"
---
# <a name="get-passwordauthenticationmethod"></a><span data-ttu-id="9beb6-103">获取 passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9beb6-103">Get passwordAuthenticationMethod</span></span>

<span data-ttu-id="9beb6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9beb6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9beb6-105">检索密码身份验证方法 [对象的属性和](../resources/passwordauthenticationmethod.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="9beb6-105">Retrieve the properties and relationships of a [password authentication method](../resources/passwordauthenticationmethod.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="9beb6-106">权限</span><span class="sxs-lookup"><span data-stu-id="9beb6-106">Permissions</span></span>

<span data-ttu-id="9beb6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9beb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="9beb6-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="9beb6-109">Permissions acting on self</span></span>

|<span data-ttu-id="9beb6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9beb6-110">Permission type</span></span>      | <span data-ttu-id="9beb6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9beb6-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="9beb6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9beb6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9beb6-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9beb6-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="9beb6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9beb6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9beb6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9beb6-115">Not supported.</span></span> |
| <span data-ttu-id="9beb6-116">Application</span><span class="sxs-lookup"><span data-stu-id="9beb6-116">Application</span></span>                            | <span data-ttu-id="9beb6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9beb6-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="9beb6-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="9beb6-118">Permissions acting on other users</span></span>

|<span data-ttu-id="9beb6-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="9beb6-119">Permission type</span></span>      | <span data-ttu-id="9beb6-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9beb6-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="9beb6-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9beb6-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="9beb6-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9beb6-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="9beb6-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9beb6-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9beb6-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="9beb6-124">Not supported.</span></span> |
| <span data-ttu-id="9beb6-125">Application</span><span class="sxs-lookup"><span data-stu-id="9beb6-125">Application</span></span>                            | <span data-ttu-id="9beb6-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9beb6-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="9beb6-127">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="9beb6-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="9beb6-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="9beb6-128">Global admin</span></span>
* <span data-ttu-id="9beb6-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="9beb6-129">Global reader</span></span>
* <span data-ttu-id="9beb6-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="9beb6-130">Privileged authentication admin</span></span>
* <span data-ttu-id="9beb6-131">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="9beb6-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="9beb6-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9beb6-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9beb6-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9beb6-133">Optional query parameters</span></span>

<span data-ttu-id="9beb6-134">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="9beb6-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9beb6-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="9beb6-135">Request headers</span></span>

| <span data-ttu-id="9beb6-136">名称</span><span class="sxs-lookup"><span data-stu-id="9beb6-136">Name</span></span>      |<span data-ttu-id="9beb6-137">说明</span><span class="sxs-lookup"><span data-stu-id="9beb6-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9beb6-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="9beb6-138">Authorization</span></span> | <span data-ttu-id="9beb6-139">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="9beb6-139">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9beb6-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="9beb6-140">Request body</span></span>

<span data-ttu-id="9beb6-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9beb6-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9beb6-142">响应</span><span class="sxs-lookup"><span data-stu-id="9beb6-142">Response</span></span>

<span data-ttu-id="9beb6-143">如果成功，此方法在响应正文中返回响应代码和请求 `200 OK` [的 passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9beb6-143">If successful, this method returns a `200 OK` response code and the requested [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9beb6-144">示例</span><span class="sxs-lookup"><span data-stu-id="9beb6-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9beb6-145">请求</span><span class="sxs-lookup"><span data-stu-id="9beb6-145">Request</span></span>

<span data-ttu-id="9beb6-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9beb6-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9beb6-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="9beb6-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods/{id}
```
# <a name="c"></a>[<span data-ttu-id="9beb6-148">C#</span><span class="sxs-lookup"><span data-stu-id="9beb6-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9beb6-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9beb6-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9beb6-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9beb6-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9beb6-151">Java</span><span class="sxs-lookup"><span data-stu-id="9beb6-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9beb6-152">响应</span><span class="sxs-lookup"><span data-stu-id="9beb6-152">Response</span></span>

<span data-ttu-id="9beb6-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9beb6-153">The following is an example of the response.</span></span>

> <span data-ttu-id="9beb6-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9beb6-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
