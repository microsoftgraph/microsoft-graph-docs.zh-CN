---
title: 获取 authenticationMethod
description: 检索 authenticationMethod 对象的属性和关系。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 95ab608e5b1c384e4ddffc2c2e252d473f9aa2af
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469085"
---
# <a name="get-authenticationmethod"></a><span data-ttu-id="002a2-103">获取 authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="002a2-103">Get authenticationMethod</span></span>

<span data-ttu-id="002a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="002a2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="002a2-105">检索 [authenticationMethod 对象的属性和](../resources/authenticationmethod.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="002a2-105">Retrieve the properties and relationships of an [authenticationMethod](../resources/authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="002a2-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="002a2-106">Permissions</span></span>

<span data-ttu-id="002a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="002a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="002a2-109">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="002a2-109">Permissions acting on self</span></span>

|<span data-ttu-id="002a2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="002a2-110">Permission type</span></span>      | <span data-ttu-id="002a2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="002a2-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="002a2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="002a2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="002a2-113">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="002a2-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="002a2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="002a2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="002a2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="002a2-115">Not supported.</span></span> |
| <span data-ttu-id="002a2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="002a2-116">Application</span></span>                            | <span data-ttu-id="002a2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="002a2-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="002a2-118">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="002a2-118">Permissions acting on other users</span></span>

|<span data-ttu-id="002a2-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="002a2-119">Permission type</span></span>      | <span data-ttu-id="002a2-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="002a2-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="002a2-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="002a2-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="002a2-122">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="002a2-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="002a2-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="002a2-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="002a2-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="002a2-124">Not supported.</span></span> |
| <span data-ttu-id="002a2-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="002a2-125">Application</span></span>                            | <span data-ttu-id="002a2-126">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="002a2-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="002a2-127">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="002a2-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="002a2-128">全局管理员</span><span class="sxs-lookup"><span data-stu-id="002a2-128">Global admin</span></span>
* <span data-ttu-id="002a2-129">全局读取者</span><span class="sxs-lookup"><span data-stu-id="002a2-129">Global reader</span></span>
* <span data-ttu-id="002a2-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="002a2-130">Privileged authentication admin</span></span>
* <span data-ttu-id="002a2-131">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="002a2-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="002a2-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="002a2-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods/{id}
GET /users/{id | userPrincipalName}/authentication/methods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="002a2-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="002a2-133">Optional query parameters</span></span>

<span data-ttu-id="002a2-134">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="002a2-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="002a2-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="002a2-135">Request headers</span></span>

| <span data-ttu-id="002a2-136">名称</span><span class="sxs-lookup"><span data-stu-id="002a2-136">Name</span></span>      |<span data-ttu-id="002a2-137">说明</span><span class="sxs-lookup"><span data-stu-id="002a2-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="002a2-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="002a2-138">Authorization</span></span> | <span data-ttu-id="002a2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="002a2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="002a2-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="002a2-141">Request body</span></span>

<span data-ttu-id="002a2-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="002a2-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="002a2-143">响应</span><span class="sxs-lookup"><span data-stu-id="002a2-143">Response</span></span>

<span data-ttu-id="002a2-144">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [authenticationMethod](../resources/authenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="002a2-144">If successful, this method returns a `200 OK` response code and the requested [authenticationMethod](../resources/authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="002a2-145">示例</span><span class="sxs-lookup"><span data-stu-id="002a2-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="002a2-146">请求</span><span class="sxs-lookup"><span data-stu-id="002a2-146">Request</span></span>

<span data-ttu-id="002a2-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="002a2-147">The following is an example of the request.</span></span>


```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/authentication/methods/{id}
```

### <a name="response"></a><span data-ttu-id="002a2-148">响应</span><span class="sxs-lookup"><span data-stu-id="002a2-148">Response</span></span>

<span data-ttu-id="002a2-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="002a2-149">The following is an example of the response.</span></span>

> <span data-ttu-id="002a2-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="002a2-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
    "id": "b5e01f81-1f81-b5e0-811f-e0b5811fe0b5",
    "displayName": "Jordan's Surface Book",
    "createdDateTime": "2020-11-27T23:12:49Z",
    "keyStrength": "normal"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get authenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
