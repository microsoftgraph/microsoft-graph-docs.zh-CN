---
title: 获取 phoneAuthenticationMethod
description: 检索单个 phoneAuthenticationMethod 对象。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f968838fb5e492c548f154afd311c212a05334fc
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921649"
---
# <a name="get-phoneauthenticationmethod"></a><span data-ttu-id="8352d-103">获取 phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8352d-103">Get phoneAuthenticationMethod</span></span>

<span data-ttu-id="8352d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8352d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8352d-105">检索单个 [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8352d-105">Retrieve a single [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.</span></span> <span data-ttu-id="8352d-106">此方法仅适用于标准 Azure AD 和 B2B 用户，但不适用于 B2C 用户。</span><span class="sxs-lookup"><span data-stu-id="8352d-106">This method is available only for standard Azure AD and B2B users, but not B2C users.</span></span>

## <a name="permissions"></a><span data-ttu-id="8352d-107">权限</span><span class="sxs-lookup"><span data-stu-id="8352d-107">Permissions</span></span>

<span data-ttu-id="8352d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8352d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="8352d-110">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="8352d-110">Permissions acting on self</span></span>

|<span data-ttu-id="8352d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8352d-111">Permission type</span></span>      | <span data-ttu-id="8352d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8352d-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="8352d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8352d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8352d-114">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8352d-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="8352d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8352d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8352d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8352d-116">Not supported.</span></span> |
| <span data-ttu-id="8352d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8352d-117">Application</span></span>                            | <span data-ttu-id="8352d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8352d-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="8352d-119">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="8352d-119">Permissions acting on other users</span></span>

|<span data-ttu-id="8352d-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="8352d-120">Permission type</span></span>      | <span data-ttu-id="8352d-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8352d-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="8352d-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8352d-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="8352d-123">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8352d-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="8352d-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8352d-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8352d-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="8352d-125">Not supported.</span></span> |
| <span data-ttu-id="8352d-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="8352d-126">Application</span></span>                            | <span data-ttu-id="8352d-127">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8352d-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="8352d-128">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="8352d-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="8352d-129">全局管理员</span><span class="sxs-lookup"><span data-stu-id="8352d-129">Global admin</span></span>
* <span data-ttu-id="8352d-130">全局读取者</span><span class="sxs-lookup"><span data-stu-id="8352d-130">Global reader</span></span>
* <span data-ttu-id="8352d-131">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="8352d-131">Privileged authentication admin</span></span>
* <span data-ttu-id="8352d-132">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="8352d-132">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="8352d-133">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8352d-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/phoneMethods/{id}
GET /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```
<span data-ttu-id="8352d-134">与要 `id` 检索的 phoneType 对应的值是下列值之一：</span><span class="sxs-lookup"><span data-stu-id="8352d-134">The value of `id` corresponding to the phoneType to retrieve is one of the following:</span></span>
+ <span data-ttu-id="8352d-135">`b6332ec1-7057-4abe-9331-3d72feddfe41` 检索 `alternateMobile` **phoneType**。</span><span class="sxs-lookup"><span data-stu-id="8352d-135">`b6332ec1-7057-4abe-9331-3d72feddfe41` to retrieve the `alternateMobile` **phoneType**.</span></span>
+ <span data-ttu-id="8352d-136">`e37fc753-ff3b-4958-9484-eaa9425c82bc` 检索 `office` **phoneType**。</span><span class="sxs-lookup"><span data-stu-id="8352d-136">`e37fc753-ff3b-4958-9484-eaa9425c82bc` to retrieve the `office` **phoneType**.</span></span>
+ <span data-ttu-id="8352d-137">`3179e48a-750b-4051-897c-87b9720928f7` 检索 `mobile` **phoneType**。</span><span class="sxs-lookup"><span data-stu-id="8352d-137">`3179e48a-750b-4051-897c-87b9720928f7` to retrieve the `mobile` **phoneType**.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="8352d-138">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8352d-138">Optional query parameters</span></span>

<span data-ttu-id="8352d-139">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="8352d-139">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8352d-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="8352d-140">Request headers</span></span>

| <span data-ttu-id="8352d-141">名称</span><span class="sxs-lookup"><span data-stu-id="8352d-141">Name</span></span>      |<span data-ttu-id="8352d-142">说明</span><span class="sxs-lookup"><span data-stu-id="8352d-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8352d-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="8352d-143">Authorization</span></span> | <span data-ttu-id="8352d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8352d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8352d-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="8352d-146">Request body</span></span>

<span data-ttu-id="8352d-147">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8352d-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8352d-148">响应</span><span class="sxs-lookup"><span data-stu-id="8352d-148">Response</span></span>

<span data-ttu-id="8352d-149">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8352d-149">If successful, this method returns a `200 OK` response code and the requested [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8352d-150">示例</span><span class="sxs-lookup"><span data-stu-id="8352d-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8352d-151">请求</span><span class="sxs-lookup"><span data-stu-id="8352d-151">Request</span></span>

<span data-ttu-id="8352d-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8352d-152">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8352d-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="8352d-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phoneauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```
# <a name="c"></a>[<span data-ttu-id="8352d-154">C#</span><span class="sxs-lookup"><span data-stu-id="8352d-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8352d-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8352d-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8352d-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8352d-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8352d-157">Java</span><span class="sxs-lookup"><span data-stu-id="8352d-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8352d-158">响应</span><span class="sxs-lookup"><span data-stu-id="8352d-158">Response</span></span>

<span data-ttu-id="8352d-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8352d-159">The following is an example of the response.</span></span>

> <span data-ttu-id="8352d-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8352d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
