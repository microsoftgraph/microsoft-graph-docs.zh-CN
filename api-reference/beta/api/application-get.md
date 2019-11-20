---
title: 获取应用程序
description: 获取 application 对象的属性和关系。
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e5a2fd02e7cf078aee3898b881d4754169ef0d6a
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747627"
---
# <a name="get-application"></a><span data-ttu-id="175ae-103">获取应用程序</span><span class="sxs-lookup"><span data-stu-id="175ae-103">Get application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="175ae-104">获取 [application](../resources/application.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="175ae-104">Get the properties and relationships of an [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="175ae-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="175ae-105">Permissions</span></span>
<span data-ttu-id="175ae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="175ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="175ae-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="175ae-108">Permission type</span></span>      | <span data-ttu-id="175ae-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="175ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="175ae-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="175ae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="175ae-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="175ae-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="175ae-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="175ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="175ae-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="175ae-113">Not supported.</span></span>    |
|<span data-ttu-id="175ae-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="175ae-114">Application</span></span> | <span data-ttu-id="175ae-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="175ae-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="175ae-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="175ae-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="175ae-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="175ae-117">Optional query parameters</span></span>
<span data-ttu-id="175ae-118">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="175ae-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="175ae-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="175ae-119">Request headers</span></span>
| <span data-ttu-id="175ae-120">名称</span><span class="sxs-lookup"><span data-stu-id="175ae-120">Name</span></span>       | <span data-ttu-id="175ae-121">类型</span><span class="sxs-lookup"><span data-stu-id="175ae-121">Type</span></span> | <span data-ttu-id="175ae-122">说明</span><span class="sxs-lookup"><span data-stu-id="175ae-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="175ae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="175ae-123">Authorization</span></span>  | <span data-ttu-id="175ae-124">string</span><span class="sxs-lookup"><span data-stu-id="175ae-124">string</span></span>  | <span data-ttu-id="175ae-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="175ae-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="175ae-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="175ae-127">Content-type</span></span> | <span data-ttu-id="175ae-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="175ae-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="175ae-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="175ae-130">Request body</span></span>
<span data-ttu-id="175ae-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="175ae-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="175ae-132">响应</span><span class="sxs-lookup"><span data-stu-id="175ae-132">Response</span></span>

<span data-ttu-id="175ae-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [application](../resources/application.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="175ae-133">If successful, this method returns a `200 OK` response code and an [application](../resources/application.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="175ae-134">示例</span><span class="sxs-lookup"><span data-stu-id="175ae-134">Examples</span></span>
### <a name="request"></a><span data-ttu-id="175ae-135">请求</span><span class="sxs-lookup"><span data-stu-id="175ae-135">Request</span></span>
<span data-ttu-id="175ae-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="175ae-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="175ae-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="175ae-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="175ae-138">C#</span><span class="sxs-lookup"><span data-stu-id="175ae-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="175ae-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="175ae-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="175ae-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="175ae-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="175ae-141">响应</span><span class="sxs-lookup"><span data-stu-id="175ae-141">Response</span></span>
<span data-ttu-id="175ae-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="175ae-142">Here is an example of the response.</span></span> 

><span data-ttu-id="175ae-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="175ae-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
