---
title: 列出 emailAuthenticationMethods
description: 获取 emailAuthenticationMethod 对象及其属性的列表。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bc1ef69b988c0e0aab2921b63fe0a08b545649f4
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49871986"
---
# <a name="list-emailauthenticationmethods"></a><span data-ttu-id="3ec4e-103">列出 emailAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="3ec4e-103">List emailAuthenticationMethods</span></span>
<span data-ttu-id="3ec4e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ec4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ec4e-105">检索用户的电子邮件 [身份验证方法对象](../resources/emailauthenticationmethod.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="3ec4e-105">Retrieve a list of a user's [email Authentication Method](../resources/emailauthenticationmethod.md) objects and their properties.</span></span> <span data-ttu-id="3ec4e-106">此调用将仅返回单个对象，因为只能为用户设置一种电子邮件方法。</span><span class="sxs-lookup"><span data-stu-id="3ec4e-106">This call will only return a single object as only one email method can be set on users.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ec4e-107">权限</span><span class="sxs-lookup"><span data-stu-id="3ec4e-107">Permissions</span></span>
<span data-ttu-id="3ec4e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ec4e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ec4e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ec4e-110">Permission type</span></span>|<span data-ttu-id="3ec4e-111">对自身执行 (权限从最低特权到最多特权) </span><span class="sxs-lookup"><span data-stu-id="3ec4e-111">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="3ec4e-112">对他人的操作权限 (权限从最低特权级别) </span><span class="sxs-lookup"><span data-stu-id="3ec4e-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="3ec4e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ec4e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ec4e-114">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ec4e-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="3ec4e-115">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec4e-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="3ec4e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ec4e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ec4e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ec4e-117">Not supported.</span></span> | <span data-ttu-id="3ec4e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ec4e-118">Not supported.</span></span> |
| <span data-ttu-id="3ec4e-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ec4e-119">Application</span></span>                            | <span data-ttu-id="3ec4e-120">不适用。</span><span class="sxs-lookup"><span data-stu-id="3ec4e-120">Not applicable.</span></span> | <span data-ttu-id="3ec4e-121">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec4e-121">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="3ec4e-122">对于管理员正在操作其他用户的委派方案，管理员需要以下角色之 [一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="3ec4e-122">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="3ec4e-123">全局管理员</span><span class="sxs-lookup"><span data-stu-id="3ec4e-123">Global admin</span></span>
* <span data-ttu-id="3ec4e-124">全局读取者</span><span class="sxs-lookup"><span data-stu-id="3ec4e-124">Global reader</span></span>
* <span data-ttu-id="3ec4e-125">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="3ec4e-125">Privileged authentication admin</span></span>
* <span data-ttu-id="3ec4e-126">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="3ec4e-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="3ec4e-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ec4e-127">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/emailMethods
GET /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3ec4e-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3ec4e-128">Optional query parameters</span></span>
<span data-ttu-id="3ec4e-129">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="3ec4e-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ec4e-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ec4e-130">Request headers</span></span>
|<span data-ttu-id="3ec4e-131">名称</span><span class="sxs-lookup"><span data-stu-id="3ec4e-131">Name</span></span>|<span data-ttu-id="3ec4e-132">说明</span><span class="sxs-lookup"><span data-stu-id="3ec4e-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3ec4e-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ec4e-133">Authorization</span></span>|<span data-ttu-id="3ec4e-134">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="3ec4e-134">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ec4e-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ec4e-135">Request body</span></span>
<span data-ttu-id="3ec4e-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3ec4e-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ec4e-137">响应</span><span class="sxs-lookup"><span data-stu-id="3ec4e-137">Response</span></span>

<span data-ttu-id="3ec4e-138">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3ec4e-138">If successful, this method returns a `200 OK` response code and a collection of [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3ec4e-139">示例</span><span class="sxs-lookup"><span data-stu-id="3ec4e-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3ec4e-140">请求</span><span class="sxs-lookup"><span data-stu-id="3ec4e-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3ec4e-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ec4e-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/emailMethods
```
# <a name="c"></a>[<span data-ttu-id="3ec4e-142">C#</span><span class="sxs-lookup"><span data-stu-id="3ec4e-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ec4e-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ec4e-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ec4e-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ec4e-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ec4e-145">Java</span><span class="sxs-lookup"><span data-stu-id="3ec4e-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="3ec4e-146">响应</span><span class="sxs-lookup"><span data-stu-id="3ec4e-146">Response</span></span>
<span data-ttu-id="3ec4e-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3ec4e-147">The following is an example of the response.</span></span>

<span data-ttu-id="3ec4e-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3ec4e-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.emailAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": [
    {
      "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
      "emailAddress": "Kim@contoso.com"
    }
  ]
}
```

