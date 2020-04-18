---
title: List 方法
description: 检索身份验证方法对象的列表。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 633680aa09d262e9263f4b4afed55a89b2d64ab5
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557624"
---
# <a name="list-methods"></a><span data-ttu-id="a374f-103">List 方法</span><span class="sxs-lookup"><span data-stu-id="a374f-103">List methods</span></span>

<span data-ttu-id="a374f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a374f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a374f-105">检索[身份验证方法](../resources/authenticationmethod.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="a374f-105">Retrieve a list of [authentication method](../resources/authenticationmethod.md) objects.</span></span> <span data-ttu-id="a374f-106">目前仅返回[电话身份验证方法](../resources/phoneauthenticationmethod.md)和[密码身份验证方法](../resources/passwordauthenticationmethod.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a374f-106">Currently only [phone authentication method](../resources/phoneauthenticationmethod.md) and [password authentication method](../resources/passwordauthenticationmethod.md) objects are returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="a374f-107">权限</span><span class="sxs-lookup"><span data-stu-id="a374f-107">Permissions</span></span>

<span data-ttu-id="a374f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a374f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a374f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a374f-110">Permission type</span></span>                        | <span data-ttu-id="a374f-111">作用于自助的权限（从最高特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a374f-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="a374f-112">对其他用户的权限（从最低到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a374f-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="a374f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a374f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a374f-114">UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、UserAuthenticationMethod、All 和 All</span><span class="sxs-lookup"><span data-stu-id="a374f-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="a374f-115">UserAuthenticationMethod、UserAuthenticationMethod 和所有</span><span class="sxs-lookup"><span data-stu-id="a374f-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="a374f-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a374f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a374f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a374f-117">Not supported.</span></span> | <span data-ttu-id="a374f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a374f-118">Not supported.</span></span> |
| <span data-ttu-id="a374f-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="a374f-119">Application</span></span>                            | <span data-ttu-id="a374f-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="a374f-120">Not supported.</span></span> | <span data-ttu-id="a374f-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="a374f-121">Not supported.</span></span> |

<span data-ttu-id="a374f-122">对于在其他用户上执行管理的委派方案，管理员需要[以下角色之一](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="a374f-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="a374f-123">全局管理员</span><span class="sxs-lookup"><span data-stu-id="a374f-123">Global admin</span></span>
* <span data-ttu-id="a374f-124">全局读取者</span><span class="sxs-lookup"><span data-stu-id="a374f-124">Global reader</span></span>
* <span data-ttu-id="a374f-125">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="a374f-125">Privileged authentication admin</span></span>
* <span data-ttu-id="a374f-126">身份验证管理员（仅查看被屏蔽的电话号码）</span><span class="sxs-lookup"><span data-stu-id="a374f-126">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="a374f-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a374f-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods
GET /users/{id}/authentication/methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a374f-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a374f-128">Optional query parameters</span></span>

<span data-ttu-id="a374f-129">此方法不支持用于自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="a374f-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a374f-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="a374f-130">Request headers</span></span>

| <span data-ttu-id="a374f-131">名称</span><span class="sxs-lookup"><span data-stu-id="a374f-131">Name</span></span>      |<span data-ttu-id="a374f-132">说明</span><span class="sxs-lookup"><span data-stu-id="a374f-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a374f-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="a374f-133">Authorization</span></span> | <span data-ttu-id="a374f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a374f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a374f-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="a374f-136">Request body</span></span>

<span data-ttu-id="a374f-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a374f-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a374f-138">响应</span><span class="sxs-lookup"><span data-stu-id="a374f-138">Response</span></span>

<span data-ttu-id="a374f-139">如果成功，此方法在响应`200 OK`正文中返回响应代码和[authenticationMethod](../resources/authenticationmethod.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="a374f-139">If successful, this method returns a `200 OK` response code and a collection of [authenticationMethod](../resources/authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a374f-140">示例</span><span class="sxs-lookup"><span data-stu-id="a374f-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a374f-141">请求</span><span class="sxs-lookup"><span data-stu-id="a374f-141">Request</span></span>

<span data-ttu-id="a374f-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a374f-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_methods"
}-->

```http
GET https://graph.microsoft.com/beta/me/authentication/methods
```

### <a name="response"></a><span data-ttu-id="a374f-143">响应</span><span class="sxs-lookup"><span data-stu-id="a374f-143">Response</span></span>

<span data-ttu-id="a374f-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a374f-144">The following is an example of the response.</span></span>

> <span data-ttu-id="a374f-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a374f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "odata.type": "#microsoft.graph.passwordAuthenticationMethod",
      "id": "28c10230-6103-485e-b985-444c60001490",
      "password": null,
      "creationDateTime": null
    },
    {
      "odata.type": "#microsoft.graph.phoneAuthenticationMethod",
      "id": "3179e48a-750b-4051-897c-87b9720928f7",
      "phoneNumber": "+1 2065555555",
      "authenticationPhoneType": "mobile",
      "smsSignInState": "ready"
    },
    {
      "odata.type": "#microsoft.graph.phoneAuthenticationMethod",
      "id": "b6332ec1-7057-4abe-9331-3d72feddfe41",
      "phoneNumber": "+1 2065555556",
      "authenticationPhoneType": "alternateMobile",
      "smsSignInState": "notSupported"
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
