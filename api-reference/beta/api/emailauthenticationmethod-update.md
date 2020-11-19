---
title: 更新 emailAuthenticationMethod
description: 更新 emailAuthenticationMethod 对象的属性。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e1927a9ea081dee5bfe72aad7715a6434f219d79
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352161"
---
# <a name="update-emailauthenticationmethod"></a><span data-ttu-id="631fa-103">更新 emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="631fa-103">Update emailAuthenticationMethod</span></span>
<span data-ttu-id="631fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="631fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="631fa-105">更新与 [电子邮件身份验证方法](../resources/emailauthenticationmethod.md) 对象关联的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="631fa-105">Update a user's email address associated with an [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="631fa-106">权限</span><span class="sxs-lookup"><span data-stu-id="631fa-106">Permissions</span></span>
<span data-ttu-id="631fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="631fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="631fa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="631fa-109">Permission type</span></span>|<span data-ttu-id="631fa-110">从最高特权到最少特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="631fa-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="631fa-111">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="631fa-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="631fa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="631fa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="631fa-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="631fa-113">Not supported.</span></span>|<span data-ttu-id="631fa-114">UserAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="631fa-114">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="631fa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="631fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="631fa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="631fa-116">Not supported.</span></span>|<span data-ttu-id="631fa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="631fa-117">Not supported.</span></span>
|<span data-ttu-id="631fa-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="631fa-118">Application</span></span>|<span data-ttu-id="631fa-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="631fa-119">Not supported.</span></span>|<span data-ttu-id="631fa-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="631fa-120">Not supported.</span></span>

<span data-ttu-id="631fa-121">对于在其他用户上执行管理的委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="631fa-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="631fa-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="631fa-122">Global admin</span></span>
* <span data-ttu-id="631fa-123">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="631fa-123">Privileged authentication admin</span></span>
* <span data-ttu-id="631fa-124">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="631fa-124">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="631fa-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="631fa-125">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="631fa-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="631fa-126">Request headers</span></span>
|<span data-ttu-id="631fa-127">名称</span><span class="sxs-lookup"><span data-stu-id="631fa-127">Name</span></span>|<span data-ttu-id="631fa-128">说明</span><span class="sxs-lookup"><span data-stu-id="631fa-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="631fa-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="631fa-129">Authorization</span></span>|<span data-ttu-id="631fa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="631fa-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="631fa-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="631fa-132">Content-Type</span></span>|<span data-ttu-id="631fa-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="631fa-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="631fa-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="631fa-135">Request body</span></span>
<span data-ttu-id="631fa-136">在请求正文中，提供具有更新的电子邮件地址的 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="631fa-136">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the updated email address.</span></span>

<span data-ttu-id="631fa-137">下表显示了在更新 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="631fa-137">The following table shows the properties that are required when you update the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="631fa-138">属性</span><span class="sxs-lookup"><span data-stu-id="631fa-138">Property</span></span>|<span data-ttu-id="631fa-139">类型</span><span class="sxs-lookup"><span data-stu-id="631fa-139">Type</span></span>|<span data-ttu-id="631fa-140">Description</span><span class="sxs-lookup"><span data-stu-id="631fa-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="631fa-141">emailAddress</span><span class="sxs-lookup"><span data-stu-id="631fa-141">emailAddress</span></span>|<span data-ttu-id="631fa-142">String</span><span class="sxs-lookup"><span data-stu-id="631fa-142">String</span></span>|<span data-ttu-id="631fa-143">更新的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="631fa-143">Updated email address</span></span>|



## <a name="response"></a><span data-ttu-id="631fa-144">响应</span><span class="sxs-lookup"><span data-stu-id="631fa-144">Response</span></span>

<span data-ttu-id="631fa-145">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="631fa-145">If successful, this method returns a `200 OK` response code and an updated [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="631fa-146">示例</span><span class="sxs-lookup"><span data-stu-id="631fa-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="631fa-147">请求</span><span class="sxs-lookup"><span data-stu-id="631fa-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="631fa-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="631fa-148">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="631fa-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="631fa-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="631fa-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="631fa-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="631fa-151">响应</span><span class="sxs-lookup"><span data-stu-id="631fa-151">Response</span></span>

<span data-ttu-id="631fa-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="631fa-152">The following is an example of the response.</span></span>

<span data-ttu-id="631fa-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="631fa-153">**Note:** The response object shown here might be shortened for readability.</span></span>

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
