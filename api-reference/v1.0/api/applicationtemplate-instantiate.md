---
title: applicationTemplate：实例化
description: 将 Azure AD 应用程序库中的应用程序实例添加到目录中。
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 34fe3ae80b34497cfe3313031cd1d3e2f5f7a91c
ms.sourcegitcommit: be09568fa07ab793cd1db500f537ca94ca9e5b4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836961"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="9b995-103">applicationTemplate：实例化</span><span class="sxs-lookup"><span data-stu-id="9b995-103">applicationTemplate: instantiate</span></span>

<span data-ttu-id="9b995-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b995-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9b995-105">将 Azure AD 应用程序库中的应用程序实例添加到目录中。</span><span class="sxs-lookup"><span data-stu-id="9b995-105">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b995-106">权限</span><span class="sxs-lookup"><span data-stu-id="9b995-106">Permissions</span></span>

<span data-ttu-id="9b995-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b995-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b995-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b995-109">Permission type</span></span>                        | <span data-ttu-id="9b995-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9b995-110">Permissions (from least to most privileged)</span></span>        |
| :------------------------------------- | :------------------------------------------------- |
| <span data-ttu-id="9b995-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b995-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b995-112">Application.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b995-112">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="9b995-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b995-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b995-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b995-114">Not supported.</span></span>                                     |
| <span data-ttu-id="9b995-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b995-115">Application</span></span>                            | <span data-ttu-id="9b995-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b995-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b995-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b995-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="9b995-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b995-118">Request headers</span></span>

| <span data-ttu-id="9b995-119">名称</span><span class="sxs-lookup"><span data-stu-id="9b995-119">Name</span></span>          | <span data-ttu-id="9b995-120">说明</span><span class="sxs-lookup"><span data-stu-id="9b995-120">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="9b995-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b995-121">Authorization</span></span> | <span data-ttu-id="9b995-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9b995-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b995-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b995-123">Request body</span></span>

<span data-ttu-id="9b995-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9b995-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9b995-125">参数</span><span class="sxs-lookup"><span data-stu-id="9b995-125">Parameter</span></span>   | <span data-ttu-id="9b995-126">类型</span><span class="sxs-lookup"><span data-stu-id="9b995-126">Type</span></span>   | <span data-ttu-id="9b995-127">说明</span><span class="sxs-lookup"><span data-stu-id="9b995-127">Description</span></span>                    |
| :---------- | :----- | :----------------------------- |
| <span data-ttu-id="9b995-128">displayName</span><span class="sxs-lookup"><span data-stu-id="9b995-128">displayName</span></span> | <span data-ttu-id="9b995-129">String</span><span class="sxs-lookup"><span data-stu-id="9b995-129">String</span></span> | <span data-ttu-id="9b995-130">应用程序的自定义名称</span><span class="sxs-lookup"><span data-stu-id="9b995-130">Custom name of the application</span></span> |

## <a name="response"></a><span data-ttu-id="9b995-131">响应</span><span class="sxs-lookup"><span data-stu-id="9b995-131">Response</span></span>

