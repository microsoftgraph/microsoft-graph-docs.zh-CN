---
title: 获取 authenticationMethod
description: 检索 authenticationMethod 对象的属性和关系。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e951cf5e7b64bf7fef411728acac0f8d21b9e51d
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796460"
---
# <a name="get-authenticationmethod"></a><span data-ttu-id="d763b-103">获取 authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d763b-103">Get authenticationMethod</span></span>

<span data-ttu-id="d763b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d763b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d763b-105">检索 [authenticationMethod 对象的属性和](../resources/authenticationmethod.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="d763b-105">Retrieve the properties and relationships of an [authenticationMethod](../resources/authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d763b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d763b-106">Permissions</span></span>

<span data-ttu-id="d763b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d763b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d763b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d763b-109">Permission type</span></span>                        | <span data-ttu-id="d763b-110">对自身执行 (权限从最低特权到最多特权) </span><span class="sxs-lookup"><span data-stu-id="d763b-110">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="d763b-111">对他人操作的权限 (权限从最低特权到最多特权) </span><span class="sxs-lookup"><span data-stu-id="d763b-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="d763b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d763b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d763b-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d763b-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="d763b-114">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d763b-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="d763b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d763b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d763b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d763b-116">Not supported.</span></span> | <span data-ttu-id="d763b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d763b-117">Not supported.</span></span> |
| <span data-ttu-id="d763b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="d763b-118">Application</span></span>                            | <span data-ttu-id="d763b-119">不适用</span><span class="sxs-lookup"><span data-stu-id="d763b-119">Not applicable.</span></span> | <span data-ttu-id="d763b-120">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d763b-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="d763b-121">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="d763b-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="d763b-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="d763b-122">Global admin</span></span>
* <span data-ttu-id="d763b-123">全局读取者</span><span class="sxs-lookup"><span data-stu-id="d763b-123">Global reader</span></span>
* <span data-ttu-id="d763b-124">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="d763b-124">Privileged authentication admin</span></span>
* <span data-ttu-id="d763b-125">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="d763b-125">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="d763b-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d763b-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods/{id}
GET /users/{id | userPrincipalName}/authentication/methods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d763b-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d763b-127">Optional query parameters</span></span>

<span data-ttu-id="d763b-128">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="d763b-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d763b-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="d763b-129">Request headers</span></span>

| <span data-ttu-id="d763b-130">名称</span><span class="sxs-lookup"><span data-stu-id="d763b-130">Name</span></span>      |<span data-ttu-id="d763b-131">说明</span><span class="sxs-lookup"><span data-stu-id="d763b-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d763b-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="d763b-132">Authorization</span></span> | <span data-ttu-id="d763b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d763b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d763b-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="d763b-135">Request body</span></span>

<span data-ttu-id="d763b-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d763b-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d763b-137">响应</span><span class="sxs-lookup"><span data-stu-id="d763b-137">Response</span></span>

<span data-ttu-id="d763b-138">如果成功，此方法在响应正文中返回响应代码和请求的 `200 OK` [authenticationMethod](../resources/authenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d763b-138">If successful, this method returns a `200 OK` response code and the requested [authenticationMethod](../resources/authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d763b-139">示例</span><span class="sxs-lookup"><span data-stu-id="d763b-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d763b-140">请求</span><span class="sxs-lookup"><span data-stu-id="d763b-140">Request</span></span>

<span data-ttu-id="d763b-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d763b-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d763b-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="d763b-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/methods/{id}
```
# <a name="c"></a>[<span data-ttu-id="d763b-143">C#</span><span class="sxs-lookup"><span data-stu-id="d763b-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d763b-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d763b-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d763b-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d763b-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d763b-146">Java</span><span class="sxs-lookup"><span data-stu-id="d763b-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-authenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d763b-147">响应</span><span class="sxs-lookup"><span data-stu-id="d763b-147">Response</span></span>

<span data-ttu-id="d763b-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d763b-148">The following is an example of the response.</span></span>

> <span data-ttu-id="d763b-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d763b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
