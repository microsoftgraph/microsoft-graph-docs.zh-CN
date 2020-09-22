---
title: 获取 servicePrincipal
description: 检索 serviceprincipal 对象的属性和关系。
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e97a22030afcc7323333e9f2a8712c1887792d71
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032872"
---
# <a name="get-serviceprincipal"></a><span data-ttu-id="c61c3-103">获取 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="c61c3-103">Get servicePrincipal</span></span>

<span data-ttu-id="c61c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c61c3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c61c3-105">检索 [servicePrincipal](../resources/serviceprincipal.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c61c3-105">Retrieve the properties and relationships of a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c61c3-106">权限</span><span class="sxs-lookup"><span data-stu-id="c61c3-106">Permissions</span></span>
<span data-ttu-id="c61c3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c61c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c61c3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c61c3-109">Permission type</span></span>      | <span data-ttu-id="c61c3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c61c3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c61c3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c61c3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c61c3-112">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c61c3-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c61c3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c61c3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c61c3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c61c3-114">Not supported.</span></span>    |
|<span data-ttu-id="c61c3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c61c3-115">Application</span></span> | <span data-ttu-id="c61c3-116">Application.Read.All, Application.ReadWrite.All, Application.ReadWrite.OwnedBy, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c61c3-116">Application.Read.All, Application.ReadWrite.All, Application.ReadWrite.OwnedBy, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c61c3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c61c3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c61c3-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c61c3-118">Optional query parameters</span></span>
<span data-ttu-id="c61c3-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c61c3-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c61c3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c61c3-120">Request headers</span></span>
| <span data-ttu-id="c61c3-121">名称</span><span class="sxs-lookup"><span data-stu-id="c61c3-121">Name</span></span>           | <span data-ttu-id="c61c3-122">说明</span><span class="sxs-lookup"><span data-stu-id="c61c3-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="c61c3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c61c3-123">Authorization</span></span>  | <span data-ttu-id="c61c3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c61c3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c61c3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c61c3-126">Request body</span></span>
<span data-ttu-id="c61c3-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c61c3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c61c3-128">响应</span><span class="sxs-lookup"><span data-stu-id="c61c3-128">Response</span></span>
<span data-ttu-id="c61c3-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [servicePrincipal](../resources/serviceprincipal.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c61c3-129">If successful, this method returns a `200 OK` response code and a [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c61c3-130">示例</span><span class="sxs-lookup"><span data-stu-id="c61c3-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="c61c3-131">请求</span><span class="sxs-lookup"><span data-stu-id="c61c3-131">Request</span></span>
<span data-ttu-id="c61c3-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c61c3-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c61c3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c61c3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="c61c3-134">C#</span><span class="sxs-lookup"><span data-stu-id="c61c3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c61c3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c61c3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c61c3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c61c3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c61c3-137">Java</span><span class="sxs-lookup"><span data-stu-id="c61c3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c61c3-138">响应</span><span class="sxs-lookup"><span data-stu-id="c61c3-138">Response</span></span>
<span data-ttu-id="c61c3-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c61c3-139">Here is an example of the response.</span></span> 

><span data-ttu-id="c61c3-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c61c3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled": true,
  "addIns": [],
  "alternativeNames": ["http://contoso/a7770d29-4321-41a6-b863-ca11d6639448"],
  "appDisplayName": "My app",
  "appId": "appId-value",
  "appOwnerOrganizationId": "65415bb1-9267-4313-bbf5-ae259732ee12",
  "appRoleAssignmentRequired":true,
  "appRoles": [],
  "displayName": "My app instance in tenant",
  "endpoints": [],
  "homepage": null,
  "id": "00af5dfb-85da-4b41-a677-0c6b86dd34f8",
  "info": {
    "termsOfServiceUrl": null,
    "supportUrl": null,
    "privacyStatementUrl": null,
    "marketingUrl": null,
    "logoUrl": null
  },
  "keyCredentials": [],
  "logoutUrl": null,
  "oauth2PermissionScopes": [],
  "passwordCredentials": [],
  "publisherName": null,
  "replyUrls": [],
  "servicePrincipalNames": [],
  "servicePrincipalType": null,
  "tags": [],
  "tokenEncryptionKeyId": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

