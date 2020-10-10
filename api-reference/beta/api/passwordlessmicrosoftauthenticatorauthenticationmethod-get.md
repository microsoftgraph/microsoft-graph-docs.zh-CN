---
title: 获取 passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: 读取 passwordlessMicrosoftAuthenticatorAuthenticationMethod 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8402360e4d4ca87afe2f09aa5b03a52e452aa0a8
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418283"
---
# <a name="get-passwordlessmicrosoftauthenticatorauthenticationmethod"></a><span data-ttu-id="dc399-103">获取 passwordlessMicrosoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="dc399-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="dc399-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc399-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc399-105">检索用户的单一 [Microsoft 身份验证器 Passwordless 电话登录方法](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dc399-105">Retrieve a user's single [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="dc399-106">在 Api 位于 Mirosoft Graph beta 过程中时，规划用于管理 Microsoft 身份验证器应用程序的 Api 的大量架构更改。</span><span class="sxs-lookup"><span data-stu-id="dc399-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="dc399-107">由于调用模式将发生更改，因此我们建议您不要对这些 Api 进行生产依赖。</span><span class="sxs-lookup"><span data-stu-id="dc399-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc399-108">权限</span><span class="sxs-lookup"><span data-stu-id="dc399-108">Permissions</span></span>
<span data-ttu-id="dc399-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc399-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc399-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc399-111">Permission type</span></span>|<span data-ttu-id="dc399-112">从最高特权到最少特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="dc399-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="dc399-113">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="dc399-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="dc399-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc399-114">Delegated (work or school account)</span></span>|<span data-ttu-id="dc399-115">UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、All 和 All</span><span class="sxs-lookup"><span data-stu-id="dc399-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="dc399-116">UserAuthenticationMethod、UserAuthenticationMethod 和所有</span><span class="sxs-lookup"><span data-stu-id="dc399-116">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="dc399-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc399-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc399-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc399-118">Not supported.</span></span>|<span data-ttu-id="dc399-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc399-119">Not supported.</span></span>
|<span data-ttu-id="dc399-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc399-120">Application</span></span>|<span data-ttu-id="dc399-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc399-121">Not supported.</span></span>|<span data-ttu-id="dc399-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc399-122">Not supported.</span></span>

<span data-ttu-id="dc399-123">对于在其他用户上执行管理的委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="dc399-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="dc399-124">全局管理员</span><span class="sxs-lookup"><span data-stu-id="dc399-124">Global admin</span></span>
* <span data-ttu-id="dc399-125">全局读取者</span><span class="sxs-lookup"><span data-stu-id="dc399-125">Global reader</span></span>
* <span data-ttu-id="dc399-126">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="dc399-126">Privileged authentication admin</span></span>
* <span data-ttu-id="dc399-127">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="dc399-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="dc399-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc399-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dc399-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc399-129">Request headers</span></span>
|<span data-ttu-id="dc399-130">名称</span><span class="sxs-lookup"><span data-stu-id="dc399-130">Name</span></span>|<span data-ttu-id="dc399-131">说明</span><span class="sxs-lookup"><span data-stu-id="dc399-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dc399-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc399-132">Authorization</span></span>|<span data-ttu-id="dc399-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dc399-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc399-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc399-135">Request body</span></span>
<span data-ttu-id="dc399-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dc399-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc399-137">响应</span><span class="sxs-lookup"><span data-stu-id="dc399-137">Response</span></span>

<span data-ttu-id="dc399-138">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dc399-138">If successful, this method returns a `200 OK` response code and the requested [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dc399-139">示例</span><span class="sxs-lookup"><span data-stu-id="dc399-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dc399-140">请求</span><span class="sxs-lookup"><span data-stu-id="dc399-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```


### <a name="response"></a><span data-ttu-id="dc399-141">响应</span><span class="sxs-lookup"><span data-stu-id="dc399-141">Response</span></span>
<span data-ttu-id="dc399-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dc399-142">The following is an example of the response.</span></span>

<span data-ttu-id="dc399-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dc399-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": {
      "id": "R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1",
      "displayName": "My mobile phone",
      "creationDateTime": "2020-09-02T04:16:49Z"
  }
}
```

