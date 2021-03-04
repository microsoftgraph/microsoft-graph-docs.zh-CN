---
title: 获取 microsoftAuthenticatorAuthenticationMethod
description: 读取 microsoftAuthenticatorAuthenticationMethod 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 08f670abf0131b43fda3a0d191baff0549ee4735
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442406"
---
# <a name="get-microsoftauthenticatorauthenticationmethod"></a><span data-ttu-id="b9e65-103">获取 microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b9e65-103">Get microsoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="b9e65-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9e65-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9e65-105">读取 [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b9e65-105">Read the properties and relationships of a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9e65-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b9e65-106">Permissions</span></span>

<span data-ttu-id="b9e65-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9e65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="b9e65-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="b9e65-109">Permissions acting on self</span></span>

|<span data-ttu-id="b9e65-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9e65-110">Permission type</span></span>      | <span data-ttu-id="b9e65-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9e65-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="b9e65-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e65-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9e65-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9e65-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="b9e65-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e65-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9e65-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9e65-115">Not supported.</span></span> |
| <span data-ttu-id="b9e65-116">Application</span><span class="sxs-lookup"><span data-stu-id="b9e65-116">Application</span></span>                            | <span data-ttu-id="b9e65-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9e65-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="b9e65-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="b9e65-118">Permissions acting on other users</span></span>

|<span data-ttu-id="b9e65-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9e65-119">Permission type</span></span>      | <span data-ttu-id="b9e65-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9e65-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="b9e65-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e65-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9e65-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9e65-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="b9e65-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e65-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9e65-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9e65-124">Not supported.</span></span> |
| <span data-ttu-id="b9e65-125">Application</span><span class="sxs-lookup"><span data-stu-id="b9e65-125">Application</span></span>                            | <span data-ttu-id="b9e65-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9e65-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="b9e65-127">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="b9e65-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="b9e65-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="b9e65-128">Global admin</span></span>
* <span data-ttu-id="b9e65-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="b9e65-129">Global reader</span></span>
* <span data-ttu-id="b9e65-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="b9e65-130">Privileged authentication admin</span></span>
* <span data-ttu-id="b9e65-131">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="b9e65-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="b9e65-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9e65-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9e65-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b9e65-133">Optional query parameters</span></span>
<span data-ttu-id="b9e65-134">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b9e65-134">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b9e65-135">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b9e65-135">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9e65-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9e65-136">Request headers</span></span>
|<span data-ttu-id="b9e65-137">名称</span><span class="sxs-lookup"><span data-stu-id="b9e65-137">Name</span></span>|<span data-ttu-id="b9e65-138">说明</span><span class="sxs-lookup"><span data-stu-id="b9e65-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b9e65-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9e65-139">Authorization</span></span>|<span data-ttu-id="b9e65-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9e65-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9e65-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9e65-142">Request body</span></span>
<span data-ttu-id="b9e65-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b9e65-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9e65-144">响应</span><span class="sxs-lookup"><span data-stu-id="b9e65-144">Response</span></span>

<span data-ttu-id="b9e65-145">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9e65-145">If successful, this method returns a `200 OK` response code and a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9e65-146">示例</span><span class="sxs-lookup"><span data-stu-id="b9e65-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b9e65-147">请求</span><span class="sxs-lookup"><span data-stu-id="b9e65-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b9e65-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9e65-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/anirban@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="b9e65-149">C#</span><span class="sxs-lookup"><span data-stu-id="b9e65-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-microsoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9e65-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9e65-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-microsoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9e65-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9e65-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-microsoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9e65-152">Java</span><span class="sxs-lookup"><span data-stu-id="b9e65-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-microsoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b9e65-153">响应</span><span class="sxs-lookup"><span data-stu-id="b9e65-153">Response</span></span>
<span data-ttu-id="b9e65-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b9e65-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
    "id": "6803c096-c096-6803-96c0-036896c00368",
    "displayName": "Sandeep's iPhone",
    "deviceTag": "",
    "phoneAppVersion": "6.5.4",
    "createdDateTime": "2020-12-03T23:16:12Z"
  }
}
```
