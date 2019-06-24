---
title: 'applicationTemplate: 实例化'
description: 使用此 API 创建新的 applicationTemplate
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d3874f7e015816dbc76ce99fa1fc26f65727ad97
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147892"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="dd277-103">applicationTemplate: 实例化</span><span class="sxs-lookup"><span data-stu-id="dd277-103">applicationTemplate: instantiate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd277-104">将 Azure AD 应用程序库中的应用程序实例添加到目录中。</span><span class="sxs-lookup"><span data-stu-id="dd277-104">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd277-105">权限</span><span class="sxs-lookup"><span data-stu-id="dd277-105">Permissions</span></span>

<span data-ttu-id="dd277-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd277-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd277-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd277-108">Permission type</span></span>                        | <span data-ttu-id="dd277-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd277-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dd277-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd277-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd277-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd277-111">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="dd277-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd277-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd277-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd277-113">Not supported.</span></span> |
| <span data-ttu-id="dd277-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd277-114">Application</span></span>                            | <span data-ttu-id="dd277-115">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd277-115">Application.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd277-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd277-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="dd277-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd277-117">Request headers</span></span>

| <span data-ttu-id="dd277-118">名称</span><span class="sxs-lookup"><span data-stu-id="dd277-118">Name</span></span>          | <span data-ttu-id="dd277-119">说明</span><span class="sxs-lookup"><span data-stu-id="dd277-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="dd277-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd277-120">Authorization</span></span> | <span data-ttu-id="dd277-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="dd277-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd277-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd277-122">Request body</span></span>

<span data-ttu-id="dd277-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="dd277-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dd277-124">参数</span><span class="sxs-lookup"><span data-stu-id="dd277-124">Parameter</span></span>    | <span data-ttu-id="dd277-125">类型</span><span class="sxs-lookup"><span data-stu-id="dd277-125">Type</span></span>        | <span data-ttu-id="dd277-126">说明</span><span class="sxs-lookup"><span data-stu-id="dd277-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd277-127">displayName</span><span class="sxs-lookup"><span data-stu-id="dd277-127">displayName</span></span>|<span data-ttu-id="dd277-128">String</span><span class="sxs-lookup"><span data-stu-id="dd277-128">String</span></span>|<span data-ttu-id="dd277-129">应用程序的自定义名称</span><span class="sxs-lookup"><span data-stu-id="dd277-129">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="dd277-130">响应</span><span class="sxs-lookup"><span data-stu-id="dd277-130">Response</span></span>

<span data-ttu-id="dd277-131">如果成功, 此方法在响应`201 OK`正文中返回响应代码和新的[applicationServicePrincipal](../resources/applicationserviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dd277-131">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dd277-132">示例</span><span class="sxs-lookup"><span data-stu-id="dd277-132">Examples</span></span>

<span data-ttu-id="dd277-133">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="dd277-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="dd277-134">请求</span><span class="sxs-lookup"><span data-stu-id="dd277-134">Request</span></span>

<span data-ttu-id="dd277-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dd277-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```http
POST https://graph.microsoft.com/beta/applicationTemplates/{id}/instantiate
Content-type: application/json

{
  "displayName": "My custom name"
}
```

### <a name="response"></a><span data-ttu-id="dd277-136">响应</span><span class="sxs-lookup"><span data-stu-id="dd277-136">Response</span></span>

<span data-ttu-id="dd277-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dd277-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="dd277-138">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dd277-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dd277-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dd277-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
} -->

```http
HTTP/1.1 201 OK
Content-type: application/json

{
   "servicePrincipal": {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
   },
   "application": {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
        "adminConsentDescription": "adminConsentDescription-value",
        "adminConsentDisplayName": "adminConsentDisplayName-value",
        "id": "id-value",
        "isEnabled": true,
        "type": "type-value",
        "userConsentDescription": "userConsentDescription-value",
        "userConsentDisplayName": "userConsentDisplayName-value",
        "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
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
