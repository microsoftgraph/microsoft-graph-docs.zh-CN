---
title: 获取 fido2AuthenticationMethod
description: 读取 fido2AuthenticationMethod 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b13b9502c1587fcef5a20a07cc4b57d0300f91ee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964654"
---
# <a name="get-fido2authenticationmethod"></a><span data-ttu-id="80501-103">获取 fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="80501-103">Get fido2AuthenticationMethod</span></span>
<span data-ttu-id="80501-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80501-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="80501-105">检索用户的单个 [FIDO2 安全密钥身份验证方法](../resources/fido2authenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80501-105">Retrieve a user's single [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="80501-106">权限</span><span class="sxs-lookup"><span data-stu-id="80501-106">Permissions</span></span>

<span data-ttu-id="80501-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80501-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="80501-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="80501-109">Permissions acting on self</span></span>

|<span data-ttu-id="80501-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="80501-110">Permission type</span></span>      | <span data-ttu-id="80501-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80501-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="80501-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80501-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="80501-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80501-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="80501-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80501-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80501-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="80501-115">Not supported.</span></span> |
| <span data-ttu-id="80501-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="80501-116">Application</span></span>                            | <span data-ttu-id="80501-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="80501-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="80501-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="80501-118">Permissions acting on other users</span></span>

|<span data-ttu-id="80501-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="80501-119">Permission type</span></span>      | <span data-ttu-id="80501-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80501-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="80501-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80501-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="80501-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80501-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="80501-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80501-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80501-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="80501-124">Not supported.</span></span> |
| <span data-ttu-id="80501-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="80501-125">Application</span></span>                            | <span data-ttu-id="80501-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80501-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="80501-127">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="80501-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="80501-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="80501-128">Global admin</span></span>
* <span data-ttu-id="80501-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="80501-129">Global reader</span></span>
* <span data-ttu-id="80501-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="80501-130">Privileged authentication admin</span></span>
* <span data-ttu-id="80501-131">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="80501-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="80501-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80501-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2AuthenticationMethod/{id}
GET /users/{id | userPrincipalName}/authentication/fido2AuthenticationMethod/{id}
```

## <a name="request-headers"></a><span data-ttu-id="80501-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="80501-133">Request headers</span></span>
|<span data-ttu-id="80501-134">名称</span><span class="sxs-lookup"><span data-stu-id="80501-134">Name</span></span>|<span data-ttu-id="80501-135">说明</span><span class="sxs-lookup"><span data-stu-id="80501-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="80501-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="80501-136">Authorization</span></span>|<span data-ttu-id="80501-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80501-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="80501-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="80501-139">Request body</span></span>
<span data-ttu-id="80501-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="80501-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80501-141">响应</span><span class="sxs-lookup"><span data-stu-id="80501-141">Response</span></span>

<span data-ttu-id="80501-142">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80501-142">If successful, this method returns a `200 OK` response code and the requested [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="80501-143">示例</span><span class="sxs-lookup"><span data-stu-id="80501-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="80501-144">请求</span><span class="sxs-lookup"><span data-stu-id="80501-144">Request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/me/authentication/fido2AuthenticationMethod/-2_GRUg2-HYz6_1YG4YRAQ2
```

### <a name="response"></a><span data-ttu-id="80501-145">响应</span><span class="sxs-lookup"><span data-stu-id="80501-145">Response</span></span>
<span data-ttu-id="80501-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="80501-146">The following is an example of the response.</span></span>

<span data-ttu-id="80501-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="80501-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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

