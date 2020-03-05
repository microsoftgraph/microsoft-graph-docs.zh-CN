---
title: applicationTemplate：实例化
description: 使用此 API 创建新的 applicationTemplate
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f37cc7351449fc2fadbf259dde16682545ccc235
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441380"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="4f244-103">applicationTemplate：实例化</span><span class="sxs-lookup"><span data-stu-id="4f244-103">applicationTemplate: instantiate</span></span>

<span data-ttu-id="4f244-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4f244-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f244-105">将 Azure AD 应用程序库中的应用程序实例添加到目录中。</span><span class="sxs-lookup"><span data-stu-id="4f244-105">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f244-106">权限</span><span class="sxs-lookup"><span data-stu-id="4f244-106">Permissions</span></span>

<span data-ttu-id="4f244-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f244-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f244-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f244-109">Permission type</span></span>                        | <span data-ttu-id="4f244-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f244-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4f244-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f244-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f244-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f244-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="4f244-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f244-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f244-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f244-114">Not supported.</span></span> |
| <span data-ttu-id="4f244-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f244-115">Application</span></span>                            | <span data-ttu-id="4f244-116">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f244-116">Application.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f244-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f244-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="4f244-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f244-118">Request headers</span></span>

| <span data-ttu-id="4f244-119">名称</span><span class="sxs-lookup"><span data-stu-id="4f244-119">Name</span></span>          | <span data-ttu-id="4f244-120">说明</span><span class="sxs-lookup"><span data-stu-id="4f244-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4f244-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f244-121">Authorization</span></span> | <span data-ttu-id="4f244-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4f244-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f244-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f244-123">Request body</span></span>

<span data-ttu-id="4f244-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4f244-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4f244-125">参数</span><span class="sxs-lookup"><span data-stu-id="4f244-125">Parameter</span></span>    | <span data-ttu-id="4f244-126">类型</span><span class="sxs-lookup"><span data-stu-id="4f244-126">Type</span></span>        | <span data-ttu-id="4f244-127">说明</span><span class="sxs-lookup"><span data-stu-id="4f244-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4f244-128">displayName</span><span class="sxs-lookup"><span data-stu-id="4f244-128">displayName</span></span>|<span data-ttu-id="4f244-129">String</span><span class="sxs-lookup"><span data-stu-id="4f244-129">String</span></span>|<span data-ttu-id="4f244-130">应用程序的自定义名称</span><span class="sxs-lookup"><span data-stu-id="4f244-130">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="4f244-131">响应</span><span class="sxs-lookup"><span data-stu-id="4f244-131">Response</span></span>

<span data-ttu-id="4f244-132">如果成功，此方法在响应`201 OK`正文中返回响应代码和新的[applicationServicePrincipal](../resources/applicationserviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4f244-132">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4f244-133">示例</span><span class="sxs-lookup"><span data-stu-id="4f244-133">Examples</span></span>

<span data-ttu-id="4f244-134">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="4f244-134">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4f244-135">请求</span><span class="sxs-lookup"><span data-stu-id="4f244-135">Request</span></span>

<span data-ttu-id="4f244-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4f244-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4f244-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f244-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4f244-138">C#</span><span class="sxs-lookup"><span data-stu-id="4f244-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f244-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f244-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f244-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f244-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4f244-141">响应</span><span class="sxs-lookup"><span data-stu-id="4f244-141">Response</span></span>

<span data-ttu-id="4f244-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4f244-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="4f244-143">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4f244-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4f244-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4f244-144">All the properties will be returned from an actual call.</span></span>

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
