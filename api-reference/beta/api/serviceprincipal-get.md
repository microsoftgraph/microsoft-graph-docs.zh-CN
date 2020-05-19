---
title: 获取 servicePrincipal
description: 检索 serviceprincipal 对象的属性和关系。
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f111552f6885fa514a003ccd37c3eb157035a33d
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291263"
---
# <a name="get-serviceprincipal"></a><span data-ttu-id="f56c0-103">获取 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="f56c0-103">Get servicePrincipal</span></span>

<span data-ttu-id="f56c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f56c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f56c0-105">检索[servicePrincipal](../resources/serviceprincipal.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f56c0-105">Retrieve the properties and relationships of a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f56c0-106">权限</span><span class="sxs-lookup"><span data-stu-id="f56c0-106">Permissions</span></span>
<span data-ttu-id="f56c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f56c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f56c0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f56c0-109">Permission type</span></span>      | <span data-ttu-id="f56c0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f56c0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f56c0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f56c0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f56c0-112">"Application"、"all"、"Directory.accessasuser.all"、"全部"、"全部"、"全部"、"全部"、"所有"</span><span class="sxs-lookup"><span data-stu-id="f56c0-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f56c0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f56c0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f56c0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f56c0-114">Not supported.</span></span>    |
|<span data-ttu-id="f56c0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f56c0-115">Application</span></span> | <span data-ttu-id="f56c0-116">"Application.readwrite.ownedby"、"所有"、"readwrite"、"全部"、"所有"、"</span><span class="sxs-lookup"><span data-stu-id="f56c0-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f56c0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f56c0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f56c0-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f56c0-118">Optional query parameters</span></span>
<span data-ttu-id="f56c0-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f56c0-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f56c0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f56c0-120">Request headers</span></span>
| <span data-ttu-id="f56c0-121">名称</span><span class="sxs-lookup"><span data-stu-id="f56c0-121">Name</span></span>           | <span data-ttu-id="f56c0-122">说明</span><span class="sxs-lookup"><span data-stu-id="f56c0-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="f56c0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f56c0-123">Authorization</span></span>  | <span data-ttu-id="f56c0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f56c0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f56c0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f56c0-126">Request body</span></span>
<span data-ttu-id="f56c0-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f56c0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f56c0-128">响应</span><span class="sxs-lookup"><span data-stu-id="f56c0-128">Response</span></span>
<span data-ttu-id="f56c0-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[servicePrincipal](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f56c0-129">If successful, this method returns a `200 OK` response code and a [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f56c0-130">示例</span><span class="sxs-lookup"><span data-stu-id="f56c0-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="f56c0-131">请求</span><span class="sxs-lookup"><span data-stu-id="f56c0-131">Request</span></span>
<span data-ttu-id="f56c0-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f56c0-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}-->

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}
```

### <a name="response"></a><span data-ttu-id="f56c0-133">响应</span><span class="sxs-lookup"><span data-stu-id="f56c0-133">Response</span></span>
<span data-ttu-id="f56c0-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f56c0-134">Here is an example of the response.</span></span> 

><span data-ttu-id="f56c0-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f56c0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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