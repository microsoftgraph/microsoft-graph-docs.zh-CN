---
title: 创建应用程序
description: 使用此 API 新建应用程序。
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 775f7d59ba19ed015b7af5d66e9d52ae817ec65c
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908318"
---
# <a name="create-application"></a><span data-ttu-id="f23c9-103">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="f23c9-103">Create Application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f23c9-104">使用此 API 新建应用程序。</span><span class="sxs-lookup"><span data-stu-id="f23c9-104">Use this API to create a new application.</span></span>

## <a name="permissions"></a><span data-ttu-id="f23c9-105">权限</span><span class="sxs-lookup"><span data-stu-id="f23c9-105">Permissions</span></span>
<span data-ttu-id="f23c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f23c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f23c9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f23c9-108">Permission type</span></span>      | <span data-ttu-id="f23c9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f23c9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f23c9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f23c9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f23c9-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f23c9-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f23c9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f23c9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f23c9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f23c9-113">Not supported.</span></span>    |
|<span data-ttu-id="f23c9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f23c9-114">Application</span></span> | <span data-ttu-id="f23c9-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f23c9-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f23c9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f23c9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="f23c9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f23c9-117">Request headers</span></span>
| <span data-ttu-id="f23c9-118">名称</span><span class="sxs-lookup"><span data-stu-id="f23c9-118">Name</span></span>       | <span data-ttu-id="f23c9-119">类型</span><span class="sxs-lookup"><span data-stu-id="f23c9-119">Type</span></span> | <span data-ttu-id="f23c9-120">说明</span><span class="sxs-lookup"><span data-stu-id="f23c9-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f23c9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f23c9-121">Authorization</span></span>  | <span data-ttu-id="f23c9-122">string</span><span class="sxs-lookup"><span data-stu-id="f23c9-122">string</span></span>  | <span data-ttu-id="f23c9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f23c9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f23c9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f23c9-125">Request body</span></span>
<span data-ttu-id="f23c9-126">在请求正文中，提供 [application](../resources/application.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f23c9-126">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f23c9-127">响应</span><span class="sxs-lookup"><span data-stu-id="f23c9-127">Response</span></span>

<span data-ttu-id="f23c9-128">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [application](../resources/application.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f23c9-128">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f23c9-129">示例</span><span class="sxs-lookup"><span data-stu-id="f23c9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f23c9-130">请求</span><span class="sxs-lookup"><span data-stu-id="f23c9-130">Request</span></span>
<span data-ttu-id="f23c9-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f23c9-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f23c9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f23c9-132">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_application_from_applications"
}-->
```http
POST https://graph.microsoft.com/beta/applications
Content-type: application/json
Content-length: 67

{
  "allowPublicClient": true,
  "displayName": "Display name"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f23c9-133">C#</span><span class="sxs-lookup"><span data-stu-id="f23c9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-from-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f23c9-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="f23c9-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f23c9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f23c9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-from-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f23c9-136">Java</span><span class="sxs-lookup"><span data-stu-id="f23c9-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-application-from-applications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="f23c9-137">在请求正文中，提供 [application](../resources/application.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f23c9-137">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f23c9-138">响应</span><span class="sxs-lookup"><span data-stu-id="f23c9-138">Response</span></span>
<span data-ttu-id="f23c9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f23c9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "id": "b5b2920e-a47c-43b7-91ef-25ae96fddddd",
    "deletedDateTime": null,
    "api": {
        "acceptedAccessTokenVersion": 2,
        "publishedPermissionScopes": []
    },
    "allowPublicClient": true,
    "applicationAliases": [],
    "appRoles": [],
    "createdDateTime": "2017-05-25T16:33:04.3646617Z",
    "installedClients": {
        "redirectUrls": []
    },
    "displayName": "Display name",
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "orgRestrictions": [],
    "passwordCredentials": [],
    "preAuthorizedApplications": [],
    "requiredResourceAccess": [],
    "tags": [],
    "web": {
        "redirectUrls": [],
        "logoutUrl": null,
        "oauth2AllowImplicitFlow": null
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
