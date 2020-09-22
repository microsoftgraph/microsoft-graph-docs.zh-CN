---
title: List oauth2PermissionGrants
description: 检索 oAuth2PermissionGrant 对象的列表，表示委派的权限授予。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 679d65641a7b9295b06111148c43a12237123cc1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044520"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="1170e-103">List oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="1170e-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="1170e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1170e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1170e-105">检索 [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) 实体的列表，表示授予服务主体（代表客户端应用程序）以代表用户访问 API 的委派权限。</span><span class="sxs-lookup"><span data-stu-id="1170e-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) entities, representing delegated permissions granted to the service principal (representing the client application) to access an API on behalf of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="1170e-106">权限</span><span class="sxs-lookup"><span data-stu-id="1170e-106">Permissions</span></span>

<span data-ttu-id="1170e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1170e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1170e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1170e-109">Permission type</span></span>      | <span data-ttu-id="1170e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1170e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1170e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1170e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1170e-112">Directory.Read.All、DelegatedPermissionGrant.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1170e-112">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1170e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1170e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1170e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1170e-114">Not supported.</span></span>    |
|<span data-ttu-id="1170e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1170e-115">Application</span></span> | <span data-ttu-id="1170e-116">.Read.All、DelegatedPermissionGrant.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1170e-116">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1170e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1170e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1170e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1170e-118">Optional query parameters</span></span>

<span data-ttu-id="1170e-119">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1170e-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1170e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1170e-120">Request headers</span></span>

| <span data-ttu-id="1170e-121">名称</span><span class="sxs-lookup"><span data-stu-id="1170e-121">Name</span></span>           | <span data-ttu-id="1170e-122">说明</span><span class="sxs-lookup"><span data-stu-id="1170e-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="1170e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1170e-123">Authorization</span></span>  | <span data-ttu-id="1170e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1170e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1170e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1170e-126">Request body</span></span>

<span data-ttu-id="1170e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1170e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1170e-128">响应</span><span class="sxs-lookup"><span data-stu-id="1170e-128">Response</span></span>

<span data-ttu-id="1170e-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1170e-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1170e-130">示例</span><span class="sxs-lookup"><span data-stu-id="1170e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1170e-131">请求</span><span class="sxs-lookup"><span data-stu-id="1170e-131">Request</span></span>

<span data-ttu-id="1170e-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1170e-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1170e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1170e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_servicePrincipal_oAuth2PermissionGrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="1170e-134">C#</span><span class="sxs-lookup"><span data-stu-id="1170e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1170e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1170e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1170e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1170e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1170e-137">响应</span><span class="sxs-lookup"><span data-stu-id="1170e-137">Response</span></span>

<span data-ttu-id="1170e-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1170e-138">Here is an example of the response.</span></span> 

> <span data-ttu-id="1170e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1170e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "scope": "scope-value",
      "startTime": "datetime-value",
      "expiryTime": "datetime-value"
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


