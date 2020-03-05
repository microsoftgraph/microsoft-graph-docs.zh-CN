---
title: 创建应用程序
description: 创建新的应用程序。
author: davidmu1
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 18d6fbb458a66f31a53917d4a0a328f399cb2593
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441485"
---
# <a name="create-application"></a><span data-ttu-id="99b39-103">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="99b39-103">Create application</span></span>

<span data-ttu-id="99b39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99b39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99b39-105">创建新的 [application](../resources/application.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="99b39-105">Create a new [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="99b39-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="99b39-106">Permissions</span></span>
<span data-ttu-id="99b39-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99b39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="99b39-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="99b39-109">Permission type</span></span>      | <span data-ttu-id="99b39-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99b39-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99b39-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99b39-111">Delegated (work or school account)</span></span> | <span data-ttu-id="99b39-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="99b39-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="99b39-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99b39-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99b39-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="99b39-114">Not supported.</span></span>    |
|<span data-ttu-id="99b39-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="99b39-115">Application</span></span> | <span data-ttu-id="99b39-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="99b39-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="99b39-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99b39-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="99b39-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="99b39-118">Request headers</span></span>
| <span data-ttu-id="99b39-119">名称</span><span class="sxs-lookup"><span data-stu-id="99b39-119">Name</span></span>       | <span data-ttu-id="99b39-120">类型</span><span class="sxs-lookup"><span data-stu-id="99b39-120">Type</span></span> | <span data-ttu-id="99b39-121">说明</span><span class="sxs-lookup"><span data-stu-id="99b39-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="99b39-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="99b39-122">Authorization</span></span>  | <span data-ttu-id="99b39-123">string</span><span class="sxs-lookup"><span data-stu-id="99b39-123">string</span></span>  | <span data-ttu-id="99b39-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="99b39-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99b39-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="99b39-126">Request body</span></span>
<span data-ttu-id="99b39-127">在请求正文中，提供 [application](../resources/application.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99b39-127">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span> <span data-ttu-id="99b39-128">请求正文必须包含 **displayName**，这是必需的属性。</span><span class="sxs-lookup"><span data-stu-id="99b39-128">The request body must contain  **displayName**, which is a required property.</span></span>

## <a name="response"></a><span data-ttu-id="99b39-129">响应</span><span class="sxs-lookup"><span data-stu-id="99b39-129">Response</span></span>

<span data-ttu-id="99b39-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [application](../resources/application.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="99b39-130">If successful, this method returns `201 Created` response code and an [application](../resources/application.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="99b39-131">示例</span><span class="sxs-lookup"><span data-stu-id="99b39-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="99b39-132">请求</span><span class="sxs-lookup"><span data-stu-id="99b39-132">Request</span></span>
<span data-ttu-id="99b39-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="99b39-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="99b39-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="99b39-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="99b39-135">C#</span><span class="sxs-lookup"><span data-stu-id="99b39-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-from-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99b39-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99b39-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99b39-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99b39-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-from-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="99b39-138">响应</span><span class="sxs-lookup"><span data-stu-id="99b39-138">Response</span></span>
<span data-ttu-id="99b39-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="99b39-139">Here is an example of the response.</span></span> 

> <span data-ttu-id="99b39-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="99b39-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
