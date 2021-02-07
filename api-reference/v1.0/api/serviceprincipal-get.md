---
title: 获取 servicePrincipal
description: 检索 serviceprincipal 对象的属性和关系。
author: sureshja
localization_priority: Priority
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: c82d15a61ac8c845608268e2fcdef804064fa80c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134601"
---
# <a name="get-serviceprincipal"></a><span data-ttu-id="99df1-103">获取 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="99df1-103">Get servicePrincipal</span></span>

<span data-ttu-id="99df1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99df1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="99df1-105">检索 [servicePrincipal](../resources/serviceprincipal.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="99df1-105">Retrieve the properties and relationships of a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="99df1-106">权限</span><span class="sxs-lookup"><span data-stu-id="99df1-106">Permissions</span></span>
<span data-ttu-id="99df1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99df1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99df1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="99df1-109">Permission type</span></span>      | <span data-ttu-id="99df1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99df1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99df1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99df1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="99df1-112">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="99df1-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="99df1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99df1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99df1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="99df1-114">Not supported.</span></span>    |
|<span data-ttu-id="99df1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="99df1-115">Application</span></span> | <span data-ttu-id="99df1-116">Application.Read.All, Application.ReadWrite.All, Application.ReadWrite.OwnedBy, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="99df1-116">Application.Read.All, Application.ReadWrite.All, Application.ReadWrite.OwnedBy, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="99df1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99df1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="99df1-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="99df1-118">Optional query parameters</span></span>
<span data-ttu-id="99df1-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="99df1-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="99df1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="99df1-120">Request headers</span></span>
| <span data-ttu-id="99df1-121">名称</span><span class="sxs-lookup"><span data-stu-id="99df1-121">Name</span></span>           | <span data-ttu-id="99df1-122">说明</span><span class="sxs-lookup"><span data-stu-id="99df1-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="99df1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="99df1-123">Authorization</span></span>  | <span data-ttu-id="99df1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="99df1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="99df1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="99df1-126">Request body</span></span>
<span data-ttu-id="99df1-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="99df1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99df1-128">响应</span><span class="sxs-lookup"><span data-stu-id="99df1-128">Response</span></span>
<span data-ttu-id="99df1-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [servicePrincipal](../resources/serviceprincipal.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="99df1-129">If successful, this method returns a `200 OK` response code and a [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="99df1-130">示例</span><span class="sxs-lookup"><span data-stu-id="99df1-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="99df1-131">请求</span><span class="sxs-lookup"><span data-stu-id="99df1-131">Request</span></span>
<span data-ttu-id="99df1-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="99df1-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="99df1-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="99df1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="99df1-134">C#</span><span class="sxs-lookup"><span data-stu-id="99df1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99df1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99df1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99df1-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99df1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99df1-137">Java</span><span class="sxs-lookup"><span data-stu-id="99df1-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="99df1-138">响应</span><span class="sxs-lookup"><span data-stu-id="99df1-138">Response</span></span>
<span data-ttu-id="99df1-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="99df1-139">Here is an example of the response.</span></span> 

><span data-ttu-id="99df1-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="99df1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
