---
title: 创建应用程序
description: 创建新的应用程序。
author: davidmu1
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3b82c816eb9b55086431936b9b033d4e7179317a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37934311"
---
# <a name="create-application"></a><span data-ttu-id="83082-103">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="83082-103">Create application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83082-104">创建新的 [application](../resources/application.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="83082-104">Create a new [](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="83082-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="83082-105">Permissions</span></span>
<span data-ttu-id="83082-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83082-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="83082-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="83082-108">Permission type</span></span>      | <span data-ttu-id="83082-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="83082-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83082-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83082-110">Delegated (work or school account)</span></span> | <span data-ttu-id="83082-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="83082-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="83082-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83082-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83082-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="83082-113">Not supported.</span></span>    |
|<span data-ttu-id="83082-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="83082-114">Application</span></span> | <span data-ttu-id="83082-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="83082-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83082-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83082-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="83082-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="83082-117">Request headers</span></span>
| <span data-ttu-id="83082-118">名称</span><span class="sxs-lookup"><span data-stu-id="83082-118">Name</span></span>       | <span data-ttu-id="83082-119">类型</span><span class="sxs-lookup"><span data-stu-id="83082-119">Type</span></span> | <span data-ttu-id="83082-120">说明</span><span class="sxs-lookup"><span data-stu-id="83082-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="83082-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="83082-121">Authorization</span></span>  | <span data-ttu-id="83082-122">string</span><span class="sxs-lookup"><span data-stu-id="83082-122">string</span></span>  | <span data-ttu-id="83082-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="83082-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83082-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="83082-125">Request body</span></span>
<span data-ttu-id="83082-126">在请求正文中，提供 [application](../resources/application.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83082-126">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span> <span data-ttu-id="83082-127">请求正文必须包含 **displayName**，这是必需的属性。</span><span class="sxs-lookup"><span data-stu-id="83082-127">The request body must contain  **displayName**, which is a required property.</span></span>

## <a name="response"></a><span data-ttu-id="83082-128">响应</span><span class="sxs-lookup"><span data-stu-id="83082-128">Response</span></span>

<span data-ttu-id="83082-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [application](../resources/application.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="83082-129">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83082-130">示例</span><span class="sxs-lookup"><span data-stu-id="83082-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="83082-131">请求</span><span class="sxs-lookup"><span data-stu-id="83082-131">Request</span></span>
<span data-ttu-id="83082-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="83082-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="83082-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="83082-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_application_from_applications"
}-->
```http
POST https://graph.microsoft.com/beta/applications
Content-type: application/json
Content-length: 67

{
  "displayName": "Display name"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="83082-134">C#</span><span class="sxs-lookup"><span data-stu-id="83082-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-from-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="83082-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83082-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="83082-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83082-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-from-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="83082-137">响应</span><span class="sxs-lookup"><span data-stu-id="83082-137">Response</span></span>
<span data-ttu-id="83082-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="83082-138">Here is an example of the response.</span></span> 

> <span data-ttu-id="83082-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="83082-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 1145

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
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
