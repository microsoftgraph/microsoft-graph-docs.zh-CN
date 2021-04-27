---
title: 获取 oAuth2PermissionGrant
description: 检索表示委派权限授予的单个 oAuth2PermissionGrant 的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 05a21be27e0df9c408134556b38aa509b1881350
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038360"
---
# <a name="get-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="53c62-103">获取 oAuth2PermissionGrant (委派) </span><span class="sxs-lookup"><span data-stu-id="53c62-103">Get a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="53c62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53c62-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="53c62-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53c62-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53c62-106">检索单个 [oAuth2PermissionGrant 的属性](../resources/oauth2permissiongrant.md)。</span><span class="sxs-lookup"><span data-stu-id="53c62-106">Retrieve the properties of a single [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="53c62-107">**oAuth2PermissionGrant** 表示已授予客户端应用程序代表已登录用户访问 API 的委派权限。</span><span class="sxs-lookup"><span data-stu-id="53c62-107">An **oAuth2PermissionGrant** represents delegated permissions which have been granted for a client application to access an API on behalf of a signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="53c62-108">权限</span><span class="sxs-lookup"><span data-stu-id="53c62-108">Permissions</span></span>

<span data-ttu-id="53c62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53c62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53c62-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="53c62-111">Permission type</span></span>      | <span data-ttu-id="53c62-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53c62-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53c62-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53c62-113">Delegated (work or school account)</span></span> | <span data-ttu-id="53c62-114">Directory.Read.All、DelegatedPermissionGrant.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="53c62-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="53c62-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53c62-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53c62-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="53c62-116">Not supported.</span></span>    |
|<span data-ttu-id="53c62-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="53c62-117">Application</span></span> | <span data-ttu-id="53c62-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53c62-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53c62-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53c62-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53c62-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="53c62-120">Optional query parameters</span></span>

<span data-ttu-id="53c62-121">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="53c62-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53c62-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="53c62-122">Request headers</span></span>

| <span data-ttu-id="53c62-123">名称</span><span class="sxs-lookup"><span data-stu-id="53c62-123">Name</span></span>       | <span data-ttu-id="53c62-124">类型</span><span class="sxs-lookup"><span data-stu-id="53c62-124">Type</span></span> | <span data-ttu-id="53c62-125">说明</span><span class="sxs-lookup"><span data-stu-id="53c62-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="53c62-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="53c62-126">Authorization</span></span>  | <span data-ttu-id="53c62-127">string</span><span class="sxs-lookup"><span data-stu-id="53c62-127">string</span></span>  | <span data-ttu-id="53c62-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53c62-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53c62-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="53c62-130">Request body</span></span>

<span data-ttu-id="53c62-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53c62-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53c62-132">响应</span><span class="sxs-lookup"><span data-stu-id="53c62-132">Response</span></span>

<span data-ttu-id="53c62-133">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53c62-133">If successful, this method returns a `200 OK` response code and [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53c62-134">示例</span><span class="sxs-lookup"><span data-stu-id="53c62-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="53c62-135">请求</span><span class="sxs-lookup"><span data-stu-id="53c62-135">Request</span></span>

<span data-ttu-id="53c62-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53c62-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="53c62-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="53c62-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oAuth2PermissionGrant"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants/{id}
```

# <a name="c"></a>[<span data-ttu-id="53c62-138">C#</span><span class="sxs-lookup"><span data-stu-id="53c62-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53c62-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53c62-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53c62-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53c62-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53c62-141">Java</span><span class="sxs-lookup"><span data-stu-id="53c62-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="53c62-142">响应</span><span class="sxs-lookup"><span data-stu-id="53c62-142">Response</span></span>

<span data-ttu-id="53c62-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="53c62-143">Here is an example of the response.</span></span> 

> <span data-ttu-id="53c62-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="53c62-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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


