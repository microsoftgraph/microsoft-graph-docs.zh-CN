---
title: 创建 oAuth2PermissionGrant
description: 创建一个代表委派权限授予的 oAuth2PermissionGrant 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 475a1f2d05a21ed327cb8026e94bdf5d3e51419a
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289827"
---
# <a name="create-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="969ad-103">创建委派权限授予（oAuth2PermissionGrant）</span><span class="sxs-lookup"><span data-stu-id="969ad-103">Create a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="969ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="969ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="969ad-105">创建委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="969ad-105">Create a delegated permission grant.</span></span> <span data-ttu-id="969ad-106">委派权限授予由[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)对象表示。</span><span class="sxs-lookup"><span data-stu-id="969ad-106">A delegated permission grant is represented by an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.</span></span>

<span data-ttu-id="969ad-107">委派权限授予授予客户端服务主体（表示客户端应用程序），以代表登录用户访问受委派权限限制的访问权限级别的客户端服务主体（表示一个 API）。</span><span class="sxs-lookup"><span data-stu-id="969ad-107">A delegated permission grant authorizes a client service principal (representing a client application) to access a resource service principal (representing an API), on behalf of a signed-in user, for the level of access limited by the delegated permissions which were granted.</span></span>

## <a name="permissions"></a><span data-ttu-id="969ad-108">权限</span><span class="sxs-lookup"><span data-stu-id="969ad-108">Permissions</span></span>

<span data-ttu-id="969ad-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="969ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="969ad-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="969ad-111">Permission type</span></span>      | <span data-ttu-id="969ad-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="969ad-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="969ad-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="969ad-113">Delegated (work or school account)</span></span> | <span data-ttu-id="969ad-114">DelegatedPermissionGrant、Directory.accessasuser.all、all 和的所有子目录</span><span class="sxs-lookup"><span data-stu-id="969ad-114">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="969ad-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="969ad-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="969ad-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="969ad-116">Not supported.</span></span>    |
|<span data-ttu-id="969ad-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="969ad-117">Application</span></span> | <span data-ttu-id="969ad-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="969ad-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="969ad-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="969ad-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /oauth2PermissionGrants
```

## <a name="request-headers"></a><span data-ttu-id="969ad-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="969ad-120">Request headers</span></span>

| <span data-ttu-id="969ad-121">名称</span><span class="sxs-lookup"><span data-stu-id="969ad-121">Name</span></span>       | <span data-ttu-id="969ad-122">类型</span><span class="sxs-lookup"><span data-stu-id="969ad-122">Type</span></span> | <span data-ttu-id="969ad-123">说明</span><span class="sxs-lookup"><span data-stu-id="969ad-123">Description</span></span> |
|:-----------|:------|:----------|
| <span data-ttu-id="969ad-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="969ad-124">Authorization</span></span>  | <span data-ttu-id="969ad-125">string</span><span class="sxs-lookup"><span data-stu-id="969ad-125">string</span></span>  | <span data-ttu-id="969ad-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="969ad-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="969ad-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="969ad-128">Request body</span></span>

<span data-ttu-id="969ad-129">在请求正文中，提供[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="969ad-129">In the request body, supply a JSON representation of an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="969ad-130">响应</span><span class="sxs-lookup"><span data-stu-id="969ad-130">Response</span></span>

<span data-ttu-id="969ad-131">如果成功，此方法在响应正文中返回一个200系列响应代码和一个新的[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)对象。</span><span class="sxs-lookup"><span data-stu-id="969ad-131">If successful, this method returns a 200-series response code and a new [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="969ad-132">示例</span><span class="sxs-lookup"><span data-stu-id="969ad-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="969ad-133">请求</span><span class="sxs-lookup"><span data-stu-id="969ad-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="969ad-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="969ad-134">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "post_oAuth2PermissionGrant"
}-->

```http
POST https://graph.microsoft.com/beta/oauth2PermissionGrants
Content-Type: application/json
Content-Length: 30

{
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "scope": "scope-value",
  "startTime": "2016-10-19T10:37:00Z",
  "expiryTime": "2016-10-19T10:37:00Z"
}
```

### <a name="response"></a><span data-ttu-id="969ad-135">响应</span><span class="sxs-lookup"><span data-stu-id="969ad-135">Response</span></span>

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
  "description": "Update oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
