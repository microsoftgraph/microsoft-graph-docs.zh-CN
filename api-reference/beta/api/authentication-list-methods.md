---
title: List 方法
description: 检索身份验证方法对象的列表。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 48156b4f2c478b5d58978fba837a0f44ed17d502
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515504"
---
# <a name="list-methods"></a><span data-ttu-id="a98df-103">List 方法</span><span class="sxs-lookup"><span data-stu-id="a98df-103">List methods</span></span>

<span data-ttu-id="a98df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a98df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a98df-105">检索身份验证 [方法对象](../resources/authenticationmethod.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="a98df-105">Retrieve a list of [authentication method](../resources/authenticationmethod.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a98df-106">权限</span><span class="sxs-lookup"><span data-stu-id="a98df-106">Permissions</span></span>

<span data-ttu-id="a98df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a98df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="a98df-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="a98df-109">Permissions acting on self</span></span>

|<span data-ttu-id="a98df-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a98df-110">Permission type</span></span>      | <span data-ttu-id="a98df-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a98df-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="a98df-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a98df-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a98df-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a98df-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="a98df-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a98df-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a98df-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a98df-115">Not supported.</span></span> |
| <span data-ttu-id="a98df-116">Application</span><span class="sxs-lookup"><span data-stu-id="a98df-116">Application</span></span>                            | <span data-ttu-id="a98df-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a98df-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="a98df-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="a98df-118">Permissions acting on other users</span></span>

|<span data-ttu-id="a98df-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="a98df-119">Permission type</span></span>      | <span data-ttu-id="a98df-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a98df-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="a98df-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a98df-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="a98df-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a98df-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="a98df-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a98df-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a98df-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="a98df-124">Not supported.</span></span> |
| <span data-ttu-id="a98df-125">Application</span><span class="sxs-lookup"><span data-stu-id="a98df-125">Application</span></span>                            | <span data-ttu-id="a98df-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a98df-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="a98df-127">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="a98df-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="a98df-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="a98df-128">Global admin</span></span>
* <span data-ttu-id="a98df-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="a98df-129">Global reader</span></span>
* <span data-ttu-id="a98df-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="a98df-130">Privileged authentication admin</span></span>
* <span data-ttu-id="a98df-131">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="a98df-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="a98df-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a98df-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods
GET /users/{id | userPrincipalName}/authentication/methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a98df-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a98df-133">Optional query parameters</span></span>

<span data-ttu-id="a98df-134">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="a98df-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a98df-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="a98df-135">Request headers</span></span>

| <span data-ttu-id="a98df-136">名称</span><span class="sxs-lookup"><span data-stu-id="a98df-136">Name</span></span>      |<span data-ttu-id="a98df-137">说明</span><span class="sxs-lookup"><span data-stu-id="a98df-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a98df-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="a98df-138">Authorization</span></span> | <span data-ttu-id="a98df-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a98df-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a98df-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="a98df-141">Request body</span></span>

<span data-ttu-id="a98df-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a98df-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a98df-143">响应</span><span class="sxs-lookup"><span data-stu-id="a98df-143">Response</span></span>

<span data-ttu-id="a98df-144">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [authenticationMethod](../resources/authenticationmethod.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a98df-144">If successful, this method returns a `200 OK` response code and a collection of [authenticationMethod](../resources/authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a98df-145">示例</span><span class="sxs-lookup"><span data-stu-id="a98df-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a98df-146">请求</span><span class="sxs-lookup"><span data-stu-id="a98df-146">Request</span></span>

<span data-ttu-id="a98df-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a98df-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a98df-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="a98df-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_methods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/methods
```
# <a name="c"></a>[<span data-ttu-id="a98df-149">C#</span><span class="sxs-lookup"><span data-stu-id="a98df-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-methods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a98df-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a98df-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-methods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a98df-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a98df-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-methods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a98df-152">Java</span><span class="sxs-lookup"><span data-stu-id="a98df-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-methods-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a98df-153">响应</span><span class="sxs-lookup"><span data-stu-id="a98df-153">Response</span></span>

<span data-ttu-id="a98df-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a98df-154">The following is an example of the response.</span></span>

> <span data-ttu-id="a98df-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a98df-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
