---
title: 创建 emailAuthenticationMethod
description: 创建新的 emailAuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b9ec2d40253faa72fd1f8d354de2649c4487e47e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436322"
---
# <a name="create-emailauthenticationmethod"></a><span data-ttu-id="d9ea7-103">创建 emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d9ea7-103">Create emailAuthenticationMethod</span></span>
<span data-ttu-id="d9ea7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9ea7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9ea7-105">设置用户 [的电子邮件AuthenticationMethod](../resources/emailauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9ea7-105">Set a user's [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object.</span></span> <span data-ttu-id="d9ea7-106">电子邮件身份验证是一种自助服务密码重置方法。</span><span class="sxs-lookup"><span data-stu-id="d9ea7-106">Email authentication is a self-service password reset method.</span></span> <span data-ttu-id="d9ea7-107">用户可能只有一种电子邮件身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="d9ea7-107">A user may only have one email authentication method.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9ea7-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="d9ea7-108">Permissions</span></span>
<span data-ttu-id="d9ea7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9ea7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9ea7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9ea7-111">Permission type</span></span>|<span data-ttu-id="d9ea7-112">自操作权限 (权限从最低到最特权) </span><span class="sxs-lookup"><span data-stu-id="d9ea7-112">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="d9ea7-113">对他人 (权限从最低到最特权) </span><span class="sxs-lookup"><span data-stu-id="d9ea7-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="d9ea7-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9ea7-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9ea7-115">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9ea7-115">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="d9ea7-116">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9ea7-116">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="d9ea7-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9ea7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9ea7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9ea7-118">Not supported.</span></span> | <span data-ttu-id="d9ea7-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9ea7-119">Not supported.</span></span> |
| <span data-ttu-id="d9ea7-120">Application</span><span class="sxs-lookup"><span data-stu-id="d9ea7-120">Application</span></span>                            | <span data-ttu-id="d9ea7-121">不适用。</span><span class="sxs-lookup"><span data-stu-id="d9ea7-121">Not applicable.</span></span> | <span data-ttu-id="d9ea7-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9ea7-122">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="d9ea7-123">对于管理员正在操作其他用户的委派方案，管理员需要以下角色之 [一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="d9ea7-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="d9ea7-124">全局管理员</span><span class="sxs-lookup"><span data-stu-id="d9ea7-124">Global admin</span></span>
* <span data-ttu-id="d9ea7-125">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="d9ea7-125">Privileged authentication admin</span></span>
* <span data-ttu-id="d9ea7-126">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="d9ea7-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="d9ea7-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9ea7-127">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="request-headers"></a><span data-ttu-id="d9ea7-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9ea7-128">Request headers</span></span>
|<span data-ttu-id="d9ea7-129">名称</span><span class="sxs-lookup"><span data-stu-id="d9ea7-129">Name</span></span>|<span data-ttu-id="d9ea7-130">说明</span><span class="sxs-lookup"><span data-stu-id="d9ea7-130">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d9ea7-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9ea7-131">Authorization</span></span>|<span data-ttu-id="d9ea7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d9ea7-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d9ea7-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9ea7-134">Content-Type</span></span>|<span data-ttu-id="d9ea7-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9ea7-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9ea7-137">Request body</span></span>
<span data-ttu-id="d9ea7-138">在请求正文中，提供 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 对象的 JSON 表示形式以及所需的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="d9ea7-138">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the desired email address.</span></span>

<span data-ttu-id="d9ea7-139">下表显示创建 [emailAuthenticationMethod 时所需的属性](../resources/emailauthenticationmethod.md)。</span><span class="sxs-lookup"><span data-stu-id="d9ea7-139">The following table shows the properties that are required when you create the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="d9ea7-140">属性</span><span class="sxs-lookup"><span data-stu-id="d9ea7-140">Property</span></span>|<span data-ttu-id="d9ea7-141">类型</span><span class="sxs-lookup"><span data-stu-id="d9ea7-141">Type</span></span>|<span data-ttu-id="d9ea7-142">说明</span><span class="sxs-lookup"><span data-stu-id="d9ea7-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9ea7-143">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d9ea7-143">emailAddress</span></span>|<span data-ttu-id="d9ea7-144">String</span><span class="sxs-lookup"><span data-stu-id="d9ea7-144">String</span></span>|<span data-ttu-id="d9ea7-145">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="d9ea7-145">Email address</span></span>|



## <a name="response"></a><span data-ttu-id="d9ea7-146">响应</span><span class="sxs-lookup"><span data-stu-id="d9ea7-146">Response</span></span>

<span data-ttu-id="d9ea7-147">如果成功，此方法在响应正文中返回响应代码和 `201 Created` 新的 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9ea7-147">If successful, this method returns a `201 Created` response code and a new [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9ea7-148">示例</span><span class="sxs-lookup"><span data-stu-id="d9ea7-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9ea7-149">请求</span><span class="sxs-lookup"><span data-stu-id="d9ea7-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d9ea7-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9ea7-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_emailauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods
Content-Type: application/json

{
  "emailAddress": "kim@contoso.com"
}
```
# <a name="javascript"></a>[<span data-ttu-id="d9ea7-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9ea7-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9ea7-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9ea7-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="d9ea7-153">C#</span><span class="sxs-lookup"><span data-stu-id="d9ea7-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-emailauthenticationmethod-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9ea7-154">Java</span><span class="sxs-lookup"><span data-stu-id="d9ea7-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-emailauthenticationmethod-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d9ea7-155">响应</span><span class="sxs-lookup"><span data-stu-id="d9ea7-155">Response</span></span>
<span data-ttu-id="d9ea7-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d9ea7-156">The following is an example of the response.</span></span>

<span data-ttu-id="d9ea7-157">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d9ea7-157">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
  "emailAddress": "kim@contoso.com"
}
```
