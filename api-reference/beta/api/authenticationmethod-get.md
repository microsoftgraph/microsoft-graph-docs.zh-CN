---
title: 获取 authenticationMethod
description: 检索 authenticationMethod 对象的属性和关系。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 10495d9b66c63207ec1b1376efcb1796b9e4c9ad
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760026"
---
# <a name="get-authenticationmethod"></a><span data-ttu-id="84e6d-103">获取 authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="84e6d-103">Get authenticationMethod</span></span>

<span data-ttu-id="84e6d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84e6d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84e6d-105">检索 [authenticationMethod 对象的属性和](../resources/authenticationmethod.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="84e6d-105">Retrieve the properties and relationships of an [authenticationMethod](../resources/authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="84e6d-106">权限</span><span class="sxs-lookup"><span data-stu-id="84e6d-106">Permissions</span></span>

<span data-ttu-id="84e6d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84e6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84e6d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="84e6d-109">Permission type</span></span>                        | <span data-ttu-id="84e6d-110">自行操作的权限 (权限从最低权限级别) </span><span class="sxs-lookup"><span data-stu-id="84e6d-110">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="84e6d-111">对他人操作的权限 (权限从最低到最多特权) </span><span class="sxs-lookup"><span data-stu-id="84e6d-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="84e6d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84e6d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="84e6d-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84e6d-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="84e6d-114">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84e6d-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="84e6d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84e6d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84e6d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="84e6d-116">Not supported.</span></span> | <span data-ttu-id="84e6d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="84e6d-117">Not supported.</span></span> |
| <span data-ttu-id="84e6d-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="84e6d-118">Application</span></span>                            | <span data-ttu-id="84e6d-119">不适用。</span><span class="sxs-lookup"><span data-stu-id="84e6d-119">Not applicable.</span></span> | <span data-ttu-id="84e6d-120">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84e6d-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="84e6d-121">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="84e6d-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="84e6d-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="84e6d-122">Global admin</span></span>
* <span data-ttu-id="84e6d-123">全局读取者</span><span class="sxs-lookup"><span data-stu-id="84e6d-123">Global reader</span></span>
* <span data-ttu-id="84e6d-124">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="84e6d-124">Privileged authentication admin</span></span>
* <span data-ttu-id="84e6d-125">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="84e6d-125">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="84e6d-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84e6d-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods/{id}
GET /users/{id | userPrincipalName}/authentication/methods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84e6d-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="84e6d-127">Optional query parameters</span></span>

<span data-ttu-id="84e6d-128">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="84e6d-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84e6d-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="84e6d-129">Request headers</span></span>

| <span data-ttu-id="84e6d-130">名称</span><span class="sxs-lookup"><span data-stu-id="84e6d-130">Name</span></span>      |<span data-ttu-id="84e6d-131">说明</span><span class="sxs-lookup"><span data-stu-id="84e6d-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="84e6d-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="84e6d-132">Authorization</span></span> | <span data-ttu-id="84e6d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="84e6d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84e6d-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="84e6d-135">Request body</span></span>

<span data-ttu-id="84e6d-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="84e6d-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84e6d-137">响应</span><span class="sxs-lookup"><span data-stu-id="84e6d-137">Response</span></span>

<span data-ttu-id="84e6d-138">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [authenticationMethod](../resources/authenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="84e6d-138">If successful, this method returns a `200 OK` response code and the requested [authenticationMethod](../resources/authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="84e6d-139">示例</span><span class="sxs-lookup"><span data-stu-id="84e6d-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="84e6d-140">请求</span><span class="sxs-lookup"><span data-stu-id="84e6d-140">Request</span></span>

<span data-ttu-id="84e6d-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="84e6d-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="84e6d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="84e6d-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/methods/{id}
```
# <a name="c"></a>[<span data-ttu-id="84e6d-143">C#</span><span class="sxs-lookup"><span data-stu-id="84e6d-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84e6d-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84e6d-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84e6d-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84e6d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84e6d-146">Java</span><span class="sxs-lookup"><span data-stu-id="84e6d-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-authenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="84e6d-147">响应</span><span class="sxs-lookup"><span data-stu-id="84e6d-147">Response</span></span>

<span data-ttu-id="84e6d-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="84e6d-148">The following is an example of the response.</span></span>

> <span data-ttu-id="84e6d-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="84e6d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "odata.type": "#microsoft.graph.phoneAuthenticationMethod",
  "id": "3179e48a-750b-4051-897c-87b9720928f7",
  "phoneNumber": "+1 2065555555",
  "authenticationPhoneType": "mobile",
  "smsSignInState": "ready"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get authenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
