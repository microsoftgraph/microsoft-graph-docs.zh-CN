---
title: 更新 emailAuthenticationMethod
description: 更新 emailAuthenticationMethod 对象的属性。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3e1509426af1d967c1fa6e6ed9ec7999a50afb04
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796427"
---
# <a name="update-emailauthenticationmethod"></a><span data-ttu-id="9707d-103">更新 emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9707d-103">Update emailAuthenticationMethod</span></span>
<span data-ttu-id="9707d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9707d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9707d-105">更新与电子邮件身份验证方法对象关联的 [用户](../resources/emailauthenticationmethod.md) 的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="9707d-105">Update a user's email address associated with an [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9707d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9707d-106">Permissions</span></span>
<span data-ttu-id="9707d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9707d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9707d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9707d-109">Permission type</span></span>|<span data-ttu-id="9707d-110">对自身执行 (权限从最多到最低特权) </span><span class="sxs-lookup"><span data-stu-id="9707d-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="9707d-111">对他人操作的权限 (权限从最低特权到最多特权) </span><span class="sxs-lookup"><span data-stu-id="9707d-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="9707d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9707d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9707d-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9707d-113">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="9707d-114">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9707d-114">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="9707d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9707d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9707d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9707d-116">Not supported.</span></span> | <span data-ttu-id="9707d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9707d-117">Not supported.</span></span> |
| <span data-ttu-id="9707d-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="9707d-118">Application</span></span>                            | <span data-ttu-id="9707d-119">不适用</span><span class="sxs-lookup"><span data-stu-id="9707d-119">Not applicable.</span></span> | <span data-ttu-id="9707d-120">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9707d-120">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="9707d-121">对于管理员正在操作其他用户的委派方案，管理员需要以下角色之 [一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="9707d-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="9707d-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="9707d-122">Global admin</span></span>
* <span data-ttu-id="9707d-123">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="9707d-123">Privileged authentication admin</span></span>
* <span data-ttu-id="9707d-124">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="9707d-124">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="9707d-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9707d-125">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9707d-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="9707d-126">Request headers</span></span>
|<span data-ttu-id="9707d-127">名称</span><span class="sxs-lookup"><span data-stu-id="9707d-127">Name</span></span>|<span data-ttu-id="9707d-128">说明</span><span class="sxs-lookup"><span data-stu-id="9707d-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9707d-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="9707d-129">Authorization</span></span>|<span data-ttu-id="9707d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9707d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9707d-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9707d-132">Content-Type</span></span>|<span data-ttu-id="9707d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9707d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9707d-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="9707d-135">Request body</span></span>
<span data-ttu-id="9707d-136">在请求正文中，提供 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 对象的 JSON 表示形式和更新的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="9707d-136">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the updated email address.</span></span>

<span data-ttu-id="9707d-137">下表显示更新 [emailAuthenticationMethod 时所需的属性](../resources/emailauthenticationmethod.md)。</span><span class="sxs-lookup"><span data-stu-id="9707d-137">The following table shows the properties that are required when you update the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="9707d-138">属性</span><span class="sxs-lookup"><span data-stu-id="9707d-138">Property</span></span>|<span data-ttu-id="9707d-139">类型</span><span class="sxs-lookup"><span data-stu-id="9707d-139">Type</span></span>|<span data-ttu-id="9707d-140">说明</span><span class="sxs-lookup"><span data-stu-id="9707d-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9707d-141">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9707d-141">emailAddress</span></span>|<span data-ttu-id="9707d-142">String</span><span class="sxs-lookup"><span data-stu-id="9707d-142">String</span></span>|<span data-ttu-id="9707d-143">更新的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="9707d-143">Updated email address</span></span>|



## <a name="response"></a><span data-ttu-id="9707d-144">响应</span><span class="sxs-lookup"><span data-stu-id="9707d-144">Response</span></span>

<span data-ttu-id="9707d-145">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9707d-145">If successful, this method returns a `200 OK` response code and an updated [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9707d-146">示例</span><span class="sxs-lookup"><span data-stu-id="9707d-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9707d-147">请求</span><span class="sxs-lookup"><span data-stu-id="9707d-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9707d-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="9707d-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_emailauthenticationmethod"
}
-->
``` http
PUT https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
Content-Type: application/json

{
  "emailAddress": "kim@contoso.com"
}
```
# <a name="javascript"></a>[<span data-ttu-id="9707d-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9707d-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9707d-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9707d-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="9707d-151">C#</span><span class="sxs-lookup"><span data-stu-id="9707d-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9707d-152">Java</span><span class="sxs-lookup"><span data-stu-id="9707d-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9707d-153">响应</span><span class="sxs-lookup"><span data-stu-id="9707d-153">Response</span></span>

<span data-ttu-id="9707d-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9707d-154">The following is an example of the response.</span></span>

<span data-ttu-id="9707d-155">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9707d-155">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAuthenticationMethod"
} -->

``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
  "emailAddress": "kim@contoso.com"
}
```
