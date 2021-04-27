---
title: 获取 temporaryAccessPassAuthenticationMethod
description: 读取 temporaryAccessPassAuthenticationMethod 对象的属性和关系。
author: inbarckMS
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ccaa0d574c2fb2261c8cb0e0e0091473ec389f1f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049672"
---
# <a name="get-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="ccd6c-103">获取 temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ccd6c-103">Get temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="ccd6c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccd6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccd6c-105">检索用户的单个  [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ccd6c-105">Retrieve a user's single  [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccd6c-106">权限</span><span class="sxs-lookup"><span data-stu-id="ccd6c-106">Permissions</span></span>
<span data-ttu-id="ccd6c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ccd6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="ccd6c-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="ccd6c-109">Permissions acting on self</span></span>

|<span data-ttu-id="ccd6c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ccd6c-110">Permission type</span></span>      | <span data-ttu-id="ccd6c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ccd6c-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="ccd6c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ccd6c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ccd6c-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ccd6c-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="ccd6c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ccd6c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccd6c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccd6c-115">Not supported.</span></span> |
| <span data-ttu-id="ccd6c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ccd6c-116">Application</span></span>                            | <span data-ttu-id="ccd6c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccd6c-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="ccd6c-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="ccd6c-118">Permissions acting on other users</span></span>

|<span data-ttu-id="ccd6c-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="ccd6c-119">Permission type</span></span>      | <span data-ttu-id="ccd6c-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ccd6c-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="ccd6c-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ccd6c-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="ccd6c-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccd6c-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="ccd6c-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ccd6c-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccd6c-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccd6c-124">Not supported.</span></span> |
| <span data-ttu-id="ccd6c-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="ccd6c-125">Application</span></span>                            | <span data-ttu-id="ccd6c-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccd6c-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="ccd6c-127">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="ccd6c-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="ccd6c-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="ccd6c-128">Global admin</span></span>
* <span data-ttu-id="ccd6c-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="ccd6c-129">Global reader</span></span>
* <span data-ttu-id="ccd6c-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="ccd6c-130">Privileged authentication admin</span></span>
* <span data-ttu-id="ccd6c-131">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="ccd6c-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="ccd6c-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ccd6c-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/temporaryAccessPassMethods/{temporaryAccessPassAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods/{temporaryAccessPassAuthenticationMethodId}
```


## <a name="request-headers"></a><span data-ttu-id="ccd6c-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="ccd6c-133">Request headers</span></span>
|<span data-ttu-id="ccd6c-134">名称</span><span class="sxs-lookup"><span data-stu-id="ccd6c-134">Name</span></span>|<span data-ttu-id="ccd6c-135">说明</span><span class="sxs-lookup"><span data-stu-id="ccd6c-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ccd6c-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccd6c-136">Authorization</span></span>|<span data-ttu-id="ccd6c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ccd6c-p102">Bearer {token}. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="ccd6c-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="ccd6c-139">Request body</span></span>
<span data-ttu-id="ccd6c-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ccd6c-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccd6c-141">响应</span><span class="sxs-lookup"><span data-stu-id="ccd6c-141">Response</span></span>

<span data-ttu-id="ccd6c-142">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ccd6c-142">If successful, this method returns a `200 OK` response code and a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ccd6c-143">示例</span><span class="sxs-lookup"><span data-stu-id="ccd6c-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ccd6c-144">请求</span><span class="sxs-lookup"><span data-stu-id="ccd6c-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ccd6c-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccd6c-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_temporaryaccesspassauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods/30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30
```
# <a name="c"></a>[<span data-ttu-id="ccd6c-146">C#</span><span class="sxs-lookup"><span data-stu-id="ccd6c-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-temporaryaccesspassauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccd6c-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccd6c-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-temporaryaccesspassauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccd6c-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccd6c-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-temporaryaccesspassauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ccd6c-149">Java</span><span class="sxs-lookup"><span data-stu-id="ccd6c-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-temporaryaccesspassauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ccd6c-150">响应</span><span class="sxs-lookup"><span data-stu-id="ccd6c-150">Response</span></span>
<span data-ttu-id="ccd6c-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ccd6c-151">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
    "id": "30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30",
    "temporaryAccessPass": null,
    "createdDateTime": "String (timestamp)",
    "startDateTime": "String (timestamp)",
    "lifetimeInMinutes": "Integer",
    "isUsableOnce": "Boolean",
    "isUsable": "Boolean",
    "methodUsabilityReason": "String"
  }
}
```
