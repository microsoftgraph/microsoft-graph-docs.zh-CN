---
title: List oauth2PermissionGrants
description: 检索 oAuth2PermissionGrant 对象的列表，表示委派权限授予。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 707a8d793f3bbf4cd58f8d68409d698622967c0f
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291109"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="cfafe-103">List oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="cfafe-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="cfafe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfafe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cfafe-105">检索[oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md)实体列表，这些实体代表用户授予的对服务主体（表示客户端应用程序）访问 API 的委派权限。</span><span class="sxs-lookup"><span data-stu-id="cfafe-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) entities, representing delegated permissions granted to the service principal (representing the client application) to access an API on behalf of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfafe-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="cfafe-106">Permissions</span></span>

<span data-ttu-id="cfafe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cfafe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfafe-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cfafe-109">Permission type</span></span>      | <span data-ttu-id="cfafe-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cfafe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfafe-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cfafe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cfafe-112">"DelegatedPermissionGrant"、"全部"、"全部"、"Directory.accessasuser.all"、"全部"、"全部"、"directory"</span><span class="sxs-lookup"><span data-stu-id="cfafe-112">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cfafe-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cfafe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfafe-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfafe-114">Not supported.</span></span>    |
|<span data-ttu-id="cfafe-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cfafe-115">Application</span></span> | <span data-ttu-id="cfafe-116">"DelegatedPermissionGrant"、"全部"、"全部"、"全部"、"全部"、"目录"</span><span class="sxs-lookup"><span data-stu-id="cfafe-116">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfafe-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cfafe-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cfafe-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cfafe-118">Optional query parameters</span></span>

<span data-ttu-id="cfafe-119">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cfafe-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cfafe-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cfafe-120">Request headers</span></span>

| <span data-ttu-id="cfafe-121">名称</span><span class="sxs-lookup"><span data-stu-id="cfafe-121">Name</span></span>           | <span data-ttu-id="cfafe-122">说明</span><span class="sxs-lookup"><span data-stu-id="cfafe-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="cfafe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfafe-123">Authorization</span></span>  | <span data-ttu-id="cfafe-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cfafe-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cfafe-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cfafe-126">Request body</span></span>

<span data-ttu-id="cfafe-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cfafe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfafe-128">响应</span><span class="sxs-lookup"><span data-stu-id="cfafe-128">Response</span></span>

<span data-ttu-id="cfafe-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="cfafe-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cfafe-130">示例</span><span class="sxs-lookup"><span data-stu-id="cfafe-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cfafe-131">请求</span><span class="sxs-lookup"><span data-stu-id="cfafe-131">Request</span></span>

<span data-ttu-id="cfafe-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cfafe-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_servicePrincipal_oAuth2PermissionGrants"
}-->

```http
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/oauth2PermissionGrants
```

### <a name="response"></a><span data-ttu-id="cfafe-133">响应</span><span class="sxs-lookup"><span data-stu-id="cfafe-133">Response</span></span>

<span data-ttu-id="cfafe-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cfafe-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="cfafe-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cfafe-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 253

{
  "value": [
    {
      "id": "id-value",
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oAuth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
