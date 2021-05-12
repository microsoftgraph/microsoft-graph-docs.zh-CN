---
title: 列出 microsoftAuthenticatorAuthenticationMethods
description: 获取 microsoftAuthenticatorAuthenticationMethod 对象及其属性的列表。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7278ae26e137e3a71988fb7ce388c3c4304bfdd3
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335651"
---
# <a name="list-microsoftauthenticatorauthenticationmethods"></a><span data-ttu-id="3c1e9-103">列出 microsoftAuthenticatorAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="3c1e9-103">List microsoftAuthenticatorAuthenticationMethods</span></span>
<span data-ttu-id="3c1e9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c1e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c1e9-105">获取 [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="3c1e9-105">Get a list of the [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c1e9-106">权限</span><span class="sxs-lookup"><span data-stu-id="3c1e9-106">Permissions</span></span>

<span data-ttu-id="3c1e9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c1e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="3c1e9-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="3c1e9-109">Permissions acting on self</span></span>

|<span data-ttu-id="3c1e9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c1e9-110">Permission type</span></span>      | <span data-ttu-id="3c1e9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c1e9-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="3c1e9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c1e9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c1e9-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c1e9-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="3c1e9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c1e9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c1e9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c1e9-115">Not supported.</span></span> |
| <span data-ttu-id="3c1e9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c1e9-116">Application</span></span>                            | <span data-ttu-id="3c1e9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c1e9-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="3c1e9-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="3c1e9-118">Permissions acting on other users</span></span>

|<span data-ttu-id="3c1e9-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c1e9-119">Permission type</span></span>      | <span data-ttu-id="3c1e9-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c1e9-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="3c1e9-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c1e9-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c1e9-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c1e9-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="3c1e9-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c1e9-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c1e9-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c1e9-124">Not supported.</span></span> |
| <span data-ttu-id="3c1e9-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c1e9-125">Application</span></span>                            | <span data-ttu-id="3c1e9-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c1e9-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="3c1e9-127">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="3c1e9-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="3c1e9-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="3c1e9-128">Global admin</span></span>
* <span data-ttu-id="3c1e9-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="3c1e9-129">Global reader</span></span>
* <span data-ttu-id="3c1e9-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="3c1e9-130">Privileged authentication admin</span></span>
* <span data-ttu-id="3c1e9-131">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="3c1e9-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="3c1e9-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c1e9-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/microsoftAuthenticatorMethods
GET /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c1e9-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3c1e9-133">Optional query parameters</span></span>

<span data-ttu-id="3c1e9-134">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c1e9-134">Not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c1e9-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c1e9-135">Request headers</span></span>

|<span data-ttu-id="3c1e9-136">名称</span><span class="sxs-lookup"><span data-stu-id="3c1e9-136">Name</span></span>|<span data-ttu-id="3c1e9-137">说明</span><span class="sxs-lookup"><span data-stu-id="3c1e9-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3c1e9-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c1e9-138">Authorization</span></span>|<span data-ttu-id="3c1e9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c1e9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c1e9-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c1e9-141">Request body</span></span>

<span data-ttu-id="3c1e9-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3c1e9-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c1e9-143">响应</span><span class="sxs-lookup"><span data-stu-id="3c1e9-143">Response</span></span>

<span data-ttu-id="3c1e9-144">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3c1e9-144">If successful, this method returns a `200 OK` response code and a collection of [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c1e9-145">示例</span><span class="sxs-lookup"><span data-stu-id="3c1e9-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3c1e9-146">请求</span><span class="sxs-lookup"><span data-stu-id="3c1e9-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3c1e9-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c1e9-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/anirban@contoso.com/authentication/microsoftAuthenticatorMethods
```
# <a name="c"></a>[<span data-ttu-id="3c1e9-148">C#</span><span class="sxs-lookup"><span data-stu-id="3c1e9-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-microsoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c1e9-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c1e9-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-microsoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c1e9-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c1e9-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-microsoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c1e9-151">Java</span><span class="sxs-lookup"><span data-stu-id="3c1e9-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-microsoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="3c1e9-152">响应</span><span class="sxs-lookup"><span data-stu-id="3c1e9-152">Response</span></span>
<span data-ttu-id="3c1e9-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3c1e9-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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

