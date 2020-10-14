---
title: 获取 emailAuthenticationMethod
description: 读取 emailAuthenticationMethod 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e16e19f52a78d1c119bb561555f6b916e71e8346
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458222"
---
# <a name="get-emailauthenticationmethod"></a><span data-ttu-id="af384-103">获取 emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="af384-103">Get emailAuthenticationMethod</span></span>
<span data-ttu-id="af384-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af384-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af384-105">检索用户的单个 [电子邮件身份验证方法](../resources/emailauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="af384-105">Retrieve a user's single [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="af384-106">权限</span><span class="sxs-lookup"><span data-stu-id="af384-106">Permissions</span></span>
<span data-ttu-id="af384-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="af384-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af384-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="af384-109">Permission type</span></span>|<span data-ttu-id="af384-110">从最高特权到最少特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="af384-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="af384-111">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="af384-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="af384-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="af384-112">Delegated (work or school account)</span></span>|<span data-ttu-id="af384-113">UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、All 和 All</span><span class="sxs-lookup"><span data-stu-id="af384-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="af384-114">UserAuthenticationMethod、UserAuthenticationMethod 和所有</span><span class="sxs-lookup"><span data-stu-id="af384-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="af384-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="af384-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af384-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="af384-116">Not supported.</span></span>|<span data-ttu-id="af384-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="af384-117">Not supported.</span></span>
|<span data-ttu-id="af384-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="af384-118">Application</span></span>|<span data-ttu-id="af384-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="af384-119">Not supported.</span></span>|<span data-ttu-id="af384-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="af384-120">Not supported.</span></span>

<span data-ttu-id="af384-121">对于在其他用户上执行管理的委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="af384-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="af384-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="af384-122">Global admin</span></span>
* <span data-ttu-id="af384-123">全局读取者</span><span class="sxs-lookup"><span data-stu-id="af384-123">Global reader</span></span>
* <span data-ttu-id="af384-124">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="af384-124">Privileged authentication admin</span></span>
* <span data-ttu-id="af384-125">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="af384-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="af384-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="af384-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/emailMethods/{id}
GET /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="af384-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="af384-127">Request headers</span></span>
|<span data-ttu-id="af384-128">名称</span><span class="sxs-lookup"><span data-stu-id="af384-128">Name</span></span>|<span data-ttu-id="af384-129">说明</span><span class="sxs-lookup"><span data-stu-id="af384-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="af384-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="af384-130">Authorization</span></span>|<span data-ttu-id="af384-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="af384-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="af384-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="af384-133">Request body</span></span>
<span data-ttu-id="af384-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="af384-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af384-135">响应</span><span class="sxs-lookup"><span data-stu-id="af384-135">Response</span></span>

<span data-ttu-id="af384-136">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="af384-136">If successful, this method returns a `200 OK` response code and the requested [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="af384-137">示例</span><span class="sxs-lookup"><span data-stu-id="af384-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="af384-138">请求</span><span class="sxs-lookup"><span data-stu-id="af384-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="af384-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="af384-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```
# <a name="c"></a>[<span data-ttu-id="af384-140">C#</span><span class="sxs-lookup"><span data-stu-id="af384-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af384-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af384-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af384-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af384-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="af384-143">响应</span><span class="sxs-lookup"><span data-stu-id="af384-143">Response</span></span>
<span data-ttu-id="af384-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="af384-144">The following is an example of the response.</span></span>

<span data-ttu-id="af384-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="af384-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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

