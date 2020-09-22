---
title: 获取 servicePrincipal
description: 检索 serviceprincipal 对象的属性和关系。
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 127549e24dc8b23de0812f0e08d8acb27f86d305
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010493"
---
# <a name="get-serviceprincipal"></a><span data-ttu-id="aed8e-103">获取 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="aed8e-103">Get servicePrincipal</span></span>

<span data-ttu-id="aed8e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aed8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aed8e-105">检索 [servicePrincipal](../resources/serviceprincipal.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aed8e-105">Retrieve the properties and relationships of a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aed8e-106">权限</span><span class="sxs-lookup"><span data-stu-id="aed8e-106">Permissions</span></span>
<span data-ttu-id="aed8e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aed8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="aed8e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="aed8e-109">Permission type</span></span>      | <span data-ttu-id="aed8e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aed8e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aed8e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aed8e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aed8e-112">Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aed8e-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aed8e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aed8e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aed8e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="aed8e-114">Not supported.</span></span>    |
|<span data-ttu-id="aed8e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="aed8e-115">Application</span></span> | <span data-ttu-id="aed8e-116">Application.Read.All、 Directory.Read.All、 Application.ReadWrite.OwnedBy、 Application.ReadWrite.All、 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aed8e-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aed8e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aed8e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aed8e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="aed8e-118">Optional query parameters</span></span>
<span data-ttu-id="aed8e-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="aed8e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aed8e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="aed8e-120">Request headers</span></span>
| <span data-ttu-id="aed8e-121">名称</span><span class="sxs-lookup"><span data-stu-id="aed8e-121">Name</span></span>           | <span data-ttu-id="aed8e-122">说明</span><span class="sxs-lookup"><span data-stu-id="aed8e-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="aed8e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aed8e-123">Authorization</span></span>  | <span data-ttu-id="aed8e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aed8e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aed8e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="aed8e-126">Request body</span></span>
<span data-ttu-id="aed8e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aed8e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aed8e-128">响应</span><span class="sxs-lookup"><span data-stu-id="aed8e-128">Response</span></span>
<span data-ttu-id="aed8e-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [servicePrincipal](../resources/serviceprincipal.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aed8e-129">If successful, this method returns a `200 OK` response code and a [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aed8e-130">示例</span><span class="sxs-lookup"><span data-stu-id="aed8e-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="aed8e-131">请求</span><span class="sxs-lookup"><span data-stu-id="aed8e-131">Request</span></span>
<span data-ttu-id="aed8e-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aed8e-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="aed8e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="aed8e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="aed8e-134">C#</span><span class="sxs-lookup"><span data-stu-id="aed8e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aed8e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aed8e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aed8e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aed8e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aed8e-137">响应</span><span class="sxs-lookup"><span data-stu-id="aed8e-137">Response</span></span>
<span data-ttu-id="aed8e-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="aed8e-138">Here is an example of the response.</span></span> 

><span data-ttu-id="aed8e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aed8e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
        "id": "59e617e5-e447-4adc-8b88-00af644d7c92",
        "deletedDateTime": null,
        "accountEnabled": true,
        "appDisplayName": "My App",
        "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
        "applicationTemplateId": null,
        "appOwnerOrganizationId": "1bc1c026-2f7b-48a5-98da-afa2fd8bc7bc",
        "appRoleAssignmentRequired": false,
        "displayName": "foo",
        "errorUrl": null,
        "homepage": null,
        "loginUrl": null,
        "logoutUrl": null,
        "notificationEmailAddresses": [],
        "preferredSingleSignOnMode": null,
        "preferredTokenSigningKeyEndDateTime": null,
        "preferredTokenSigningKeyThumbprint": null,
        "publisherName": "Contoso",
        "replyUrls": [],
        "samlMetadataUrl": null,
        "samlSingleSignOnSettings": null,
        "servicePrincipalNames": [
            "f1bd758f-4a1a-4b71-aa20-a248a22a8928"
        ],
        "signInAudience": "AzureADandPersonalMicrosoftAccount",
        "tags": [],
        "addIns": [],
        "api": {
            "resourceSpecificApplicationPermissions": []
        },
        "appRoles": [],
        "info": {
            "termsOfServiceUrl": null,
            "supportUrl": null,
            "privacyStatementUrl": null,
            "marketingUrl": null,
            "logoUrl": null
        },
        "keyCredentials": [],
        "publishedPermissionScopes": [],
        "passwordCredentials": []
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


