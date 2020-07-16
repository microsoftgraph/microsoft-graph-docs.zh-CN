---
title: applicationTemplate：实例化
description: 使用此 API 创建新的 applicationTemplate
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 12928d7917ea0a274c69454d82943d72a7587c67
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050713"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="a784c-103">applicationTemplate：实例化</span><span class="sxs-lookup"><span data-stu-id="a784c-103">applicationTemplate: instantiate</span></span>

<span data-ttu-id="a784c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a784c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a784c-105">将 Azure AD 应用程序库中的应用程序实例添加到目录中。</span><span class="sxs-lookup"><span data-stu-id="a784c-105">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="a784c-106">权限</span><span class="sxs-lookup"><span data-stu-id="a784c-106">Permissions</span></span>

<span data-ttu-id="a784c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a784c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a784c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a784c-109">Permission type</span></span>                        | <span data-ttu-id="a784c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a784c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a784c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a784c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a784c-112">所有的读写全部。</span><span class="sxs-lookup"><span data-stu-id="a784c-112">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="a784c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a784c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a784c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a784c-114">Not supported.</span></span> |
| <span data-ttu-id="a784c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a784c-115">Application</span></span>                            | <span data-ttu-id="a784c-116">所有的读写全部。</span><span class="sxs-lookup"><span data-stu-id="a784c-116">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a784c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a784c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="a784c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a784c-118">Request headers</span></span>

| <span data-ttu-id="a784c-119">名称</span><span class="sxs-lookup"><span data-stu-id="a784c-119">Name</span></span>          | <span data-ttu-id="a784c-120">说明</span><span class="sxs-lookup"><span data-stu-id="a784c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a784c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a784c-121">Authorization</span></span> | <span data-ttu-id="a784c-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a784c-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a784c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a784c-123">Request body</span></span>

<span data-ttu-id="a784c-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a784c-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a784c-125">参数</span><span class="sxs-lookup"><span data-stu-id="a784c-125">Parameter</span></span>    | <span data-ttu-id="a784c-126">类型</span><span class="sxs-lookup"><span data-stu-id="a784c-126">Type</span></span>        | <span data-ttu-id="a784c-127">说明</span><span class="sxs-lookup"><span data-stu-id="a784c-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a784c-128">displayName</span><span class="sxs-lookup"><span data-stu-id="a784c-128">displayName</span></span>|<span data-ttu-id="a784c-129">String</span><span class="sxs-lookup"><span data-stu-id="a784c-129">String</span></span>|<span data-ttu-id="a784c-130">应用程序的自定义名称</span><span class="sxs-lookup"><span data-stu-id="a784c-130">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="a784c-131">响应</span><span class="sxs-lookup"><span data-stu-id="a784c-131">Response</span></span>

<span data-ttu-id="a784c-132">如果成功，此方法 `201 OK` 在响应正文中返回响应代码和新的[applicationServicePrincipal](../resources/applicationserviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a784c-132">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a784c-133">示例</span><span class="sxs-lookup"><span data-stu-id="a784c-133">Examples</span></span>

<span data-ttu-id="a784c-134">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a784c-134">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a784c-135">请求</span><span class="sxs-lookup"><span data-stu-id="a784c-135">Request</span></span>

<span data-ttu-id="a784c-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a784c-136">The following is an example of the request.</span></span>

> [!NOTE] 
> <span data-ttu-id="a784c-137">您可以使用此 API 实例化[非库应用程序](https://docs.microsoft.com/azure/active-directory/manage-apps/add-non-gallery-app)。</span><span class="sxs-lookup"><span data-stu-id="a784c-137">You can use this API to instantiate [non-gallery apps](https://docs.microsoft.com/azure/active-directory/manage-apps/add-non-gallery-app).</span></span> <span data-ttu-id="a784c-138">对**applicationTemplate**：使用以下 ID `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` 。</span><span class="sxs-lookup"><span data-stu-id="a784c-138">Use the following ID for **applicationTemplate**: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>

# <a name="http"></a>[<span data-ttu-id="a784c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="a784c-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a784c-140">C#</span><span class="sxs-lookup"><span data-stu-id="a784c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a784c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a784c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a784c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a784c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a784c-143">响应</span><span class="sxs-lookup"><span data-stu-id="a784c-143">Response</span></span>

<span data-ttu-id="a784c-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a784c-144">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="a784c-145">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a784c-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a784c-146">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a784c-146">All the properties will be returned from an actual call.</span></span>

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
