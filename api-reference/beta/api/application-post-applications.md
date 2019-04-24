---
title: 创建应用程序
description: 使用此 API 新建应用程序。
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: b86030eede69b85d7b66e4ec5acdd7e2dfef0ce4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459106"
---
# <a name="create-application"></a><span data-ttu-id="483f1-103">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="483f1-103">Create Application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="483f1-104">使用此 API 新建应用程序。</span><span class="sxs-lookup"><span data-stu-id="483f1-104">Use this API to create a new application.</span></span>

## <a name="permissions"></a><span data-ttu-id="483f1-105">权限</span><span class="sxs-lookup"><span data-stu-id="483f1-105">Permissions</span></span>
<span data-ttu-id="483f1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="483f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="483f1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="483f1-108">Permission type</span></span>      | <span data-ttu-id="483f1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="483f1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="483f1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="483f1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="483f1-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="483f1-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="483f1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="483f1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="483f1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="483f1-113">Not supported.</span></span>    |
|<span data-ttu-id="483f1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="483f1-114">Application</span></span> | <span data-ttu-id="483f1-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="483f1-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="483f1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="483f1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="483f1-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="483f1-117">Request headers</span></span>
| <span data-ttu-id="483f1-118">名称</span><span class="sxs-lookup"><span data-stu-id="483f1-118">Name</span></span>       | <span data-ttu-id="483f1-119">类型</span><span class="sxs-lookup"><span data-stu-id="483f1-119">Type</span></span> | <span data-ttu-id="483f1-120">说明</span><span class="sxs-lookup"><span data-stu-id="483f1-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="483f1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="483f1-121">Authorization</span></span>  | <span data-ttu-id="483f1-122">string</span><span class="sxs-lookup"><span data-stu-id="483f1-122">string</span></span>  | <span data-ttu-id="483f1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="483f1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="483f1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="483f1-125">Request body</span></span>
<span data-ttu-id="483f1-126">在请求正文中，提供 [application](../resources/application.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="483f1-126">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="483f1-127">响应</span><span class="sxs-lookup"><span data-stu-id="483f1-127">Response</span></span>

<span data-ttu-id="483f1-128">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [application](../resources/application.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="483f1-128">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="483f1-129">示例</span><span class="sxs-lookup"><span data-stu-id="483f1-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="483f1-130">请求</span><span class="sxs-lookup"><span data-stu-id="483f1-130">Request</span></span>
<span data-ttu-id="483f1-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="483f1-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="483f1-132">在请求正文中，提供 [application](../resources/application.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="483f1-132">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="483f1-133">响应</span><span class="sxs-lookup"><span data-stu-id="483f1-133">Response</span></span>
<span data-ttu-id="483f1-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="483f1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/application-post-applications.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
