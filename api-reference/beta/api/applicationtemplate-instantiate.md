---
title: 'applicationTemplate: 实例化'
description: 使用此 API 创建新的 applicationTemplate
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 64d754b0053cd63711f4c0a1ef35d8429be84883
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856688"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="81b0c-103">applicationTemplate: 实例化</span><span class="sxs-lookup"><span data-stu-id="81b0c-103">applicationTemplate: instantiate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81b0c-104">将 Azure AD 应用程序库中的应用程序实例添加到目录中。</span><span class="sxs-lookup"><span data-stu-id="81b0c-104">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="81b0c-105">权限</span><span class="sxs-lookup"><span data-stu-id="81b0c-105">Permissions</span></span>

<span data-ttu-id="81b0c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="81b0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="81b0c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="81b0c-108">Permission type</span></span>                        | <span data-ttu-id="81b0c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="81b0c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="81b0c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81b0c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="81b0c-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81b0c-111">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="81b0c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81b0c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81b0c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="81b0c-113">Not supported.</span></span> |
| <span data-ttu-id="81b0c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="81b0c-114">Application</span></span>                            | <span data-ttu-id="81b0c-115">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81b0c-115">Application.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81b0c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81b0c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="81b0c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="81b0c-117">Request headers</span></span>

| <span data-ttu-id="81b0c-118">名称</span><span class="sxs-lookup"><span data-stu-id="81b0c-118">Name</span></span>          | <span data-ttu-id="81b0c-119">说明</span><span class="sxs-lookup"><span data-stu-id="81b0c-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="81b0c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="81b0c-120">Authorization</span></span> | <span data-ttu-id="81b0c-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="81b0c-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="81b0c-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="81b0c-122">Request body</span></span>

<span data-ttu-id="81b0c-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="81b0c-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="81b0c-124">参数</span><span class="sxs-lookup"><span data-stu-id="81b0c-124">Parameter</span></span>    | <span data-ttu-id="81b0c-125">类型</span><span class="sxs-lookup"><span data-stu-id="81b0c-125">Type</span></span>        | <span data-ttu-id="81b0c-126">说明</span><span class="sxs-lookup"><span data-stu-id="81b0c-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="81b0c-127">displayName</span><span class="sxs-lookup"><span data-stu-id="81b0c-127">displayName</span></span>|<span data-ttu-id="81b0c-128">String</span><span class="sxs-lookup"><span data-stu-id="81b0c-128">String</span></span>|<span data-ttu-id="81b0c-129">应用程序的自定义名称</span><span class="sxs-lookup"><span data-stu-id="81b0c-129">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="81b0c-130">响应</span><span class="sxs-lookup"><span data-stu-id="81b0c-130">Response</span></span>

<span data-ttu-id="81b0c-131">如果成功, 此方法在响应`201 OK`正文中返回响应代码和新的[applicationServicePrincipal](../resources/applicationserviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="81b0c-131">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81b0c-132">示例</span><span class="sxs-lookup"><span data-stu-id="81b0c-132">Examples</span></span>

<span data-ttu-id="81b0c-133">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="81b0c-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="81b0c-134">请求</span><span class="sxs-lookup"><span data-stu-id="81b0c-134">Request</span></span>

<span data-ttu-id="81b0c-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="81b0c-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="81b0c-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="81b0c-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="81b0c-137">C#</span><span class="sxs-lookup"><span data-stu-id="81b0c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="81b0c-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="81b0c-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="81b0c-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="81b0c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="81b0c-140">Java</span><span class="sxs-lookup"><span data-stu-id="81b0c-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/applicationtemplate-instantiate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="81b0c-141">响应</span><span class="sxs-lookup"><span data-stu-id="81b0c-141">Response</span></span>

<span data-ttu-id="81b0c-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="81b0c-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="81b0c-143">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="81b0c-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="81b0c-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="81b0c-144">All the properties will be returned from an actual call.</span></span>

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
