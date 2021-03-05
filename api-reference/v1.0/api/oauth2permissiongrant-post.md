---
title: 创建 oAuth2PermissionGrant
description: 创建一个 oAuth2PermissionGrant 对象，该对象代表委派的权限授予。
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: e893f69fba9e8494854cb89b030f75fe5b30dc8f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448198"
---
# <a name="create-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="ee805-103">通过 oAuth2PermissionGrant (创建委派) </span><span class="sxs-lookup"><span data-stu-id="ee805-103">Create a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="ee805-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee805-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="ee805-105">创建委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="ee805-105">Create a delegated permission grant.</span></span> <span data-ttu-id="ee805-106">委派的权限授予由 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象表示。</span><span class="sxs-lookup"><span data-stu-id="ee805-106">A delegated permission grant is represented by an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.</span></span>

<span data-ttu-id="ee805-107">委派权限授予授权客户端服务主体 (代表客户端应用程序) 访问代表 API) 的资源服务主体 (（代表已登录用户）访问已授予的委派权限限制的访问级别。</span><span class="sxs-lookup"><span data-stu-id="ee805-107">A delegated permission grant authorizes a client service principal (representing a client application) to access a resource service principal (representing an API), on behalf of a signed-in user, for the level of access limited by the delegated permissions which were granted.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee805-108">权限</span><span class="sxs-lookup"><span data-stu-id="ee805-108">Permissions</span></span>

<span data-ttu-id="ee805-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee805-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee805-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee805-111">Permission type</span></span>      | <span data-ttu-id="ee805-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ee805-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee805-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee805-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ee805-114">DelegatedPermissionGrant.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ee805-114">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ee805-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee805-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee805-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee805-116">Not supported.</span></span>    |
|<span data-ttu-id="ee805-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee805-117">Application</span></span> | <span data-ttu-id="ee805-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee805-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee805-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee805-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /oauth2PermissionGrants
```

## <a name="request-headers"></a><span data-ttu-id="ee805-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee805-120">Request headers</span></span>

| <span data-ttu-id="ee805-121">名称</span><span class="sxs-lookup"><span data-stu-id="ee805-121">Name</span></span>       | <span data-ttu-id="ee805-122">类型</span><span class="sxs-lookup"><span data-stu-id="ee805-122">Type</span></span> | <span data-ttu-id="ee805-123">说明</span><span class="sxs-lookup"><span data-stu-id="ee805-123">Description</span></span> |
|:-----------|:------|:----------|
| <span data-ttu-id="ee805-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee805-124">Authorization</span></span>  | <span data-ttu-id="ee805-125">string</span><span class="sxs-lookup"><span data-stu-id="ee805-125">string</span></span>  | <span data-ttu-id="ee805-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ee805-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee805-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee805-128">Request body</span></span>

<span data-ttu-id="ee805-129">在请求正文中，提供 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee805-129">In the request body, supply a JSON representation of an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ee805-130">响应</span><span class="sxs-lookup"><span data-stu-id="ee805-130">Response</span></span>

<span data-ttu-id="ee805-131">如果成功，此方法在响应正文中返回 200 系列响应代码和新的 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ee805-131">If successful, this method returns a 200-series response code and a new [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee805-132">示例</span><span class="sxs-lookup"><span data-stu-id="ee805-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee805-133">请求</span><span class="sxs-lookup"><span data-stu-id="ee805-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ee805-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee805-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_oAuth2PermissionGrant"
}-->

```http
POST https://graph.microsoft.com/v1.0/oauth2PermissionGrants
Content-Type: application/json
Content-Length: 30

{
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "scope": "scope-value"
}
```
# <a name="c"></a>[<span data-ttu-id="ee805-135">C#</span><span class="sxs-lookup"><span data-stu-id="ee805-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee805-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee805-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee805-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee805-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee805-138">Java</span><span class="sxs-lookup"><span data-stu-id="ee805-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ee805-139">响应</span><span class="sxs-lookup"><span data-stu-id="ee805-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

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
  "description": "Update oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

