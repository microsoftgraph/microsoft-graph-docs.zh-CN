---
title: 获取 emailAuthenticationMethod
description: 读取 emailAuthenticationMethod 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 46189eb8bb465ea0e436e71fa3c9129094d3ece0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436338"
---
# <a name="get-emailauthenticationmethod"></a><span data-ttu-id="6a7aa-103">获取 emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6a7aa-103">Get emailAuthenticationMethod</span></span>
<span data-ttu-id="6a7aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a7aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a7aa-105">检索用户的单个 [电子邮件身份验证方法](../resources/emailauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6a7aa-105">Retrieve a user's single [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a7aa-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6a7aa-106">Permissions</span></span>
<span data-ttu-id="6a7aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a7aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a7aa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a7aa-109">Permission type</span></span>|<span data-ttu-id="6a7aa-110">自操作权限 (权限从最低到最特权) </span><span class="sxs-lookup"><span data-stu-id="6a7aa-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="6a7aa-111">对他人 (权限从最低到最特权) </span><span class="sxs-lookup"><span data-stu-id="6a7aa-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="6a7aa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a7aa-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a7aa-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a7aa-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="6a7aa-114">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a7aa-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="6a7aa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a7aa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a7aa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a7aa-116">Not supported.</span></span> | <span data-ttu-id="6a7aa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a7aa-117">Not supported.</span></span> |
| <span data-ttu-id="6a7aa-118">Application</span><span class="sxs-lookup"><span data-stu-id="6a7aa-118">Application</span></span>                            | <span data-ttu-id="6a7aa-119">不适用。</span><span class="sxs-lookup"><span data-stu-id="6a7aa-119">Not applicable.</span></span> | <span data-ttu-id="6a7aa-120">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a7aa-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="6a7aa-121">对于管理员正在操作其他用户的委派方案，管理员需要以下角色之 [一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="6a7aa-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="6a7aa-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="6a7aa-122">Global admin</span></span>
* <span data-ttu-id="6a7aa-123">全局读取者</span><span class="sxs-lookup"><span data-stu-id="6a7aa-123">Global reader</span></span>
* <span data-ttu-id="6a7aa-124">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="6a7aa-124">Privileged authentication admin</span></span>
* <span data-ttu-id="6a7aa-125">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="6a7aa-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="6a7aa-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a7aa-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/emailMethods/{id}
GET /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6a7aa-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a7aa-127">Request headers</span></span>
|<span data-ttu-id="6a7aa-128">名称</span><span class="sxs-lookup"><span data-stu-id="6a7aa-128">Name</span></span>|<span data-ttu-id="6a7aa-129">说明</span><span class="sxs-lookup"><span data-stu-id="6a7aa-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6a7aa-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a7aa-130">Authorization</span></span>|<span data-ttu-id="6a7aa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6a7aa-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a7aa-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a7aa-133">Request body</span></span>
<span data-ttu-id="6a7aa-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6a7aa-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a7aa-135">响应</span><span class="sxs-lookup"><span data-stu-id="6a7aa-135">Response</span></span>

<span data-ttu-id="6a7aa-136">如果成功，此方法在响应正文中返回响应代码和请求 `200 OK` [的 emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6a7aa-136">If successful, this method returns a `200 OK` response code and the requested [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a7aa-137">示例</span><span class="sxs-lookup"><span data-stu-id="6a7aa-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a7aa-138">请求</span><span class="sxs-lookup"><span data-stu-id="6a7aa-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6a7aa-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a7aa-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```
# <a name="c"></a>[<span data-ttu-id="6a7aa-140">C#</span><span class="sxs-lookup"><span data-stu-id="6a7aa-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a7aa-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a7aa-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a7aa-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a7aa-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6a7aa-143">Java</span><span class="sxs-lookup"><span data-stu-id="6a7aa-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6a7aa-144">响应</span><span class="sxs-lookup"><span data-stu-id="6a7aa-144">Response</span></span>
<span data-ttu-id="6a7aa-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6a7aa-145">The following is an example of the response.</span></span>

<span data-ttu-id="6a7aa-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6a7aa-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": {
      "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
      "emailAddress": "Kim@contoso.com"
  }
}
```

