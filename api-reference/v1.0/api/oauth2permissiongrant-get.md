---
title: 获取 oAuth2PermissionGrant
description: 检索表示委派权限授予的单个 oAuth2PermissionGrant 的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 86e1bd2bbf03ac9304082bee44e5ed6e46ff00fd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039326"
---
# <a name="get-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="219fc-103">获取 oAuth2PermissionGrant (委派) </span><span class="sxs-lookup"><span data-stu-id="219fc-103">Get a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="219fc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="219fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="219fc-105">检索单个 [oAuth2PermissionGrant 的属性](../resources/oauth2permissiongrant.md)。</span><span class="sxs-lookup"><span data-stu-id="219fc-105">Retrieve the properties of a single [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="219fc-106">**oAuth2PermissionGrant** 表示已授予客户端应用程序代表已登录用户访问 API 的委派权限。</span><span class="sxs-lookup"><span data-stu-id="219fc-106">An **oAuth2PermissionGrant** represents delegated permissions which have been granted for a client application to access an API on behalf of a signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="219fc-107">权限</span><span class="sxs-lookup"><span data-stu-id="219fc-107">Permissions</span></span>

<span data-ttu-id="219fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="219fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="219fc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="219fc-110">Permission type</span></span>      | <span data-ttu-id="219fc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="219fc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="219fc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="219fc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="219fc-113">Directory.Read.All、DelegatedPermissionGrant.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="219fc-113">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="219fc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="219fc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="219fc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="219fc-115">Not supported.</span></span>    |
|<span data-ttu-id="219fc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="219fc-116">Application</span></span> | <span data-ttu-id="219fc-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="219fc-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="219fc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="219fc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="219fc-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="219fc-119">Optional query parameters</span></span>

<span data-ttu-id="219fc-120">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="219fc-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="219fc-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="219fc-121">Request headers</span></span>

| <span data-ttu-id="219fc-122">名称</span><span class="sxs-lookup"><span data-stu-id="219fc-122">Name</span></span>       | <span data-ttu-id="219fc-123">类型</span><span class="sxs-lookup"><span data-stu-id="219fc-123">Type</span></span> | <span data-ttu-id="219fc-124">说明</span><span class="sxs-lookup"><span data-stu-id="219fc-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="219fc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="219fc-125">Authorization</span></span>  | <span data-ttu-id="219fc-126">string</span><span class="sxs-lookup"><span data-stu-id="219fc-126">string</span></span>  | <span data-ttu-id="219fc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="219fc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="219fc-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="219fc-129">Request body</span></span>

<span data-ttu-id="219fc-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="219fc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="219fc-131">响应</span><span class="sxs-lookup"><span data-stu-id="219fc-131">Response</span></span>

<span data-ttu-id="219fc-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="219fc-132">If successful, this method returns a `200 OK` response code and [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="219fc-133">示例</span><span class="sxs-lookup"><span data-stu-id="219fc-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="219fc-134">请求</span><span class="sxs-lookup"><span data-stu-id="219fc-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="219fc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="219fc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrant"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/oauth2PermissionGrants/{id}
```
# <a name="c"></a>[<span data-ttu-id="219fc-136">C#</span><span class="sxs-lookup"><span data-stu-id="219fc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="219fc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="219fc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="219fc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="219fc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="219fc-139">Java</span><span class="sxs-lookup"><span data-stu-id="219fc-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="219fc-140">响应</span><span class="sxs-lookup"><span data-stu-id="219fc-140">Response</span></span>

> <span data-ttu-id="219fc-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="219fc-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "scope": "scope-value"
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

