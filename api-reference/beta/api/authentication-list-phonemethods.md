---
title: 列出 phoneMethods
description: 检索电话身份验证方法对象的列表。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 996398e47431ad353e32f0f85a1d50f3f54bd712
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438580"
---
# <a name="list-phonemethods"></a><span data-ttu-id="69484-103">列出 phoneMethods</span><span class="sxs-lookup"><span data-stu-id="69484-103">List phoneMethods</span></span>

<span data-ttu-id="69484-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69484-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69484-105">检索电话 [身份验证方法对象](../resources/phoneauthenticationmethod.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="69484-105">Retrieve a list of [phone authentication method](../resources/phoneauthenticationmethod.md) objects.</span></span> <span data-ttu-id="69484-106">这将返回最多三个对象，因为用户最多有三部电话可用于身份验证。</span><span class="sxs-lookup"><span data-stu-id="69484-106">This will return up to three objects, as a user can have up to three phones usable for authentication.</span></span>

## <a name="permissions"></a><span data-ttu-id="69484-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="69484-107">Permissions</span></span>

<span data-ttu-id="69484-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69484-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="69484-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="69484-110">Permission type</span></span>                        | <span data-ttu-id="69484-111">自操作权限 (权限从最低到最特权) </span><span class="sxs-lookup"><span data-stu-id="69484-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="69484-112">对他人 (权限从最低到最特权) </span><span class="sxs-lookup"><span data-stu-id="69484-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="69484-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69484-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="69484-114">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69484-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="69484-115">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69484-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="69484-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69484-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69484-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="69484-117">Not supported.</span></span> | <span data-ttu-id="69484-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="69484-118">Not supported.</span></span> |
| <span data-ttu-id="69484-119">Application</span><span class="sxs-lookup"><span data-stu-id="69484-119">Application</span></span>                            | <span data-ttu-id="69484-120">不适用。</span><span class="sxs-lookup"><span data-stu-id="69484-120">Not applicable.</span></span> | <span data-ttu-id="69484-121">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69484-121">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="69484-122">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="69484-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="69484-123">全局管理员</span><span class="sxs-lookup"><span data-stu-id="69484-123">Global admin</span></span>
* <span data-ttu-id="69484-124">全局读取者</span><span class="sxs-lookup"><span data-stu-id="69484-124">Global reader</span></span>
* <span data-ttu-id="69484-125">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="69484-125">Privileged authentication admin</span></span>
* <span data-ttu-id="69484-126">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="69484-126">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="69484-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69484-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/phoneMethods
GET /users/{id | userPrincipalName}/authentication/phoneMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69484-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="69484-128">Optional query parameters</span></span>

<span data-ttu-id="69484-129">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="69484-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69484-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="69484-130">Request headers</span></span>

| <span data-ttu-id="69484-131">名称</span><span class="sxs-lookup"><span data-stu-id="69484-131">Name</span></span>      |<span data-ttu-id="69484-132">说明</span><span class="sxs-lookup"><span data-stu-id="69484-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="69484-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="69484-133">Authorization</span></span> | <span data-ttu-id="69484-134">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="69484-134">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="69484-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="69484-135">Request body</span></span>

<span data-ttu-id="69484-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="69484-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69484-137">响应</span><span class="sxs-lookup"><span data-stu-id="69484-137">Response</span></span>

<span data-ttu-id="69484-138">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="69484-138">If successful, this method returns a `200 OK` response code and a collection of [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="69484-139">示例</span><span class="sxs-lookup"><span data-stu-id="69484-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="69484-140">请求</span><span class="sxs-lookup"><span data-stu-id="69484-140">Request</span></span>

<span data-ttu-id="69484-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="69484-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="69484-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="69484-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phonemethods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/phoneMethods
```
# <a name="c"></a>[<span data-ttu-id="69484-143">C#</span><span class="sxs-lookup"><span data-stu-id="69484-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phonemethods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69484-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69484-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phonemethods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69484-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69484-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phonemethods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="69484-146">Java</span><span class="sxs-lookup"><span data-stu-id="69484-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-phonemethods-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="69484-147">响应</span><span class="sxs-lookup"><span data-stu-id="69484-147">Response</span></span>

<span data-ttu-id="69484-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="69484-148">The following is an example of the response.</span></span>

> <span data-ttu-id="69484-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="69484-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "phoneNumber": "+1 2065555555",
      "phoneType": "mobile",
      "smsSignInState": "ready",
      "id": "3179e48a-750b-4051-897c-87b9720928f7"
    },
    {
      "phoneNumber": "+1 2065555556",
      "phoneType": "alternateMobile",
      "smsSignInState": "notSupported",
      "id": "b6332ec1-7057-4abe-9331-3d72feddfe41"
    },
    {
      "phoneNumber": "+1 2065555557",
      "phoneType": "office",
      "smsSignInState": "notSupported",
      "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List phoneMethods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
