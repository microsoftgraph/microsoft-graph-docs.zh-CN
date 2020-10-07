---
title: 获取 authenticationMethod
description: 检索 authenticationMethod 对象的属性和关系。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5fba175c46aa86b0db649cb69eee9cad6e8cbc8a
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372395"
---
# <a name="get-authenticationmethod"></a><span data-ttu-id="da435-103">获取 authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="da435-103">Get authenticationMethod</span></span>

<span data-ttu-id="da435-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da435-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da435-105">检索 [authenticationMethod](../resources/authenticationmethod.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="da435-105">Retrieve the properties and relationships of an [authenticationMethod](../resources/authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="da435-106">权限</span><span class="sxs-lookup"><span data-stu-id="da435-106">Permissions</span></span>

<span data-ttu-id="da435-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da435-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="da435-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="da435-109">Permission type</span></span>                        | <span data-ttu-id="da435-110">从最高特权到最高特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="da435-110">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="da435-111">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="da435-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="da435-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da435-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="da435-113">UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、All 和 All</span><span class="sxs-lookup"><span data-stu-id="da435-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="da435-114">UserAuthenticationMethod、UserAuthenticationMethod 和所有</span><span class="sxs-lookup"><span data-stu-id="da435-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="da435-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da435-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da435-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="da435-116">Not supported.</span></span> | <span data-ttu-id="da435-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="da435-117">Not supported.</span></span> |
| <span data-ttu-id="da435-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="da435-118">Application</span></span>                            | <span data-ttu-id="da435-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="da435-119">Not supported.</span></span> | <span data-ttu-id="da435-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="da435-120">Not supported.</span></span> |

<span data-ttu-id="da435-121">对于在其他用户上执行管理的委派方案，管理员需要 [以下角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="da435-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="da435-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="da435-122">Global admin</span></span>
* <span data-ttu-id="da435-123">全局读取者</span><span class="sxs-lookup"><span data-stu-id="da435-123">Global reader</span></span>
* <span data-ttu-id="da435-124">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="da435-124">Privileged authentication admin</span></span>
* <span data-ttu-id="da435-125">身份验证管理员 (仅查看被屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="da435-125">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="da435-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da435-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods/{id}
GET /users/{id}/authentication/methods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da435-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="da435-127">Optional query parameters</span></span>

<span data-ttu-id="da435-128">此方法不支持用于自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="da435-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da435-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="da435-129">Request headers</span></span>

| <span data-ttu-id="da435-130">名称</span><span class="sxs-lookup"><span data-stu-id="da435-130">Name</span></span>      |<span data-ttu-id="da435-131">说明</span><span class="sxs-lookup"><span data-stu-id="da435-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="da435-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="da435-132">Authorization</span></span> | <span data-ttu-id="da435-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="da435-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da435-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="da435-135">Request body</span></span>

<span data-ttu-id="da435-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="da435-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da435-137">响应</span><span class="sxs-lookup"><span data-stu-id="da435-137">Response</span></span>

<span data-ttu-id="da435-138">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [authenticationMethod](../resources/authenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="da435-138">If successful, this method returns a `200 OK` response code and the requested [authenticationMethod](../resources/authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="da435-139">示例</span><span class="sxs-lookup"><span data-stu-id="da435-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="da435-140">请求</span><span class="sxs-lookup"><span data-stu-id="da435-140">Request</span></span>

<span data-ttu-id="da435-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="da435-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="da435-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="da435-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/methods/{id}
```
# <a name="c"></a>[<span data-ttu-id="da435-143">C#</span><span class="sxs-lookup"><span data-stu-id="da435-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da435-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da435-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da435-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da435-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="da435-146">响应</span><span class="sxs-lookup"><span data-stu-id="da435-146">Response</span></span>

<span data-ttu-id="da435-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="da435-147">The following is an example of the response.</span></span>

> <span data-ttu-id="da435-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="da435-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
