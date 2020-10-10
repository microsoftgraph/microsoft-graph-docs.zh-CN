---
title: 列出 fido2AuthenticationMethod
description: 检索 fido2AuthenticationMethod 对象及其属性的列表。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 98b078f4b79af76e2618c94f533b5d4e4b6d672f
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418198"
---
# <a name="list-fido2authenticationmethod"></a><span data-ttu-id="738c5-103">列出 fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="738c5-103">List fido2AuthenticationMethod</span></span>
<span data-ttu-id="738c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="738c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="738c5-105">检索用户的 [FIDO2 安全密钥身份验证方法](../resources/fido2authenticationmethod.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="738c5-105">Retrieve a list of a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="738c5-106">权限</span><span class="sxs-lookup"><span data-stu-id="738c5-106">Permissions</span></span>
<span data-ttu-id="738c5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="738c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="738c5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="738c5-109">Permission type</span></span>|<span data-ttu-id="738c5-110">从最高特权到最少特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="738c5-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="738c5-111">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="738c5-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="738c5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="738c5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="738c5-113">UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、All 和 All</span><span class="sxs-lookup"><span data-stu-id="738c5-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="738c5-114">UserAuthenticationMethod、UserAuthenticationMethod 和所有</span><span class="sxs-lookup"><span data-stu-id="738c5-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="738c5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="738c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="738c5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="738c5-116">Not supported.</span></span>|<span data-ttu-id="738c5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="738c5-117">Not supported.</span></span>
|<span data-ttu-id="738c5-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="738c5-118">Application</span></span>|<span data-ttu-id="738c5-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="738c5-119">Not supported.</span></span>|<span data-ttu-id="738c5-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="738c5-120">Not supported.</span></span>

<span data-ttu-id="738c5-121">对于在其他用户上执行管理的委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="738c5-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="738c5-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="738c5-122">Global admin</span></span>
* <span data-ttu-id="738c5-123">全局读取者</span><span class="sxs-lookup"><span data-stu-id="738c5-123">Global reader</span></span>
* <span data-ttu-id="738c5-124">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="738c5-124">Privileged authentication admin</span></span>
* <span data-ttu-id="738c5-125">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="738c5-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="738c5-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="738c5-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2Methods
GET /users/{id | userPrincipalName}/authentication/fido2Methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="738c5-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="738c5-127">Optional query parameters</span></span>
<span data-ttu-id="738c5-128">此方法不支持用于自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="738c5-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="738c5-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="738c5-129">Request headers</span></span>
|<span data-ttu-id="738c5-130">名称</span><span class="sxs-lookup"><span data-stu-id="738c5-130">Name</span></span>|<span data-ttu-id="738c5-131">说明</span><span class="sxs-lookup"><span data-stu-id="738c5-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="738c5-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="738c5-132">Authorization</span></span>|<span data-ttu-id="738c5-133">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="738c5-133">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="738c5-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="738c5-134">Request body</span></span>
<span data-ttu-id="738c5-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="738c5-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="738c5-136">响应</span><span class="sxs-lookup"><span data-stu-id="738c5-136">Response</span></span>

<span data-ttu-id="738c5-137">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="738c5-137">If successful, this method returns a `200 OK` response code and a collection of [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="738c5-138">示例</span><span class="sxs-lookup"><span data-stu-id="738c5-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="738c5-139">请求</span><span class="sxs-lookup"><span data-stu-id="738c5-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/fido2Methods
```


### <a name="response"></a><span data-ttu-id="738c5-140">响应</span><span class="sxs-lookup"><span data-stu-id="738c5-140">Response</span></span>
<span data-ttu-id="738c5-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="738c5-141">The following is an example of the response.</span></span>

<span data-ttu-id="738c5-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="738c5-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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

