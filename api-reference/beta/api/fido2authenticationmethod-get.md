---
title: 获取 fido2AuthenticationMethod
description: 读取 fido2AuthenticationMethod 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4b5bad06b344db8355b1c73c7bf7886517795027
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959232"
---
# <a name="get-fido2authenticationmethod"></a><span data-ttu-id="90332-103">获取 fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="90332-103">Get fido2AuthenticationMethod</span></span>
<span data-ttu-id="90332-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90332-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90332-105">检索用户的单个 [FIDO2 安全密钥身份验证方法](../resources/fido2authenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="90332-105">Retrieve a user's single [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="90332-106">权限</span><span class="sxs-lookup"><span data-stu-id="90332-106">Permissions</span></span>
<span data-ttu-id="90332-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90332-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90332-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="90332-109">Permission type</span></span>|<span data-ttu-id="90332-110">自行操作的权限 (权限从最低权限级别) </span><span class="sxs-lookup"><span data-stu-id="90332-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="90332-111">对他人操作的权限 (权限从最低到最多特权) </span><span class="sxs-lookup"><span data-stu-id="90332-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="90332-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90332-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="90332-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90332-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="90332-114">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90332-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="90332-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90332-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90332-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="90332-116">Not supported.</span></span> | <span data-ttu-id="90332-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="90332-117">Not supported.</span></span> |
| <span data-ttu-id="90332-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="90332-118">Application</span></span>                            | <span data-ttu-id="90332-119">不适用。</span><span class="sxs-lookup"><span data-stu-id="90332-119">Not applicable.</span></span> | <span data-ttu-id="90332-120">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90332-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="90332-121">对于管理员正在操作其他用户的委派方案，管理员需要下列角色之 [一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="90332-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="90332-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="90332-122">Global admin</span></span>
* <span data-ttu-id="90332-123">全局读取者</span><span class="sxs-lookup"><span data-stu-id="90332-123">Global reader</span></span>
* <span data-ttu-id="90332-124">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="90332-124">Privileged authentication admin</span></span>
* <span data-ttu-id="90332-125">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="90332-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="90332-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90332-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2Methods/{id}
GET /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="90332-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="90332-127">Request headers</span></span>
|<span data-ttu-id="90332-128">名称</span><span class="sxs-lookup"><span data-stu-id="90332-128">Name</span></span>|<span data-ttu-id="90332-129">说明</span><span class="sxs-lookup"><span data-stu-id="90332-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="90332-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="90332-130">Authorization</span></span>|<span data-ttu-id="90332-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="90332-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="90332-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="90332-133">Request body</span></span>
<span data-ttu-id="90332-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="90332-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90332-135">响应</span><span class="sxs-lookup"><span data-stu-id="90332-135">Response</span></span>

<span data-ttu-id="90332-136">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="90332-136">If successful, this method returns a `200 OK` response code and the requested [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90332-137">示例</span><span class="sxs-lookup"><span data-stu-id="90332-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="90332-138">请求</span><span class="sxs-lookup"><span data-stu-id="90332-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="90332-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="90332-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethod_1"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/fido2Methods/-2_GRUg2-HYz6_1YG4YRAQ2
```
# <a name="c"></a>[<span data-ttu-id="90332-140">C#</span><span class="sxs-lookup"><span data-stu-id="90332-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fido2authenticationmethod-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90332-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90332-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fido2authenticationmethod-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90332-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90332-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fido2authenticationmethod-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90332-143">Java</span><span class="sxs-lookup"><span data-stu-id="90332-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-fido2authenticationmethod-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="90332-144">响应</span><span class="sxs-lookup"><span data-stu-id="90332-144">Response</span></span>
<span data-ttu-id="90332-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="90332-145">The following is an example of the response.</span></span>

<span data-ttu-id="90332-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="90332-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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

