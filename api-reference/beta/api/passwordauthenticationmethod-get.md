---
title: 获取 passwordAuthenticationMethod
description: 检索 passwordauthenticationmethod 对象的属性和关系。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1cd38f82b3b79002c7fe31f9b6e6858b0801e44c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040344"
---
# <a name="get-passwordauthenticationmethod"></a><span data-ttu-id="778f4-103">获取 passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="778f4-103">Get passwordAuthenticationMethod</span></span>

<span data-ttu-id="778f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="778f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="778f4-105">检索 [密码身份验证方法](../resources/passwordauthenticationmethod.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="778f4-105">Retrieve the properties and relationships of a [password authentication method](../resources/passwordauthenticationmethod.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="778f4-106">权限</span><span class="sxs-lookup"><span data-stu-id="778f4-106">Permissions</span></span>

<span data-ttu-id="778f4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="778f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="778f4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="778f4-109">Permission type</span></span>                        | <span data-ttu-id="778f4-110">从最高特权到最高特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="778f4-110">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="778f4-111">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="778f4-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="778f4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="778f4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="778f4-113">UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、All 和 All</span><span class="sxs-lookup"><span data-stu-id="778f4-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="778f4-114">UserAuthenticationMethod、UserAuthenticationMethod 和所有</span><span class="sxs-lookup"><span data-stu-id="778f4-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="778f4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="778f4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="778f4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="778f4-116">Not supported.</span></span> | <span data-ttu-id="778f4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="778f4-117">Not supported.</span></span> |
| <span data-ttu-id="778f4-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="778f4-118">Application</span></span>                            | <span data-ttu-id="778f4-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="778f4-119">Not supported.</span></span> | <span data-ttu-id="778f4-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="778f4-120">Not supported.</span></span> |

<span data-ttu-id="778f4-121">对于在其他用户上执行管理的委派方案，管理员需要 [以下角色之一](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="778f4-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="778f4-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="778f4-122">Global admin</span></span>
* <span data-ttu-id="778f4-123">全局读取者</span><span class="sxs-lookup"><span data-stu-id="778f4-123">Global reader</span></span>
* <span data-ttu-id="778f4-124">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="778f4-124">Privileged authentication admin</span></span>
* <span data-ttu-id="778f4-125">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="778f4-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="778f4-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="778f4-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods/{id}
GET /users/{id}/authentication/passwordMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="778f4-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="778f4-127">Optional query parameters</span></span>

<span data-ttu-id="778f4-128">此方法不支持用于自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="778f4-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="778f4-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="778f4-129">Request headers</span></span>

| <span data-ttu-id="778f4-130">名称</span><span class="sxs-lookup"><span data-stu-id="778f4-130">Name</span></span>      |<span data-ttu-id="778f4-131">说明</span><span class="sxs-lookup"><span data-stu-id="778f4-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="778f4-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="778f4-132">Authorization</span></span> | <span data-ttu-id="778f4-133">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="778f4-133">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="778f4-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="778f4-134">Request body</span></span>

<span data-ttu-id="778f4-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="778f4-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="778f4-136">响应</span><span class="sxs-lookup"><span data-stu-id="778f4-136">Response</span></span>

<span data-ttu-id="778f4-137">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="778f4-137">If successful, this method returns a `200 OK` response code and the requested [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="778f4-138">示例</span><span class="sxs-lookup"><span data-stu-id="778f4-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="778f4-139">请求</span><span class="sxs-lookup"><span data-stu-id="778f4-139">Request</span></span>

<span data-ttu-id="778f4-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="778f4-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="778f4-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="778f4-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods/{id}
```
# <a name="c"></a>[<span data-ttu-id="778f4-142">C#</span><span class="sxs-lookup"><span data-stu-id="778f4-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="778f4-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="778f4-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="778f4-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="778f4-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="778f4-145">响应</span><span class="sxs-lookup"><span data-stu-id="778f4-145">Response</span></span>

<span data-ttu-id="778f4-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="778f4-146">The following is an example of the response.</span></span>

> <span data-ttu-id="778f4-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="778f4-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


