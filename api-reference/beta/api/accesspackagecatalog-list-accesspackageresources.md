---
title: 列出 accessPackageResources
description: 检索 accesspackageresource 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3aaeddef635a80bb8a54d3680281b8b9edae98ae
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53466943"
---
# <a name="list-accesspackageresources"></a><span data-ttu-id="a2399-103">列出 accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="a2399-103">List accessPackageResources</span></span>

<span data-ttu-id="a2399-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2399-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2399-105">在[accessPackageCatalog](../resources/accesspackagecatalog.md)中检索[accessPackageResource](../resources/accesspackageresource.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="a2399-105">Retrieve a list of [accessPackageResource](../resources/accesspackageresource.md) objects in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>  <span data-ttu-id="a2399-106">若要请求添加或删除 [accessPackageResource](../resources/accesspackageresource.md)，请使用 [create accessPackageResourceRequest](accesspackageresourcerequest-post.md)。</span><span class="sxs-lookup"><span data-stu-id="a2399-106">To request to add or remove an [accessPackageResource](../resources/accesspackageresource.md), use [create accessPackageResourceRequest](accesspackageresourcerequest-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a2399-107">权限</span><span class="sxs-lookup"><span data-stu-id="a2399-107">Permissions</span></span>

<span data-ttu-id="a2399-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2399-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2399-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2399-110">Permission type</span></span>                        | <span data-ttu-id="a2399-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2399-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a2399-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2399-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2399-113">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2399-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="a2399-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2399-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2399-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2399-115">Not supported.</span></span> |
| <span data-ttu-id="a2399-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2399-116">Application</span></span>                            | <span data-ttu-id="a2399-117">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2399-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2399-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2399-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2399-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a2399-119">Optional query parameters</span></span>

<span data-ttu-id="a2399-120">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a2399-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="a2399-121">例如，若要检索每个资源的访问包资源范围和环境，请包括在 `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` 查询中。</span><span class="sxs-lookup"><span data-stu-id="a2399-121">For example, to retrieve the access package resource scopes and environments for each resource, include `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` in the query.</span></span> <span data-ttu-id="a2399-122">若要检索资源的可用角色，请包含 `$expand=accessPackageResourceRoles` 。</span><span class="sxs-lookup"><span data-stu-id="a2399-122">To retrieve the available roles of a resource, include `$expand=accessPackageResourceRoles`.</span></span> <span data-ttu-id="a2399-123">若要仅检索应用程序的资源，而不是检索组或网站的资源，请 `$filter=resourceType eq 'Application'` 包括在查询中。</span><span class="sxs-lookup"><span data-stu-id="a2399-123">To retrieve only resources for applications and not groups or sites, include `$filter=resourceType eq 'Application'` in the query.</span></span> <span data-ttu-id="a2399-124">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="a2399-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2399-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2399-125">Request headers</span></span>

| <span data-ttu-id="a2399-126">名称</span><span class="sxs-lookup"><span data-stu-id="a2399-126">Name</span></span>      |<span data-ttu-id="a2399-127">说明</span><span class="sxs-lookup"><span data-stu-id="a2399-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a2399-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2399-128">Authorization</span></span> | <span data-ttu-id="a2399-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="a2399-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2399-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2399-131">Request body</span></span>

<span data-ttu-id="a2399-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a2399-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2399-133">响应</span><span class="sxs-lookup"><span data-stu-id="a2399-133">Response</span></span>

<span data-ttu-id="a2399-134">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackageResource](../resources/accesspackageresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a2399-134">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResource](../resources/accesspackageresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a2399-135">示例</span><span class="sxs-lookup"><span data-stu-id="a2399-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a2399-136">请求</span><span class="sxs-lookup"><span data-stu-id="a2399-136">Request</span></span>

<span data-ttu-id="a2399-137">下面是一个请求示例，使用筛选器选择特定类型的资源并 `$expand` 返回每个资源的资源范围。</span><span class="sxs-lookup"><span data-stu-id="a2399-137">The following is an example of the request, using a filter to select resources of a particular type and `$expand` to return resource scopes of each resource.</span></span>

# <a name="http"></a>[<span data-ttu-id="a2399-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2399-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources?$filter=resourceType eq 'Application'&$expand=accessPackageResourceScopes
```
# <a name="c"></a>[<span data-ttu-id="a2399-139">C#</span><span class="sxs-lookup"><span data-stu-id="a2399-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2399-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2399-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2399-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2399-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2399-142">Java</span><span class="sxs-lookup"><span data-stu-id="a2399-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a2399-143">响应</span><span class="sxs-lookup"><span data-stu-id="a2399-143">Response</span></span>

<span data-ttu-id="a2399-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a2399-144">The following is an example of the response.</span></span>

> <span data-ttu-id="a2399-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a2399-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "400279ff-8e85-4dcf-b1d6-d3a6be372951",
      "displayName": "Faculty cafeteria ordering",
      "description": "Example application",
      "url": "https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/",
      "resourceType": "Application",
      "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e",
      "accessPackageResourceScopes": [
         {
            "id": "452d78a7-69a5-482d-a82f-859a5169c55e",
            "displayName": "Root",
            "description": "Root Scope",
            "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e",
            "originSystem": "AadApplication",
            "isRootScope": true
         }
      ]
    }
  ]
}
```

https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/e71fafe7-9ccb-4c5a-a7b3-77ec35e83e3c/accessPackageResources

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


