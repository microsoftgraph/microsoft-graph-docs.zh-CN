---
title: applicationTemplate：实例化
description: 使用此 API 创建新的 applicationTemplate
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8f0ec8b1501d4501703fbe5d41630039976fd4c8
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312538"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="3ecda-103">applicationTemplate：实例化</span><span class="sxs-lookup"><span data-stu-id="3ecda-103">applicationTemplate: instantiate</span></span>

<span data-ttu-id="3ecda-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ecda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ecda-105">将 Azure AD 应用程序库中的应用程序实例添加到目录中。</span><span class="sxs-lookup"><span data-stu-id="3ecda-105">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ecda-106">权限</span><span class="sxs-lookup"><span data-stu-id="3ecda-106">Permissions</span></span>

<span data-ttu-id="3ecda-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ecda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ecda-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ecda-109">Permission type</span></span>                        | <span data-ttu-id="3ecda-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ecda-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3ecda-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ecda-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ecda-112">所有的读写全部。</span><span class="sxs-lookup"><span data-stu-id="3ecda-112">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="3ecda-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ecda-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ecda-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ecda-114">Not supported.</span></span> |
| <span data-ttu-id="3ecda-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ecda-115">Application</span></span>                            | <span data-ttu-id="3ecda-116">所有的读写全部。</span><span class="sxs-lookup"><span data-stu-id="3ecda-116">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ecda-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ecda-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="3ecda-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ecda-118">Request headers</span></span>

| <span data-ttu-id="3ecda-119">名称</span><span class="sxs-lookup"><span data-stu-id="3ecda-119">Name</span></span>          | <span data-ttu-id="3ecda-120">说明</span><span class="sxs-lookup"><span data-stu-id="3ecda-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3ecda-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ecda-121">Authorization</span></span> | <span data-ttu-id="3ecda-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3ecda-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ecda-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ecda-123">Request body</span></span>

<span data-ttu-id="3ecda-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3ecda-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3ecda-125">参数</span><span class="sxs-lookup"><span data-stu-id="3ecda-125">Parameter</span></span>    | <span data-ttu-id="3ecda-126">类型</span><span class="sxs-lookup"><span data-stu-id="3ecda-126">Type</span></span>        | <span data-ttu-id="3ecda-127">说明</span><span class="sxs-lookup"><span data-stu-id="3ecda-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3ecda-128">displayName</span><span class="sxs-lookup"><span data-stu-id="3ecda-128">displayName</span></span>|<span data-ttu-id="3ecda-129">字符串</span><span class="sxs-lookup"><span data-stu-id="3ecda-129">String</span></span>|<span data-ttu-id="3ecda-130">应用程序的自定义名称</span><span class="sxs-lookup"><span data-stu-id="3ecda-130">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="3ecda-131">响应</span><span class="sxs-lookup"><span data-stu-id="3ecda-131">Response</span></span>

<span data-ttu-id="3ecda-132">如果成功，此方法 `201 OK` 在响应正文中返回响应代码和新的 [applicationServicePrincipal](../resources/applicationserviceprincipal.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3ecda-132">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3ecda-133">示例</span><span class="sxs-lookup"><span data-stu-id="3ecda-133">Examples</span></span>

<span data-ttu-id="3ecda-134">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="3ecda-134">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="3ecda-135">请求</span><span class="sxs-lookup"><span data-stu-id="3ecda-135">Request</span></span>

<span data-ttu-id="3ecda-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3ecda-136">The following is an example of the request.</span></span>

> [!NOTE] 
> <span data-ttu-id="3ecda-137">您可以使用此 API 实例化 [非库应用程序](/azure/active-directory/manage-apps/add-non-gallery-app)。</span><span class="sxs-lookup"><span data-stu-id="3ecda-137">You can use this API to instantiate [non-gallery apps](/azure/active-directory/manage-apps/add-non-gallery-app).</span></span> <span data-ttu-id="3ecda-138">对 **applicationTemplate**：使用以下 ID `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` 。</span><span class="sxs-lookup"><span data-stu-id="3ecda-138">Use the following ID for **applicationTemplate**: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>

# <a name="http"></a>[<span data-ttu-id="3ecda-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ecda-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3ecda-140">C#</span><span class="sxs-lookup"><span data-stu-id="3ecda-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ecda-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ecda-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ecda-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ecda-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3ecda-143">响应</span><span class="sxs-lookup"><span data-stu-id="3ecda-143">Response</span></span>

<span data-ttu-id="3ecda-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3ecda-144">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="3ecda-145">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3ecda-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3ecda-146">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3ecda-146">All the properties will be returned from an actual call.</span></span>

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