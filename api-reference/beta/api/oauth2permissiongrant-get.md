---
title: 获取 oAuth2PermissionGrant
description: 检索表示委派权限授予的单个 oAuth2PermissionGrant 的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 4919e2e664ba3af1d3b74c8af9f7f5047c915a16
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442370"
---
# <a name="get-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="9d1ca-103">获取 oAuth2PermissionGrant (委派) </span><span class="sxs-lookup"><span data-stu-id="9d1ca-103">Get a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="9d1ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d1ca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d1ca-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d1ca-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d1ca-106">检索单个 [oAuth2PermissionGrant 的属性](../resources/oauth2permissiongrant.md)。</span><span class="sxs-lookup"><span data-stu-id="9d1ca-106">Retrieve the properties of a single [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="9d1ca-107">**oAuth2PermissionGrant** 表示已授予客户端应用程序代表登录用户访问 API 的委派权限。</span><span class="sxs-lookup"><span data-stu-id="9d1ca-107">An **oAuth2PermissionGrant** represents delegated permissions which have been granted for a client application to access an API on behalf of a signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d1ca-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="9d1ca-108">Permissions</span></span>

<span data-ttu-id="9d1ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d1ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d1ca-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d1ca-111">Permission type</span></span>      | <span data-ttu-id="9d1ca-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9d1ca-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d1ca-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d1ca-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9d1ca-114">Directory.Read.All、DelegatedPermissionGrant.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9d1ca-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9d1ca-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d1ca-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d1ca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d1ca-116">Not supported.</span></span>    |
|<span data-ttu-id="9d1ca-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d1ca-117">Application</span></span> | <span data-ttu-id="9d1ca-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d1ca-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d1ca-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d1ca-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9d1ca-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9d1ca-120">Optional query parameters</span></span>

<span data-ttu-id="9d1ca-121">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9d1ca-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d1ca-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d1ca-122">Request headers</span></span>

| <span data-ttu-id="9d1ca-123">名称</span><span class="sxs-lookup"><span data-stu-id="9d1ca-123">Name</span></span>       | <span data-ttu-id="9d1ca-124">类型</span><span class="sxs-lookup"><span data-stu-id="9d1ca-124">Type</span></span> | <span data-ttu-id="9d1ca-125">说明</span><span class="sxs-lookup"><span data-stu-id="9d1ca-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9d1ca-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d1ca-126">Authorization</span></span>  | <span data-ttu-id="9d1ca-127">string</span><span class="sxs-lookup"><span data-stu-id="9d1ca-127">string</span></span>  | <span data-ttu-id="9d1ca-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9d1ca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d1ca-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d1ca-130">Request body</span></span>

<span data-ttu-id="9d1ca-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9d1ca-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d1ca-132">响应</span><span class="sxs-lookup"><span data-stu-id="9d1ca-132">Response</span></span>

<span data-ttu-id="9d1ca-133">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9d1ca-133">If successful, this method returns a `200 OK` response code and [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d1ca-134">示例</span><span class="sxs-lookup"><span data-stu-id="9d1ca-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d1ca-135">请求</span><span class="sxs-lookup"><span data-stu-id="9d1ca-135">Request</span></span>

<span data-ttu-id="9d1ca-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9d1ca-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9d1ca-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d1ca-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oAuth2PermissionGrant"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants/{id}
```

# <a name="c"></a>[<span data-ttu-id="9d1ca-138">C#</span><span class="sxs-lookup"><span data-stu-id="9d1ca-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d1ca-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d1ca-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d1ca-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d1ca-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d1ca-141">Java</span><span class="sxs-lookup"><span data-stu-id="9d1ca-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="9d1ca-142">响应</span><span class="sxs-lookup"><span data-stu-id="9d1ca-142">Response</span></span>

<span data-ttu-id="9d1ca-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9d1ca-143">Here is an example of the response.</span></span> 

> <span data-ttu-id="9d1ca-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9d1ca-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


