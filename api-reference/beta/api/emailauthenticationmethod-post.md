---
title: 创建 emailAuthenticationMethod
description: 创建新的 emailAuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0fa084db81af3677f5a6e12c6d90020178653b4f
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458127"
---
# <a name="create-emailauthenticationmethod"></a><span data-ttu-id="edc3b-103">创建 emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="edc3b-103">Create emailAuthenticationMethod</span></span>
<span data-ttu-id="edc3b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edc3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edc3b-105">设置用户的 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="edc3b-105">Set a user's [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object.</span></span> <span data-ttu-id="edc3b-106">电子邮件身份验证是一种自助密码重置方法。</span><span class="sxs-lookup"><span data-stu-id="edc3b-106">Email authentication is a self-service password reset method.</span></span> <span data-ttu-id="edc3b-107">一个用户可能只有一种电子邮件身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="edc3b-107">A user may only have one email authentication method.</span></span>

## <a name="permissions"></a><span data-ttu-id="edc3b-108">权限</span><span class="sxs-lookup"><span data-stu-id="edc3b-108">Permissions</span></span>
<span data-ttu-id="edc3b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="edc3b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edc3b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="edc3b-111">Permission type</span></span>|<span data-ttu-id="edc3b-112">从最高特权到最少特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="edc3b-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="edc3b-113">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="edc3b-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="edc3b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="edc3b-114">Delegated (work or school account)</span></span>|<span data-ttu-id="edc3b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="edc3b-115">Not supported.</span></span>|<span data-ttu-id="edc3b-116">UserAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="edc3b-116">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="edc3b-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="edc3b-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edc3b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="edc3b-118">Not supported.</span></span>|<span data-ttu-id="edc3b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="edc3b-119">Not supported.</span></span>
|<span data-ttu-id="edc3b-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="edc3b-120">Application</span></span>|<span data-ttu-id="edc3b-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="edc3b-121">Not supported.</span></span>|<span data-ttu-id="edc3b-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="edc3b-122">Not supported.</span></span>

<span data-ttu-id="edc3b-123">对于在其他用户上执行管理的委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="edc3b-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="edc3b-124">全局管理员</span><span class="sxs-lookup"><span data-stu-id="edc3b-124">Global admin</span></span>
* <span data-ttu-id="edc3b-125">全局读取者</span><span class="sxs-lookup"><span data-stu-id="edc3b-125">Global reader</span></span>
* <span data-ttu-id="edc3b-126">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="edc3b-126">Privileged authentication admin</span></span>
* <span data-ttu-id="edc3b-127">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="edc3b-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="edc3b-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="edc3b-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="request-headers"></a><span data-ttu-id="edc3b-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="edc3b-129">Request headers</span></span>
|<span data-ttu-id="edc3b-130">名称</span><span class="sxs-lookup"><span data-stu-id="edc3b-130">Name</span></span>|<span data-ttu-id="edc3b-131">说明</span><span class="sxs-lookup"><span data-stu-id="edc3b-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="edc3b-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="edc3b-132">Authorization</span></span>|<span data-ttu-id="edc3b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="edc3b-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="edc3b-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="edc3b-135">Content-Type</span></span>|<span data-ttu-id="edc3b-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="edc3b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="edc3b-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="edc3b-138">Request body</span></span>
<span data-ttu-id="edc3b-139">在请求正文中，提供具有所需电子邮件地址的 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edc3b-139">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the desired email address.</span></span>

<span data-ttu-id="edc3b-140">下表显示创建 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="edc3b-140">The following table shows the properties that are required when you create the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="edc3b-141">属性</span><span class="sxs-lookup"><span data-stu-id="edc3b-141">Property</span></span>|<span data-ttu-id="edc3b-142">类型</span><span class="sxs-lookup"><span data-stu-id="edc3b-142">Type</span></span>|<span data-ttu-id="edc3b-143">说明</span><span class="sxs-lookup"><span data-stu-id="edc3b-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edc3b-144">emailAddress</span><span class="sxs-lookup"><span data-stu-id="edc3b-144">emailAddress</span></span>|<span data-ttu-id="edc3b-145">String</span><span class="sxs-lookup"><span data-stu-id="edc3b-145">String</span></span>|<span data-ttu-id="edc3b-146">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="edc3b-146">Email address</span></span>|



## <a name="response"></a><span data-ttu-id="edc3b-147">响应</span><span class="sxs-lookup"><span data-stu-id="edc3b-147">Response</span></span>

<span data-ttu-id="edc3b-148">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="edc3b-148">If successful, this method returns a `201 Created` response code and a new [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="edc3b-149">示例</span><span class="sxs-lookup"><span data-stu-id="edc3b-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="edc3b-150">请求</span><span class="sxs-lookup"><span data-stu-id="edc3b-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="edc3b-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="edc3b-151">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="edc3b-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edc3b-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="edc3b-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="edc3b-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="edc3b-154">响应</span><span class="sxs-lookup"><span data-stu-id="edc3b-154">Response</span></span>
<span data-ttu-id="edc3b-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="edc3b-155">The following is an example of the response.</span></span>

<span data-ttu-id="edc3b-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="edc3b-156">**Note:** The response object shown here might be shortened for readability.</span></span>
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
