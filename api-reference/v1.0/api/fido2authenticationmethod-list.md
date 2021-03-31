---
title: 列出 fido2AuthenticationMethod
description: 检索 fido2AuthenticationMethod 对象及其属性的列表。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 166ac533d85e43fdc413f614ce848cdbdb5c56e7
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469267"
---
# <a name="list-fido2authenticationmethod"></a><span data-ttu-id="69711-103">列出 fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="69711-103">List fido2AuthenticationMethod</span></span>
<span data-ttu-id="69711-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69711-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69711-105">检索用户的 [FIDO2](../resources/fido2authenticationmethod.md) 安全密钥身份验证方法对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="69711-105">Retrieve a list of a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="69711-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="69711-106">Permissions</span></span>

<span data-ttu-id="69711-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69711-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="69711-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="69711-109">Permissions acting on self</span></span>

|<span data-ttu-id="69711-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="69711-110">Permission type</span></span>      | <span data-ttu-id="69711-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69711-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="69711-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69711-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="69711-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69711-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="69711-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69711-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69711-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="69711-115">Not supported.</span></span> |
| <span data-ttu-id="69711-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="69711-116">Application</span></span>                            | <span data-ttu-id="69711-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="69711-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="69711-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="69711-118">Permissions acting on other users</span></span>

|<span data-ttu-id="69711-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="69711-119">Permission type</span></span>      | <span data-ttu-id="69711-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69711-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="69711-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69711-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="69711-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69711-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="69711-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69711-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69711-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="69711-124">Not supported.</span></span> |
| <span data-ttu-id="69711-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="69711-125">Application</span></span>                            | <span data-ttu-id="69711-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69711-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="69711-127">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="69711-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="69711-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="69711-128">Global admin</span></span>
* <span data-ttu-id="69711-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="69711-129">Global reader</span></span>
* <span data-ttu-id="69711-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="69711-130">Privileged authentication admin</span></span>
* <span data-ttu-id="69711-131">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="69711-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="69711-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69711-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2Methods
GET /users/{id | userPrincipalName}/authentication/fido2Methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69711-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="69711-133">Optional query parameters</span></span>
<span data-ttu-id="69711-134">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="69711-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69711-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="69711-135">Request headers</span></span>
|<span data-ttu-id="69711-136">名称</span><span class="sxs-lookup"><span data-stu-id="69711-136">Name</span></span>|<span data-ttu-id="69711-137">说明</span><span class="sxs-lookup"><span data-stu-id="69711-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="69711-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="69711-138">Authorization</span></span>|<span data-ttu-id="69711-139">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="69711-139">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="69711-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="69711-140">Request body</span></span>
<span data-ttu-id="69711-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="69711-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69711-142">响应</span><span class="sxs-lookup"><span data-stu-id="69711-142">Response</span></span>

<span data-ttu-id="69711-143">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="69711-143">If successful, this method returns a `200 OK` response code and a collection of [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="69711-144">示例</span><span class="sxs-lookup"><span data-stu-id="69711-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="69711-145">请求</span><span class="sxs-lookup"><span data-stu-id="69711-145">Request</span></span>


``` http
GET https://graph.microsoft.com/v1.0/me/authentication/fido2Methods
```

### <a name="response"></a><span data-ttu-id="69711-146">响应</span><span class="sxs-lookup"><span data-stu-id="69711-146">Response</span></span>
<span data-ttu-id="69711-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="69711-147">The following is an example of the response.</span></span>

<span data-ttu-id="69711-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="69711-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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

