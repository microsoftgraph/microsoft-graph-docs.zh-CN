---
title: 获取 fido2AuthenticationMethod
description: 读取 fido2AuthenticationMethod 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0144069949623693005855426ca483bedebcac74
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418200"
---
# <a name="get-fido2authenticationmethod"></a><span data-ttu-id="5f20b-103">获取 fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5f20b-103">Get fido2AuthenticationMethod</span></span>
<span data-ttu-id="5f20b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f20b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f20b-105">检索用户的单一 [FIDO2 安全密钥身份验证方法](../resources/fido2authenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5f20b-105">Retrieve a user's single [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f20b-106">权限</span><span class="sxs-lookup"><span data-stu-id="5f20b-106">Permissions</span></span>
<span data-ttu-id="5f20b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f20b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f20b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f20b-109">Permission type</span></span>|<span data-ttu-id="5f20b-110">从最高特权到最少特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="5f20b-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="5f20b-111">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="5f20b-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="5f20b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f20b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5f20b-113">UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、All 和 All</span><span class="sxs-lookup"><span data-stu-id="5f20b-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="5f20b-114">UserAuthenticationMethod、UserAuthenticationMethod 和所有</span><span class="sxs-lookup"><span data-stu-id="5f20b-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="5f20b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f20b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f20b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f20b-116">Not supported.</span></span>|<span data-ttu-id="5f20b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f20b-117">Not supported.</span></span>
|<span data-ttu-id="5f20b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f20b-118">Application</span></span>|<span data-ttu-id="5f20b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f20b-119">Not supported.</span></span>|<span data-ttu-id="5f20b-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f20b-120">Not supported.</span></span>

<span data-ttu-id="5f20b-121">对于在其他用户上执行管理的委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="5f20b-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="5f20b-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="5f20b-122">Global admin</span></span>
* <span data-ttu-id="5f20b-123">全局读取者</span><span class="sxs-lookup"><span data-stu-id="5f20b-123">Global reader</span></span>
* <span data-ttu-id="5f20b-124">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="5f20b-124">Privileged authentication admin</span></span>
* <span data-ttu-id="5f20b-125">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="5f20b-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="5f20b-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f20b-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2AuthenticationMethod/{id}
GET /users/{id | userPrincipalName}/authentication/fido2AuthenticationMethod/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5f20b-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f20b-127">Request headers</span></span>
|<span data-ttu-id="5f20b-128">名称</span><span class="sxs-lookup"><span data-stu-id="5f20b-128">Name</span></span>|<span data-ttu-id="5f20b-129">说明</span><span class="sxs-lookup"><span data-stu-id="5f20b-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5f20b-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f20b-130">Authorization</span></span>|<span data-ttu-id="5f20b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5f20b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f20b-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f20b-133">Request body</span></span>
<span data-ttu-id="5f20b-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5f20b-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f20b-135">响应</span><span class="sxs-lookup"><span data-stu-id="5f20b-135">Response</span></span>

<span data-ttu-id="5f20b-136">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5f20b-136">If successful, this method returns a `200 OK` response code and the requested [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f20b-137">示例</span><span class="sxs-lookup"><span data-stu-id="5f20b-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5f20b-138">请求</span><span class="sxs-lookup"><span data-stu-id="5f20b-138">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/fido2AuthenticationMethod/-2_GRUg2-HYz6_1YG4YRAQ2
```


### <a name="response"></a><span data-ttu-id="5f20b-139">响应</span><span class="sxs-lookup"><span data-stu-id="5f20b-139">Response</span></span>
<span data-ttu-id="5f20b-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5f20b-140">The following is an example of the response.</span></span>

<span data-ttu-id="5f20b-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5f20b-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fido2AuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": {
      "id": "-2_GRUg2-HYz6_1YG4YRAQ2",
      "displayName": "Red key",
      "creationDateTime": "2020-08-10T06:44:09Z",
      "aaGuid": "2fc0579f-8113-47ea-b116-555a8db9202a",
      "model": "NFC key",
      "attestationCertificates": [
          "dbe793efdf1945e2df25d93653a1e8a3268a9075"
      ],
      "attestationLevel": "attested"
  }
}
```

