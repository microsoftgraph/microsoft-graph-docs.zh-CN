---
title: 列出 microsoftAuthenticatorAuthenticationMethods
description: 获取 microsoftAuthenticatorAuthenticationMethod 对象及其属性的列表。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c23c72d9ee7addfd48f762a718731874ce450231
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469183"
---
# <a name="list-microsoftauthenticatorauthenticationmethods"></a><span data-ttu-id="82765-103">列出 microsoftAuthenticatorAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="82765-103">List microsoftAuthenticatorAuthenticationMethods</span></span>
<span data-ttu-id="82765-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82765-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="82765-105">获取 [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="82765-105">Get a list of the [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="82765-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="82765-106">Permissions</span></span>

<span data-ttu-id="82765-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82765-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="82765-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="82765-109">Permissions acting on self</span></span>

|<span data-ttu-id="82765-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="82765-110">Permission type</span></span>      | <span data-ttu-id="82765-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82765-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="82765-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82765-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="82765-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82765-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="82765-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82765-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82765-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="82765-115">Not supported.</span></span> |
| <span data-ttu-id="82765-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="82765-116">Application</span></span>                            | <span data-ttu-id="82765-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="82765-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="82765-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="82765-118">Permissions acting on other users</span></span>

|<span data-ttu-id="82765-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="82765-119">Permission type</span></span>      | <span data-ttu-id="82765-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82765-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="82765-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82765-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="82765-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82765-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="82765-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82765-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82765-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="82765-124">Not supported.</span></span> |
| <span data-ttu-id="82765-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="82765-125">Application</span></span>                            | <span data-ttu-id="82765-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82765-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="82765-127">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="82765-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="82765-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="82765-128">Global admin</span></span>
* <span data-ttu-id="82765-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="82765-129">Global reader</span></span>
* <span data-ttu-id="82765-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="82765-130">Privileged authentication admin</span></span>
* <span data-ttu-id="82765-131">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="82765-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="82765-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82765-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/microsoftAuthenticatorMethods
GET /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="82765-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="82765-133">Optional query parameters</span></span>

<span data-ttu-id="82765-134">不支持。</span><span class="sxs-lookup"><span data-stu-id="82765-134">Not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="82765-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="82765-135">Request headers</span></span>

|<span data-ttu-id="82765-136">名称</span><span class="sxs-lookup"><span data-stu-id="82765-136">Name</span></span>|<span data-ttu-id="82765-137">说明</span><span class="sxs-lookup"><span data-stu-id="82765-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="82765-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="82765-138">Authorization</span></span>|<span data-ttu-id="82765-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="82765-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="82765-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="82765-141">Request body</span></span>

<span data-ttu-id="82765-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="82765-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82765-143">响应</span><span class="sxs-lookup"><span data-stu-id="82765-143">Response</span></span>

<span data-ttu-id="82765-144">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="82765-144">If successful, this method returns a `200 OK` response code and a collection of [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="82765-145">示例</span><span class="sxs-lookup"><span data-stu-id="82765-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="82765-146">请求</span><span class="sxs-lookup"><span data-stu-id="82765-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="82765-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="82765-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/users/sandeep@contoso.com/authentication/microsoftAuthenticatorMethods
```
# <a name="c"></a>[<span data-ttu-id="82765-148">C#</span><span class="sxs-lookup"><span data-stu-id="82765-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-microsoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82765-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82765-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-microsoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82765-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82765-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-microsoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="82765-151">Java</span><span class="sxs-lookup"><span data-stu-id="82765-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-microsoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="82765-152">响应</span><span class="sxs-lookup"><span data-stu-id="82765-152">Response</span></span>
<span data-ttu-id="82765-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="82765-153">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.microsoftAuthenticatorAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
      "id": "6803c096-c096-6803-96c0-036896c00368",
      "displayName": "Sandeep's iPhone",
      "deviceTag": "",
      "phoneAppVersion": "6.5.4",
      "createdDateTime": "2020-12-03T23:16:12Z"
    }
  ]
}
```