<span data-ttu-id="9b995-132">如果成功，此方法在响应正文中返回 响应代码和新的 `201 OK` [applicationServicePrincipal](../resources/applicationserviceprincipal.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9b995-132">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9b995-133">示例</span><span class="sxs-lookup"><span data-stu-id="9b995-133">Examples</span></span>

<span data-ttu-id="9b995-134">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="9b995-134">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="9b995-135">请求</span><span class="sxs-lookup"><span data-stu-id="9b995-135">Request</span></span>

<span data-ttu-id="9b995-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9b995-136">The following is an example of the request.</span></span>

> <span data-ttu-id="9b995-137">可以使用此 API 实例化 [非库应用](/azure/active-directory/manage-apps/add-non-gallery-app)。</span><span class="sxs-lookup"><span data-stu-id="9b995-137">You can use this API to instantiate [non-gallery apps](/azure/active-directory/manage-apps/add-non-gallery-app).</span></span> <span data-ttu-id="9b995-138">对 **applicationTemplate** 使用以下 `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` ID：。</span><span class="sxs-lookup"><span data-stu-id="9b995-138">Use the following ID for **applicationTemplate**: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>


# <a name="http"></a>[<span data-ttu-id="9b995-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b995-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```http
POST https://graph.microsoft.com/v1.0/applicationTemplates/{id}/instantiate
Content-type: application/json

{
  "displayName": "My custom name"
}
```
# <a name="c"></a>[<span data-ttu-id="9b995-140">C#</span><span class="sxs-lookup"><span data-stu-id="9b995-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b995-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b995-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b995-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b995-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9b995-143">Java</span><span class="sxs-lookup"><span data-stu-id="9b995-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/applicationtemplate-instantiate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9b995-144">响应</span><span class="sxs-lookup"><span data-stu-id="9b995-144">Response</span></span>

<span data-ttu-id="9b995-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9b995-145">The following is an example of the response.</span></span>

> <span data-ttu-id="9b995-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9b995-146">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
} -->

```http
HTTP/1.1 201 OK
Content-type: application/json

{
   "servicePrincipal":{
      "accountEnabled":true,
      "addIns":[],
      "alternativeNames":[
         "http://contoso/a7770d29-4321-41a6-b863-ca11d6639448"
      ],
      "appDisplayName":"appDisplayName-value",
      "appId":"appId-value",
      "appOwnerOrganizationId":"appOwnerOrganizationId-value",
      "appRoleAssignmentRequired":true,
      "appRoles":[],
      "displayName":"Display name",
      "endpoints":[],
      "homepage":null,
      "id":"id-value",
      "info":{
         "termsOfServiceUrl":null,
         "supportUrl":null,
         "privacyStatementUrl":null,
         "marketingUrl":null,
         "logoUrl":null
      },
      "keyCredentials":[],
      "logoutUrl":null,
      "oauth2PermissionScopes":[],
      "passwordCredentials":[],
      "publisherName":null,
      "replyUrls":[],
      "servicePrincipalNames":[],
      "servicePrincipalType":null,
      "tags":[],
      "tokenEncryptionKeyId":null
   },
   "application":{
      "id":"id-value",
      "isFallbackPublicClient":null,
      "appId":"appId-value",
      "applicationTemplateId":null,
      "identifierUris":[],
      "createdDateTime":"2019-09-17T19:10:35.2742618Z",
      "displayName":"Display name",
      "isDeviceOnlyAuthSupported":null,
      "groupMembershipClaims":null,
      "optionalClaims":null,
      "addIns":[],
      "publisherDomain":"contoso.onmicrosoft.com",
      "signInAudience":"AzureADMyOrg",
      "tags":[],
      "tokenEncryptionKeyId":null,
      "api":{
         "requestedAccessTokenVersion":2,
         "acceptMappedClaims":null,
         "knownClientApplications":[],
         "oauth2PermissionScopes":[],
         "preAuthorizedApplications":[]
      },
      "appRoles":[],
      "publicClient":{
         "redirectUris":[]
      },
      "info":{
         "termsOfServiceUrl":null,
         "supportUrl":null,
         "privacyStatementUrl":null,
         "marketingUrl":null,
         "logoUrl":null
      },
      "keyCredentials":[],
      "parentalControlSettings":{
         "countriesBlockedForMinors":[],
         "legalAgeGroupRule":"Allow"
      },
      "passwordCredentials":[],
      "requiredResourceAccess":[ ],
      "web":{
         "redirectUris":[],
         "homePageUrl":null,
         "logoutUrl":null,
         "implicitGrantSettings":{
            "enableIdTokenIssuance":false,
            "enableAccessTokenIssuance":false
         }
      }
   }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate: instantiate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
