---
title: 获取 phoneAuthenticationMethod
description: 检索单个 phoneAuthenticationMethod 对象。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4aea872d99deedb3fbf952954e2d6ff691994220
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957286"
---
# <a name="get-phoneauthenticationmethod"></a><span data-ttu-id="32bc8-103">获取 phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="32bc8-103">Get phoneAuthenticationMethod</span></span>

<span data-ttu-id="32bc8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32bc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32bc8-105">检索单个 [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="32bc8-105">Retrieve a single [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="32bc8-106">权限</span><span class="sxs-lookup"><span data-stu-id="32bc8-106">Permissions</span></span>

<span data-ttu-id="32bc8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32bc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="32bc8-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="32bc8-109">Permissions acting on self</span></span>

|<span data-ttu-id="32bc8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="32bc8-110">Permission type</span></span>      | <span data-ttu-id="32bc8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="32bc8-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="32bc8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32bc8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="32bc8-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32bc8-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="32bc8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32bc8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32bc8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="32bc8-115">Not supported.</span></span> |
| <span data-ttu-id="32bc8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="32bc8-116">Application</span></span>                            | <span data-ttu-id="32bc8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="32bc8-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="32bc8-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="32bc8-118">Permissions acting on other users</span></span>

|<span data-ttu-id="32bc8-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="32bc8-119">Permission type</span></span>      | <span data-ttu-id="32bc8-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="32bc8-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="32bc8-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32bc8-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="32bc8-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32bc8-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="32bc8-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32bc8-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32bc8-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="32bc8-124">Not supported.</span></span> |
| <span data-ttu-id="32bc8-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="32bc8-125">Application</span></span>                            | <span data-ttu-id="32bc8-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32bc8-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="32bc8-127">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="32bc8-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="32bc8-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="32bc8-128">Global admin</span></span>
* <span data-ttu-id="32bc8-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="32bc8-129">Global reader</span></span>
* <span data-ttu-id="32bc8-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="32bc8-130">Privileged authentication admin</span></span>
* <span data-ttu-id="32bc8-131">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="32bc8-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="32bc8-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32bc8-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/phoneMethods/{id}
GET /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```
<span data-ttu-id="32bc8-133">与要 `id` 检索的 phoneType 对应的值是下列值之一：</span><span class="sxs-lookup"><span data-stu-id="32bc8-133">The value of `id` corresponding to the phoneType to retrieve is one of the following:</span></span>
+ <span data-ttu-id="32bc8-134">`b6332ec1-7057-4abe-9331-3d72feddfe41` 检索 `alternateMobile` **phoneType**。</span><span class="sxs-lookup"><span data-stu-id="32bc8-134">`b6332ec1-7057-4abe-9331-3d72feddfe41` to retrieve the `alternateMobile` **phoneType**.</span></span>
+ <span data-ttu-id="32bc8-135">`e37fc753-ff3b-4958-9484-eaa9425c82bc` 检索 `office` **phoneType**。</span><span class="sxs-lookup"><span data-stu-id="32bc8-135">`e37fc753-ff3b-4958-9484-eaa9425c82bc` to retrieve the `office` **phoneType**.</span></span>
+ <span data-ttu-id="32bc8-136">`3179e48a-750b-4051-897c-87b9720928f7` 检索 `mobile` **phoneType**。</span><span class="sxs-lookup"><span data-stu-id="32bc8-136">`3179e48a-750b-4051-897c-87b9720928f7` to retrieve the `mobile` **phoneType**.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="32bc8-137">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="32bc8-137">Optional query parameters</span></span>

<span data-ttu-id="32bc8-138">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="32bc8-138">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="32bc8-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="32bc8-139">Request headers</span></span>

| <span data-ttu-id="32bc8-140">名称</span><span class="sxs-lookup"><span data-stu-id="32bc8-140">Name</span></span>      |<span data-ttu-id="32bc8-141">说明</span><span class="sxs-lookup"><span data-stu-id="32bc8-141">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="32bc8-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="32bc8-142">Authorization</span></span> | <span data-ttu-id="32bc8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="32bc8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32bc8-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="32bc8-145">Request body</span></span>

<span data-ttu-id="32bc8-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="32bc8-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32bc8-147">响应</span><span class="sxs-lookup"><span data-stu-id="32bc8-147">Response</span></span>

<span data-ttu-id="32bc8-148">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="32bc8-148">If successful, this method returns a `200 OK` response code and the requested [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="32bc8-149">示例</span><span class="sxs-lookup"><span data-stu-id="32bc8-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="32bc8-150">请求</span><span class="sxs-lookup"><span data-stu-id="32bc8-150">Request</span></span>

<span data-ttu-id="32bc8-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="32bc8-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="32bc8-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="32bc8-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phoneauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```
# <a name="c"></a>[<span data-ttu-id="32bc8-153">C#</span><span class="sxs-lookup"><span data-stu-id="32bc8-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32bc8-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32bc8-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32bc8-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32bc8-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32bc8-156">Java</span><span class="sxs-lookup"><span data-stu-id="32bc8-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="32bc8-157">响应</span><span class="sxs-lookup"><span data-stu-id="32bc8-157">Response</span></span>

<span data-ttu-id="32bc8-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="32bc8-158">The following is an example of the response.</span></span>

> <span data-ttu-id="32bc8-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="32bc8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "mobile",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get phoneAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
