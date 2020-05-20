---
title: 获取 oAuth2PermissionGrant
description: 检索单个 oAuth2PermissionGrant 的属性和关系，表示委派权限授予。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: a4e6626bef1969822954ddb889e33526cd09604f
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288706"
---
# <a name="get-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="afa33-103">获取委派权限授予（oAuth2PermissionGrant）</span><span class="sxs-lookup"><span data-stu-id="afa33-103">Get a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="afa33-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afa33-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="afa33-105">检索单个[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="afa33-105">Retrieve the properties of a single [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="afa33-106">**OAuth2PermissionGrant**表示已授予客户端应用程序代表登录用户访问 API 的委派权限。</span><span class="sxs-lookup"><span data-stu-id="afa33-106">An **oAuth2PermissionGrant** represents delegated permissions which have been granted for a client application to access an API on behalf of a signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="afa33-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="afa33-107">Permissions</span></span>

<span data-ttu-id="afa33-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="afa33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afa33-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="afa33-110">Permission type</span></span>      | <span data-ttu-id="afa33-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="afa33-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afa33-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="afa33-112">Delegated (work or school account)</span></span> | <span data-ttu-id="afa33-113">"DelegatedPermissionGrant"、"全部"、"全部"、"Directory.accessasuser.all"、"全部"、"全部"、"directory"</span><span class="sxs-lookup"><span data-stu-id="afa33-113">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="afa33-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="afa33-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afa33-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="afa33-115">Not supported.</span></span>    |
|<span data-ttu-id="afa33-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="afa33-116">Application</span></span> | <span data-ttu-id="afa33-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afa33-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="afa33-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="afa33-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="afa33-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="afa33-119">Optional query parameters</span></span>

<span data-ttu-id="afa33-120">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="afa33-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="afa33-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="afa33-121">Request headers</span></span>

| <span data-ttu-id="afa33-122">名称</span><span class="sxs-lookup"><span data-stu-id="afa33-122">Name</span></span>       | <span data-ttu-id="afa33-123">类型</span><span class="sxs-lookup"><span data-stu-id="afa33-123">Type</span></span> | <span data-ttu-id="afa33-124">说明</span><span class="sxs-lookup"><span data-stu-id="afa33-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="afa33-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="afa33-125">Authorization</span></span>  | <span data-ttu-id="afa33-126">string</span><span class="sxs-lookup"><span data-stu-id="afa33-126">string</span></span>  | <span data-ttu-id="afa33-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="afa33-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="afa33-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="afa33-129">Request body</span></span>

<span data-ttu-id="afa33-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="afa33-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afa33-131">响应</span><span class="sxs-lookup"><span data-stu-id="afa33-131">Response</span></span>

<span data-ttu-id="afa33-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)对象。</span><span class="sxs-lookup"><span data-stu-id="afa33-132">If successful, this method returns a `200 OK` response code and [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afa33-133">示例</span><span class="sxs-lookup"><span data-stu-id="afa33-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="afa33-134">请求</span><span class="sxs-lookup"><span data-stu-id="afa33-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrant"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/oauth2PermissionGrants/{id}
```

### <a name="response"></a><span data-ttu-id="afa33-135">响应</span><span class="sxs-lookup"><span data-stu-id="afa33-135">Response</span></span>

> <span data-ttu-id="afa33-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="afa33-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
