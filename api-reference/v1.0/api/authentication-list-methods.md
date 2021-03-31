---
title: List 方法
description: 检索身份验证方法对象的列表。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1cca7f87bc5eb6b0c12108b0214ab81db99f0568
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468595"
---
# <a name="list-methods"></a><span data-ttu-id="ab810-103">List 方法</span><span class="sxs-lookup"><span data-stu-id="ab810-103">List methods</span></span>

<span data-ttu-id="ab810-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab810-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab810-105">检索身份验证 [方法对象](../resources/authenticationmethod.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="ab810-105">Retrieve a list of [authentication method](../resources/authenticationmethod.md) objects.</span></span>

> <span data-ttu-id="ab810-106">**注意：** 仅返回 v1.0 上支持的方法。</span><span class="sxs-lookup"><span data-stu-id="ab810-106">**Note:** Only methods supported on v1.0 will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab810-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="ab810-107">Permissions</span></span>

<span data-ttu-id="ab810-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab810-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="ab810-110">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="ab810-110">Permissions acting on self</span></span>

|<span data-ttu-id="ab810-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab810-111">Permission type</span></span>      | <span data-ttu-id="ab810-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ab810-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="ab810-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab810-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab810-114">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab810-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="ab810-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab810-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab810-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab810-116">Not supported.</span></span> |
| <span data-ttu-id="ab810-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab810-117">Application</span></span>                            | <span data-ttu-id="ab810-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab810-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="ab810-119">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="ab810-119">Permissions acting on other users</span></span>

|<span data-ttu-id="ab810-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab810-120">Permission type</span></span>      | <span data-ttu-id="ab810-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ab810-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="ab810-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab810-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab810-123">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab810-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="ab810-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab810-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab810-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab810-125">Not supported.</span></span> |
| <span data-ttu-id="ab810-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab810-126">Application</span></span>                            | <span data-ttu-id="ab810-127">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab810-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="ab810-128">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="ab810-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="ab810-129">全局管理员</span><span class="sxs-lookup"><span data-stu-id="ab810-129">Global admin</span></span>
* <span data-ttu-id="ab810-130">全局读取者</span><span class="sxs-lookup"><span data-stu-id="ab810-130">Global reader</span></span>
* <span data-ttu-id="ab810-131">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="ab810-131">Privileged authentication admin</span></span>
* <span data-ttu-id="ab810-132">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="ab810-132">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="ab810-133">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab810-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods
GET /users/{id | userPrincipalName}/authentication/methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab810-134">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ab810-134">Optional query parameters</span></span>

<span data-ttu-id="ab810-135">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="ab810-135">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab810-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab810-136">Request headers</span></span>

| <span data-ttu-id="ab810-137">名称</span><span class="sxs-lookup"><span data-stu-id="ab810-137">Name</span></span>      |<span data-ttu-id="ab810-138">说明</span><span class="sxs-lookup"><span data-stu-id="ab810-138">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ab810-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab810-139">Authorization</span></span> | <span data-ttu-id="ab810-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ab810-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab810-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab810-142">Request body</span></span>

<span data-ttu-id="ab810-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ab810-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab810-144">响应</span><span class="sxs-lookup"><span data-stu-id="ab810-144">Response</span></span>

<span data-ttu-id="ab810-145">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [authenticationMethod](../resources/authenticationmethod.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ab810-145">If successful, this method returns a `200 OK` response code and a collection of [authenticationMethod](../resources/authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ab810-146">示例</span><span class="sxs-lookup"><span data-stu-id="ab810-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ab810-147">请求</span><span class="sxs-lookup"><span data-stu-id="ab810-147">Request</span></span>

<span data-ttu-id="ab810-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ab810-148">The following is an example of the request.</span></span>


```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/authentication/methods
```

### <a name="response"></a><span data-ttu-id="ab810-149">响应</span><span class="sxs-lookup"><span data-stu-id="ab810-149">Response</span></span>

<span data-ttu-id="ab810-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ab810-150">The following is an example of the response.</span></span>

> <span data-ttu-id="ab810-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ab810-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.fido2AuthenticationMethod",
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
    "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
    "id": "b5e01f81-1f81-b5e0-811f-e0b5811fe0b5",
    "displayName": "Jordan's Surface Book",
    "createdDateTime": "2020-11-27T23:12:49Z",
    "keyStrength": "normal"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List methods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
