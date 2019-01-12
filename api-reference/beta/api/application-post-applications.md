---
title: 创建应用程序
description: 使用此 API 创建新的应用程序。
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 8cde90f31f7583d24361f6935701a91f69d7cfde
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941469"
---
# <a name="create-application"></a><span data-ttu-id="09903-103">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="09903-103">Create Application</span></span>

> <span data-ttu-id="09903-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="09903-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09903-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="09903-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="09903-106">使用此 API 创建新的应用程序。</span><span class="sxs-lookup"><span data-stu-id="09903-106">Use this API to create a new application.</span></span>

## <a name="permissions"></a><span data-ttu-id="09903-107">权限</span><span class="sxs-lookup"><span data-stu-id="09903-107">Permissions</span></span>
<span data-ttu-id="09903-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09903-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="09903-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="09903-110">Permission type</span></span>      | <span data-ttu-id="09903-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09903-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09903-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09903-112">Delegated (work or school account)</span></span> | <span data-ttu-id="09903-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09903-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="09903-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09903-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09903-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="09903-115">Not supported.</span></span>    |
|<span data-ttu-id="09903-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="09903-116">Application</span></span> | <span data-ttu-id="09903-117">Application.ReadWrite.OwnedBy Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09903-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09903-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09903-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="09903-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="09903-119">Request headers</span></span>
| <span data-ttu-id="09903-120">名称</span><span class="sxs-lookup"><span data-stu-id="09903-120">Name</span></span>       | <span data-ttu-id="09903-121">类型</span><span class="sxs-lookup"><span data-stu-id="09903-121">Type</span></span> | <span data-ttu-id="09903-122">说明</span><span class="sxs-lookup"><span data-stu-id="09903-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="09903-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="09903-123">Authorization</span></span>  | <span data-ttu-id="09903-124">string</span><span class="sxs-lookup"><span data-stu-id="09903-124">string</span></span>  | <span data-ttu-id="09903-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="09903-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09903-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="09903-127">Request body</span></span>
<span data-ttu-id="09903-128">在请求正文中，提供[应用程序](../resources/application.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09903-128">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="09903-129">响应</span><span class="sxs-lookup"><span data-stu-id="09903-129">Response</span></span>

<span data-ttu-id="09903-130">如果成功，此方法返回`201 Created`响应正文中的响应代码和[应用程序](../resources/application.md)对象。</span><span class="sxs-lookup"><span data-stu-id="09903-130">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09903-131">示例</span><span class="sxs-lookup"><span data-stu-id="09903-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09903-132">请求</span><span class="sxs-lookup"><span data-stu-id="09903-132">Request</span></span>
<span data-ttu-id="09903-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="09903-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="09903-134">在请求正文中，提供[应用程序](../resources/application.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09903-134">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="09903-135">响应</span><span class="sxs-lookup"><span data-stu-id="09903-135">Response</span></span>
<span data-ttu-id="09903-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="09903-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
