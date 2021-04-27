---
title: 获取应用程序
description: 获取 application 对象的属性和关系。
author: sureshja
localization_priority: Priority
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 5c1c15ede7c49bf7aa5fdd0ae5fdfbaa3c59cbb8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048132"
---
# <a name="get-application"></a><span data-ttu-id="2bc9e-103">获取应用程序</span><span class="sxs-lookup"><span data-stu-id="2bc9e-103">Get application</span></span>

<span data-ttu-id="2bc9e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bc9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bc9e-105">获取 [application](../resources/application.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2bc9e-105">Get the properties and relationships of an [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2bc9e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="2bc9e-106">Permissions</span></span>
<span data-ttu-id="2bc9e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2bc9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bc9e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2bc9e-109">Permission type</span></span>      | <span data-ttu-id="2bc9e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2bc9e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2bc9e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2bc9e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2bc9e-112">Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2bc9e-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2bc9e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2bc9e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bc9e-114">Application.Read.All， Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bc9e-114">Application.Read.All, Application.ReadWrite.All</span></span>    |
|<span data-ttu-id="2bc9e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2bc9e-115">Application</span></span> | <span data-ttu-id="2bc9e-116">Application.Read.All、 Directory.Read.All、 Application.ReadWrite.OwnedBy、  Application.ReadWrite.All、 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bc9e-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy,  Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2bc9e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2bc9e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2bc9e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2bc9e-118">Optional query parameters</span></span>
<span data-ttu-id="2bc9e-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2bc9e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2bc9e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2bc9e-120">Request headers</span></span>
| <span data-ttu-id="2bc9e-121">名称</span><span class="sxs-lookup"><span data-stu-id="2bc9e-121">Name</span></span>           | <span data-ttu-id="2bc9e-122">说明</span><span class="sxs-lookup"><span data-stu-id="2bc9e-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="2bc9e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bc9e-123">Authorization</span></span>  | <span data-ttu-id="2bc9e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2bc9e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2bc9e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2bc9e-126">Request body</span></span>
<span data-ttu-id="2bc9e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2bc9e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bc9e-128">响应</span><span class="sxs-lookup"><span data-stu-id="2bc9e-128">Response</span></span>

<span data-ttu-id="2bc9e-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [application](../resources/application.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2bc9e-129">If successful, this method returns a `200 OK` response code and an [application](../resources/application.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="2bc9e-130">示例</span><span class="sxs-lookup"><span data-stu-id="2bc9e-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="2bc9e-131">请求</span><span class="sxs-lookup"><span data-stu-id="2bc9e-131">Request</span></span>
<span data-ttu-id="2bc9e-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2bc9e-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2bc9e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2bc9e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}
```
# <a name="c"></a>[<span data-ttu-id="2bc9e-134">C#</span><span class="sxs-lookup"><span data-stu-id="2bc9e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2bc9e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2bc9e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2bc9e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2bc9e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2bc9e-137">Java</span><span class="sxs-lookup"><span data-stu-id="2bc9e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2bc9e-138">响应</span><span class="sxs-lookup"><span data-stu-id="2bc9e-138">Response</span></span>
<span data-ttu-id="2bc9e-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2bc9e-139">Here is an example of the response.</span></span> 

><span data-ttu-id="2bc9e-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2bc9e-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1044

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications/$entity",
    "id": "03ef14b0-ca33-4840-8f4f-d6e91916010e",
    "deletedDateTime": null,
    "isFallbackPublicClient": null,
    "appId": "631a96bc-a705-4eda-9f99-fdaf9f54f6a2",
    "applicationTemplateId": null,
    "identifierUris": [],
    "createdDateTime": "2019-09-17T19:10:35.2742618Z",
    "displayName": "Display name",
    "isDeviceOnlyAuthSupported": null,
    "groupMembershipClaims": null,
    "optionalClaims": null,
    "addIns": [],
    "publisherDomain": "contoso.onmicrosoft.com",
    "signInAudience": "AzureADandPersonalMicrosoftAccount",
    "tags": [],
    "tokenEncryptionKeyId": null,
    "api": {
        "requestedAccessTokenVersion": 2,
        "acceptMappedClaims": null,
        "knownClientApplications": [],
        "oauth2PermissionScopes": [],
        "preAuthorizedApplications": []
    },
    "appRoles": [],
    "publicClient": {
        "redirectUris": []
    },
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "parentalControlSettings": {
        "countriesBlockedForMinors": [],
        "legalAgeGroupRule": "Allow"
    },
    "passwordCredentials": [],
    "requiredResourceAccess": [],
    "uniqueName": null,
    "web": {
        "redirectUris": [],
        "homePageUrl": null,
        "logoutUrl": null,
        "implicitGrantSettings": {
            "enableIdTokenIssuance": false,
            "enableAccessTokenIssuance": false
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



