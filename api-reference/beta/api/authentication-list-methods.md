---
title: List 方法
description: 检索身份验证方法对象的列表。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac205663b183e91b0925a3c246e9dd5a78c9aeba
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796554"
---
# <a name="list-methods"></a><span data-ttu-id="aca20-103">List 方法</span><span class="sxs-lookup"><span data-stu-id="aca20-103">List methods</span></span>

<span data-ttu-id="aca20-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aca20-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aca20-105">检索身份验证 [方法对象](../resources/authenticationmethod.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="aca20-105">Retrieve a list of [authentication method](../resources/authenticationmethod.md) objects.</span></span> <span data-ttu-id="aca20-106">当前仅[返回电话身份验证](../resources/phoneauthenticationmethod.md)[方法和密码身份验证](../resources/passwordauthenticationmethod.md)方法对象。</span><span class="sxs-lookup"><span data-stu-id="aca20-106">Currently only [phone authentication method](../resources/phoneauthenticationmethod.md) and [password authentication method](../resources/passwordauthenticationmethod.md) objects are returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="aca20-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="aca20-107">Permissions</span></span>

<span data-ttu-id="aca20-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aca20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="aca20-110">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="aca20-110">Permissions acting on self</span></span>

|<span data-ttu-id="aca20-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aca20-111">Permission type</span></span>      | <span data-ttu-id="aca20-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aca20-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="aca20-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aca20-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="aca20-114">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aca20-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="aca20-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aca20-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aca20-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aca20-116">Not supported.</span></span> |
| <span data-ttu-id="aca20-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="aca20-117">Application</span></span>                            | <span data-ttu-id="aca20-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="aca20-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="aca20-119">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="aca20-119">Permissions acting on other users</span></span>

|<span data-ttu-id="aca20-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="aca20-120">Permission type</span></span>      | <span data-ttu-id="aca20-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aca20-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="aca20-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aca20-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="aca20-123">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aca20-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="aca20-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aca20-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aca20-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="aca20-125">Not supported.</span></span> |
| <span data-ttu-id="aca20-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="aca20-126">Application</span></span>                            | <span data-ttu-id="aca20-127">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aca20-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="aca20-128">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="aca20-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="aca20-129">全局管理员</span><span class="sxs-lookup"><span data-stu-id="aca20-129">Global admin</span></span>
* <span data-ttu-id="aca20-130">全局读取者</span><span class="sxs-lookup"><span data-stu-id="aca20-130">Global reader</span></span>
* <span data-ttu-id="aca20-131">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="aca20-131">Privileged authentication admin</span></span>
* <span data-ttu-id="aca20-132">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="aca20-132">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="aca20-133">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aca20-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods
GET /users/{id | userPrincipalName}/authentication/methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aca20-134">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="aca20-134">Optional query parameters</span></span>

<span data-ttu-id="aca20-135">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="aca20-135">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aca20-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="aca20-136">Request headers</span></span>

| <span data-ttu-id="aca20-137">名称</span><span class="sxs-lookup"><span data-stu-id="aca20-137">Name</span></span>      |<span data-ttu-id="aca20-138">说明</span><span class="sxs-lookup"><span data-stu-id="aca20-138">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aca20-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="aca20-139">Authorization</span></span> | <span data-ttu-id="aca20-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aca20-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aca20-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="aca20-142">Request body</span></span>

<span data-ttu-id="aca20-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aca20-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aca20-144">响应</span><span class="sxs-lookup"><span data-stu-id="aca20-144">Response</span></span>

<span data-ttu-id="aca20-145">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [authenticationMethod](../resources/authenticationmethod.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="aca20-145">If successful, this method returns a `200 OK` response code and a collection of [authenticationMethod](../resources/authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aca20-146">示例</span><span class="sxs-lookup"><span data-stu-id="aca20-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aca20-147">请求</span><span class="sxs-lookup"><span data-stu-id="aca20-147">Request</span></span>

<span data-ttu-id="aca20-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aca20-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aca20-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="aca20-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_methods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/methods
```
# <a name="c"></a>[<span data-ttu-id="aca20-150">C#</span><span class="sxs-lookup"><span data-stu-id="aca20-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-methods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aca20-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aca20-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-methods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aca20-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aca20-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-methods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aca20-153">Java</span><span class="sxs-lookup"><span data-stu-id="aca20-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-methods-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aca20-154">响应</span><span class="sxs-lookup"><span data-stu-id="aca20-154">Response</span></span>

<span data-ttu-id="aca20-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aca20-155">The following is an example of the response.</span></span>

> <span data-ttu-id="aca20-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aca20-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "odata.type": "#microsoft.graph.passwordAuthenticationMethod",
      "id": "28c10230-6103-485e-b985-444c60001490",
      "password": null,
      "creationDateTime": null
    },
    {
      "odata.type": "#microsoft.graph.phoneAuthenticationMethod",
      "id": "3179e48a-750b-4051-897c-87b9720928f7",
      "phoneNumber": "+1 2065555555",
      "authenticationPhoneType": "mobile",
      "smsSignInState": "ready"
    },
    {
      "odata.type": "#microsoft.graph.phoneAuthenticationMethod",
      "id": "b6332ec1-7057-4abe-9331-3d72feddfe41",
      "phoneNumber": "+1 2065555556",
      "authenticationPhoneType": "alternateMobile",
      "smsSignInState": "notSupported"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List methods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
