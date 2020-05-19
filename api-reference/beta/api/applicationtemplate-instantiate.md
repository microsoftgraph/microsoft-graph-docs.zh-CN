---
title: applicationTemplate：实例化
description: 使用此 API 创建新的 applicationTemplate
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ff663e0775a0a18f8f82daaa547a6ca774f9138f
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289115"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="63972-103">applicationTemplate：实例化</span><span class="sxs-lookup"><span data-stu-id="63972-103">applicationTemplate: instantiate</span></span>

<span data-ttu-id="63972-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63972-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63972-105">将 Azure AD 应用程序库中的应用程序实例添加到目录中。</span><span class="sxs-lookup"><span data-stu-id="63972-105">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="63972-106">权限</span><span class="sxs-lookup"><span data-stu-id="63972-106">Permissions</span></span>

<span data-ttu-id="63972-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63972-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63972-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="63972-109">Permission type</span></span>                        | <span data-ttu-id="63972-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63972-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="63972-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63972-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="63972-112">所有的读写全部。</span><span class="sxs-lookup"><span data-stu-id="63972-112">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="63972-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63972-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63972-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="63972-114">Not supported.</span></span> |
| <span data-ttu-id="63972-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="63972-115">Application</span></span>                            | <span data-ttu-id="63972-116">所有的读写全部。</span><span class="sxs-lookup"><span data-stu-id="63972-116">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="63972-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63972-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="63972-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="63972-118">Request headers</span></span>

| <span data-ttu-id="63972-119">名称</span><span class="sxs-lookup"><span data-stu-id="63972-119">Name</span></span>          | <span data-ttu-id="63972-120">说明</span><span class="sxs-lookup"><span data-stu-id="63972-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="63972-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="63972-121">Authorization</span></span> | <span data-ttu-id="63972-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="63972-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="63972-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="63972-123">Request body</span></span>

<span data-ttu-id="63972-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="63972-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="63972-125">参数</span><span class="sxs-lookup"><span data-stu-id="63972-125">Parameter</span></span>    | <span data-ttu-id="63972-126">类型</span><span class="sxs-lookup"><span data-stu-id="63972-126">Type</span></span>        | <span data-ttu-id="63972-127">说明</span><span class="sxs-lookup"><span data-stu-id="63972-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="63972-128">displayName</span><span class="sxs-lookup"><span data-stu-id="63972-128">displayName</span></span>|<span data-ttu-id="63972-129">String</span><span class="sxs-lookup"><span data-stu-id="63972-129">String</span></span>|<span data-ttu-id="63972-130">应用程序的自定义名称</span><span class="sxs-lookup"><span data-stu-id="63972-130">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="63972-131">响应</span><span class="sxs-lookup"><span data-stu-id="63972-131">Response</span></span>

<span data-ttu-id="63972-132">如果成功，此方法 `201 OK` 在响应正文中返回响应代码和新的[applicationServicePrincipal](../resources/applicationserviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="63972-132">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63972-133">示例</span><span class="sxs-lookup"><span data-stu-id="63972-133">Examples</span></span>

<span data-ttu-id="63972-134">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="63972-134">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="63972-135">请求</span><span class="sxs-lookup"><span data-stu-id="63972-135">Request</span></span>

<span data-ttu-id="63972-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="63972-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="63972-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="63972-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="63972-138">C#</span><span class="sxs-lookup"><span data-stu-id="63972-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63972-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63972-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63972-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63972-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="63972-141">响应</span><span class="sxs-lookup"><span data-stu-id="63972-141">Response</span></span>

<span data-ttu-id="63972-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="63972-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="63972-143">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="63972-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="63972-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="63972-144">All the properties will be returned from an actual call.</span></span>

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
