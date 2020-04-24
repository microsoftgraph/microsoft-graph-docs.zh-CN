---
title: 列出 passwordMethods
description: 检索 passwordauthenticationmethod 对象的列表。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: efbd934a1043f99583eba27c32c1b1e2e76fb288
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805892"
---
# <a name="list-passwordmethods"></a><span data-ttu-id="d1511-103">列出 passwordMethods</span><span class="sxs-lookup"><span data-stu-id="d1511-103">List passwordMethods</span></span>

<span data-ttu-id="d1511-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1511-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1511-105">检索[密码身份验证方法](../resources/passwordauthenticationmethod.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="d1511-105">Retrieve a list of [password authentication method](../resources/passwordauthenticationmethod.md) objects.</span></span> <span data-ttu-id="d1511-106">这将只返回一个对象，因为用户只能有一个密码。</span><span class="sxs-lookup"><span data-stu-id="d1511-106">This will return exactly one object, as a user can have exactly one password.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1511-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="d1511-107">Permissions</span></span>

<span data-ttu-id="d1511-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1511-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d1511-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1511-110">Permission type</span></span>                        | <span data-ttu-id="d1511-111">作用于自助的权限（从最高特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1511-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="d1511-112">对其他用户的权限（从最低到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1511-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="d1511-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1511-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1511-114">UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、All 和 All</span><span class="sxs-lookup"><span data-stu-id="d1511-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="d1511-115">UserAuthenticationMethod、UserAuthenticationMethod 和所有</span><span class="sxs-lookup"><span data-stu-id="d1511-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="d1511-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1511-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1511-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1511-117">Not supported.</span></span> | <span data-ttu-id="d1511-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1511-118">Not supported.</span></span> |
| <span data-ttu-id="d1511-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1511-119">Application</span></span>                            | <span data-ttu-id="d1511-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1511-120">Not supported.</span></span> | <span data-ttu-id="d1511-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1511-121">Not supported.</span></span> |

<span data-ttu-id="d1511-122">对于在其他用户上执行管理的委派方案，管理员需要[以下角色之一](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="d1511-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="d1511-123">全局管理员</span><span class="sxs-lookup"><span data-stu-id="d1511-123">Global admin</span></span>
* <span data-ttu-id="d1511-124">全局读取者</span><span class="sxs-lookup"><span data-stu-id="d1511-124">Global reader</span></span>
* <span data-ttu-id="d1511-125">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="d1511-125">Privileged authentication admin</span></span>
* <span data-ttu-id="d1511-126">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="d1511-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="d1511-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1511-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods
GET /users/{id}/authentication/passwordMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1511-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d1511-128">Optional query parameters</span></span>

<span data-ttu-id="d1511-129">此方法不支持用于自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="d1511-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1511-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1511-130">Request headers</span></span>

| <span data-ttu-id="d1511-131">名称</span><span class="sxs-lookup"><span data-stu-id="d1511-131">Name</span></span>      |<span data-ttu-id="d1511-132">说明</span><span class="sxs-lookup"><span data-stu-id="d1511-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d1511-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1511-133">Authorization</span></span> | <span data-ttu-id="d1511-134">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="d1511-134">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1511-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1511-135">Request body</span></span>

<span data-ttu-id="d1511-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d1511-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1511-137">响应</span><span class="sxs-lookup"><span data-stu-id="d1511-137">Response</span></span>

<span data-ttu-id="d1511-138">如果成功，此方法在响应`200 OK`正文中返回响应代码和[passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="d1511-138">If successful, this method returns a `200 OK` response code and a collection of [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1511-139">示例</span><span class="sxs-lookup"><span data-stu-id="d1511-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d1511-140">请求</span><span class="sxs-lookup"><span data-stu-id="d1511-140">Request</span></span>

<span data-ttu-id="d1511-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d1511-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d1511-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1511-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordmethods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods
```
# <a name="c"></a>[<span data-ttu-id="d1511-143">C#</span><span class="sxs-lookup"><span data-stu-id="d1511-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordmethods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1511-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1511-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordmethods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1511-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1511-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordmethods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d1511-146">响应</span><span class="sxs-lookup"><span data-stu-id="d1511-146">Response</span></span>

<span data-ttu-id="d1511-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d1511-147">The following is an example of the response.</span></span>

> <span data-ttu-id="d1511-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d1511-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
