---
title: 获取 oAuth2PermissionGrant
description: 检索单个 oAuth2PermissionGrant 的属性和关系，表示委派权限授予。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 4bcd823339b6f7c4c5ca0745d523ed27d820a67a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064750"
---
# <a name="get-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="a81c8-103">获取委派权限授予 (oAuth2PermissionGrant) </span><span class="sxs-lookup"><span data-stu-id="a81c8-103">Get a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="a81c8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a81c8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a81c8-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a81c8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a81c8-106">检索单个 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="a81c8-106">Retrieve the properties of a single [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="a81c8-107">**OAuth2PermissionGrant**表示已授予客户端应用程序代表登录用户访问 API 的委派权限。</span><span class="sxs-lookup"><span data-stu-id="a81c8-107">An **oAuth2PermissionGrant** represents delegated permissions which have been granted for a client application to access an API on behalf of a signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="a81c8-108">权限</span><span class="sxs-lookup"><span data-stu-id="a81c8-108">Permissions</span></span>

<span data-ttu-id="a81c8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a81c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a81c8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a81c8-111">Permission type</span></span>      | <span data-ttu-id="a81c8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a81c8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a81c8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a81c8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a81c8-114">"DelegatedPermissionGrant"、"全部"、"全部"、"Directory.accessasuser.all"、"全部"、"全部"、"directory"</span><span class="sxs-lookup"><span data-stu-id="a81c8-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a81c8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a81c8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a81c8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a81c8-116">Not supported.</span></span>    |
|<span data-ttu-id="a81c8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a81c8-117">Application</span></span> | <span data-ttu-id="a81c8-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a81c8-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a81c8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a81c8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a81c8-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a81c8-120">Optional query parameters</span></span>

<span data-ttu-id="a81c8-121">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a81c8-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a81c8-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a81c8-122">Request headers</span></span>

| <span data-ttu-id="a81c8-123">名称</span><span class="sxs-lookup"><span data-stu-id="a81c8-123">Name</span></span>       | <span data-ttu-id="a81c8-124">类型</span><span class="sxs-lookup"><span data-stu-id="a81c8-124">Type</span></span> | <span data-ttu-id="a81c8-125">说明</span><span class="sxs-lookup"><span data-stu-id="a81c8-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a81c8-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a81c8-126">Authorization</span></span>  | <span data-ttu-id="a81c8-127">string</span><span class="sxs-lookup"><span data-stu-id="a81c8-127">string</span></span>  | <span data-ttu-id="a81c8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a81c8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a81c8-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="a81c8-130">Request body</span></span>

<span data-ttu-id="a81c8-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a81c8-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a81c8-132">响应</span><span class="sxs-lookup"><span data-stu-id="a81c8-132">Response</span></span>

<span data-ttu-id="a81c8-133">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a81c8-133">If successful, this method returns a `200 OK` response code and [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a81c8-134">示例</span><span class="sxs-lookup"><span data-stu-id="a81c8-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="a81c8-135">请求</span><span class="sxs-lookup"><span data-stu-id="a81c8-135">Request</span></span>

<span data-ttu-id="a81c8-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a81c8-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a81c8-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="a81c8-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oAuth2PermissionGrant"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants/{id}
```

# <a name="c"></a>[<span data-ttu-id="a81c8-138">C#</span><span class="sxs-lookup"><span data-stu-id="a81c8-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a81c8-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a81c8-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a81c8-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a81c8-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a81c8-141">响应</span><span class="sxs-lookup"><span data-stu-id="a81c8-141">Response</span></span>

<span data-ttu-id="a81c8-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a81c8-142">Here is an example of the response.</span></span> 

> <span data-ttu-id="a81c8-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a81c8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 200

{
  "id": "id-value",
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "scope": "scope-value",
  "startTime": "2016-10-19T10:37:00Z",
  "expiryTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


