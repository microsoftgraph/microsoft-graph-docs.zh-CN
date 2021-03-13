---
title: 获取 temporaryAccessPassAuthenticationMethod
description: 读取 temporaryAccessPassAuthenticationMethod 对象的属性和关系。
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6567ee2f287f33837f5e3354c327b1c5b8c16f20
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761498"
---
# <a name="get-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="b9e03-103">获取 temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b9e03-103">Get temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="b9e03-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9e03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9e03-105">检索用户的单个  [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9e03-105">Retrieve a user's single  [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9e03-106">权限</span><span class="sxs-lookup"><span data-stu-id="b9e03-106">Permissions</span></span>
<span data-ttu-id="b9e03-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9e03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="b9e03-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="b9e03-109">Permissions acting on self</span></span>

|<span data-ttu-id="b9e03-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9e03-110">Permission type</span></span>      | <span data-ttu-id="b9e03-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9e03-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="b9e03-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e03-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9e03-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9e03-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="b9e03-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e03-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9e03-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9e03-115">Not supported.</span></span> |
| <span data-ttu-id="b9e03-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9e03-116">Application</span></span>                            | <span data-ttu-id="b9e03-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9e03-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="b9e03-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="b9e03-118">Permissions acting on other users</span></span>

|<span data-ttu-id="b9e03-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9e03-119">Permission type</span></span>      | <span data-ttu-id="b9e03-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9e03-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="b9e03-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e03-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9e03-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9e03-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="b9e03-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e03-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9e03-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9e03-124">Not supported.</span></span> |
| <span data-ttu-id="b9e03-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9e03-125">Application</span></span>                            | <span data-ttu-id="b9e03-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9e03-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="b9e03-127">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="b9e03-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="b9e03-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="b9e03-128">Global admin</span></span>
* <span data-ttu-id="b9e03-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="b9e03-129">Global reader</span></span>
* <span data-ttu-id="b9e03-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="b9e03-130">Privileged authentication admin</span></span>
* <span data-ttu-id="b9e03-131">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="b9e03-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="b9e03-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9e03-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/temporaryAccessPassMethods/{temporaryAccessPassAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods/{temporaryAccessPassAuthenticationMethodId}
```


## <a name="request-headers"></a><span data-ttu-id="b9e03-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9e03-133">Request headers</span></span>
|<span data-ttu-id="b9e03-134">名称</span><span class="sxs-lookup"><span data-stu-id="b9e03-134">Name</span></span>|<span data-ttu-id="b9e03-135">说明</span><span class="sxs-lookup"><span data-stu-id="b9e03-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b9e03-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9e03-136">Authorization</span></span>|<span data-ttu-id="b9e03-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9e03-p102">Bearer {token}. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="b9e03-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9e03-139">Request body</span></span>
<span data-ttu-id="b9e03-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b9e03-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9e03-141">响应</span><span class="sxs-lookup"><span data-stu-id="b9e03-141">Response</span></span>

<span data-ttu-id="b9e03-142">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9e03-142">If successful, this method returns a `200 OK` response code and a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9e03-143">示例</span><span class="sxs-lookup"><span data-stu-id="b9e03-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b9e03-144">请求</span><span class="sxs-lookup"><span data-stu-id="b9e03-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b9e03-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9e03-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_temporaryaccesspassauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods/30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30
```
# <a name="c"></a>[<span data-ttu-id="b9e03-146">C#</span><span class="sxs-lookup"><span data-stu-id="b9e03-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-temporaryaccesspassauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9e03-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9e03-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-temporaryaccesspassauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9e03-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9e03-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-temporaryaccesspassauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9e03-149">Java</span><span class="sxs-lookup"><span data-stu-id="b9e03-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-temporaryaccesspassauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b9e03-150">响应</span><span class="sxs-lookup"><span data-stu-id="b9e03-150">Response</span></span>
<span data-ttu-id="b9e03-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b9e03-151">**Note:** The response object shown here might be shortened for readability.</span></span>
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
