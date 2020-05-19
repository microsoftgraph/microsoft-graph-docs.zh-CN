---
title: 创建应用程序
description: 创建新的应用程序。
author: sureshja
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 005de9ffadbe5264e595a59b59ae4d4e6c2a4842
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289304"
---
# <a name="create-application"></a><span data-ttu-id="c4985-103">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="c4985-103">Create application</span></span>

<span data-ttu-id="c4985-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4985-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4985-105">创建新的 [application](../resources/application.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c4985-105">Create a new [application](../resources/application.md) object.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c4985-106">不支持在创建应用程序时添加[**passwordCredential**](../resources/passwordcredential.md) 。</span><span class="sxs-lookup"><span data-stu-id="c4985-106">Adding [**passwordCredential**](../resources/passwordcredential.md) when creating applications is not supported.</span></span> <span data-ttu-id="c4985-107">使用[addPassword](application-addpassword.md)方法可为应用程序添加密码。</span><span class="sxs-lookup"><span data-stu-id="c4985-107">Use the [addPassword](application-addpassword.md) method to add passwords for an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4985-108">权限</span><span class="sxs-lookup"><span data-stu-id="c4985-108">Permissions</span></span>
<span data-ttu-id="c4985-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4985-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c4985-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4985-111">Permission type</span></span>      | <span data-ttu-id="c4985-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4985-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4985-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4985-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c4985-114">所有的 Directory.accessasuser.all，all，all，All</span><span class="sxs-lookup"><span data-stu-id="c4985-114">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c4985-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4985-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4985-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4985-116">Not supported.</span></span>    |
|<span data-ttu-id="c4985-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4985-117">Application</span></span> | <span data-ttu-id="c4985-118">Application.readwrite.ownedby、所有的 readwrite、全部、读写。</span><span class="sxs-lookup"><span data-stu-id="c4985-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4985-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4985-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="c4985-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4985-120">Request headers</span></span>
| <span data-ttu-id="c4985-121">名称</span><span class="sxs-lookup"><span data-stu-id="c4985-121">Name</span></span>           | <span data-ttu-id="c4985-122">说明</span><span class="sxs-lookup"><span data-stu-id="c4985-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="c4985-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4985-123">Authorization</span></span>  | <span data-ttu-id="c4985-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4985-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c4985-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4985-126">Content-Type</span></span>   | <span data-ttu-id="c4985-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c4985-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4985-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4985-129">Request body</span></span>
<span data-ttu-id="c4985-130">在请求正文中，提供 [application](../resources/application.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4985-130">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span> <span data-ttu-id="c4985-131">请求正文必须包含 **displayName**，这是必需的属性。</span><span class="sxs-lookup"><span data-stu-id="c4985-131">The request body must contain  **displayName**, which is a required property.</span></span>

## <a name="response"></a><span data-ttu-id="c4985-132">响应</span><span class="sxs-lookup"><span data-stu-id="c4985-132">Response</span></span>

<span data-ttu-id="c4985-133">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [application](../resources/application.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c4985-133">If successful, this method returns `201 Created` response code and an [application](../resources/application.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4985-134">示例</span><span class="sxs-lookup"><span data-stu-id="c4985-134">Examples</span></span>
### <a name="request"></a><span data-ttu-id="c4985-135">请求</span><span class="sxs-lookup"><span data-stu-id="c4985-135">Request</span></span>
<span data-ttu-id="c4985-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c4985-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c4985-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4985-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c4985-138">C#</span><span class="sxs-lookup"><span data-stu-id="c4985-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-from-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4985-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4985-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4985-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4985-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-from-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c4985-141">响应</span><span class="sxs-lookup"><span data-stu-id="c4985-141">Response</span></span>
<span data-ttu-id="c4985-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c4985-142">Here is an example of the response.</span></span> 

> <span data-ttu-id="c4985-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c4985-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
