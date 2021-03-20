---
title: 列出 fido2AuthenticationMethod
description: 检索 fido2AuthenticationMethod 对象及其属性的列表。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e6755328e47b39a36d0882fa2fb15921a25a4456
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953306"
---
# <a name="list-fido2authenticationmethod"></a><span data-ttu-id="b76bc-103">列出 fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b76bc-103">List fido2AuthenticationMethod</span></span>
<span data-ttu-id="b76bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b76bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b76bc-105">检索用户的 [FIDO2](../resources/fido2authenticationmethod.md) 安全密钥身份验证方法对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="b76bc-105">Retrieve a list of a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="b76bc-106">权限</span><span class="sxs-lookup"><span data-stu-id="b76bc-106">Permissions</span></span>
<span data-ttu-id="b76bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b76bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b76bc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b76bc-109">Permission type</span></span>|<span data-ttu-id="b76bc-110">自行操作的权限 (权限从最低权限级别) </span><span class="sxs-lookup"><span data-stu-id="b76bc-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="b76bc-111">对他人操作的权限 (权限从最低到最多特权) </span><span class="sxs-lookup"><span data-stu-id="b76bc-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="b76bc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b76bc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b76bc-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b76bc-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="b76bc-114">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b76bc-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="b76bc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b76bc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b76bc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b76bc-116">Not supported.</span></span> | <span data-ttu-id="b76bc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b76bc-117">Not supported.</span></span> |
| <span data-ttu-id="b76bc-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b76bc-118">Application</span></span>                            | <span data-ttu-id="b76bc-119">不适用。</span><span class="sxs-lookup"><span data-stu-id="b76bc-119">Not applicable.</span></span> | <span data-ttu-id="b76bc-120">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b76bc-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="b76bc-121">对于管理员正在操作其他用户的委派方案，管理员需要下列角色之 [一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="b76bc-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="b76bc-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="b76bc-122">Global admin</span></span>
* <span data-ttu-id="b76bc-123">全局读取者</span><span class="sxs-lookup"><span data-stu-id="b76bc-123">Global reader</span></span>
* <span data-ttu-id="b76bc-124">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="b76bc-124">Privileged authentication admin</span></span>
* <span data-ttu-id="b76bc-125">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="b76bc-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="b76bc-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b76bc-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2Methods
GET /users/{id | userPrincipalName}/authentication/fido2Methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b76bc-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b76bc-127">Optional query parameters</span></span>
<span data-ttu-id="b76bc-128">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="b76bc-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b76bc-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="b76bc-129">Request headers</span></span>
|<span data-ttu-id="b76bc-130">名称</span><span class="sxs-lookup"><span data-stu-id="b76bc-130">Name</span></span>|<span data-ttu-id="b76bc-131">说明</span><span class="sxs-lookup"><span data-stu-id="b76bc-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b76bc-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="b76bc-132">Authorization</span></span>|<span data-ttu-id="b76bc-133">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="b76bc-133">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b76bc-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="b76bc-134">Request body</span></span>
<span data-ttu-id="b76bc-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b76bc-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b76bc-136">响应</span><span class="sxs-lookup"><span data-stu-id="b76bc-136">Response</span></span>

<span data-ttu-id="b76bc-137">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b76bc-137">If successful, this method returns a `200 OK` response code and a collection of [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b76bc-138">示例</span><span class="sxs-lookup"><span data-stu-id="b76bc-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b76bc-139">请求</span><span class="sxs-lookup"><span data-stu-id="b76bc-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b76bc-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b76bc-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethod_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/fido2Methods
```
# <a name="c"></a>[<span data-ttu-id="b76bc-141">C#</span><span class="sxs-lookup"><span data-stu-id="b76bc-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fido2authenticationmethod-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b76bc-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b76bc-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fido2authenticationmethod-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b76bc-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b76bc-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fido2authenticationmethod-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b76bc-144">Java</span><span class="sxs-lookup"><span data-stu-id="b76bc-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-fido2authenticationmethod-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b76bc-145">响应</span><span class="sxs-lookup"><span data-stu-id="b76bc-145">Response</span></span>
<span data-ttu-id="b76bc-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b76bc-146">The following is an example of the response.</span></span>

<span data-ttu-id="b76bc-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b76bc-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.fido2AuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": [
    {
      "id": "-2_GRUg2-HYz6_1YG4YRAQ2",
      "displayName": "Red key",
      "creationDateTime": "2020-08-10T06:44:09Z",
      "aaGuid": "2fc0579f-8113-47ea-b116-555a8db9202a",
      "model": "NFC key",
      "attestationCertificates": [
          "dbe793efdf1945e2df25d93653a1e8a3268a9075"
      ],
      "attestationLevel": "attested"
    },
    {
      "id": "_jpuR-TGZgk6aQCLF3BQjA2",
      "displayName": "Blue key",
      "creationDateTime": "2020-08-10T06:25:38Z",
      "aaGuid": "c5ef55ff-ad9a-4b9f-b580-ababafe026d0",
      "model": "USB key",
      "attestationCertificates": [
          "b479e7652167f574296e76bfa76731b8ccd22ed7"
      ],
      "attestationLevel": "attested"
    }
  ]
}
```

