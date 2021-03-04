---
title: 列出 accessPackageResourceRoles
description: 检索 accessPackageResourceRole 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9d3a8c243b6e2789fada38dec2643f3cd9bd1bd9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439562"
---
# <a name="list-accesspackageresourceroles"></a><span data-ttu-id="eb99e-103">列出 accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="eb99e-103">List accessPackageResourceRoles</span></span>

<span data-ttu-id="eb99e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb99e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb99e-105">在 accessPackageCatalog 中检索[accessPackageResourceResource](../resources/accesspackageresource.md)的[accessPackageResourceRole 对象列表](../resources/accesspackagecatalog.md)。 [](../resources/accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="eb99e-105">Retrieve a list of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects of an [accessPackageResource](../resources/accesspackageresource.md) in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>  <span data-ttu-id="eb99e-106">然后，呼叫者可以使用此角色列表来选择角色，随后创建 [accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md)时需要此角色。</span><span class="sxs-lookup"><span data-stu-id="eb99e-106">This list of roles can then be used by the caller to select a role, which is needed when subsequently [creating an accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb99e-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="eb99e-107">Permissions</span></span>

<span data-ttu-id="eb99e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb99e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eb99e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb99e-110">Permission type</span></span>                        | <span data-ttu-id="eb99e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb99e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="eb99e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb99e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb99e-113">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb99e-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="eb99e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb99e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb99e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb99e-115">Not supported.</span></span> |
| <span data-ttu-id="eb99e-116">Application</span><span class="sxs-lookup"><span data-stu-id="eb99e-116">Application</span></span>                            | <span data-ttu-id="eb99e-117">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb99e-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb99e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb99e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{catalogId}/accessPackageResourceRoles?$filter=(originSystem+eq+%27{originSystemType}%27+and+accessPackageResource/id+eq+%27{resourceId}%27)&$expand=accessPackageResource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb99e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="eb99e-119">Optional query parameters</span></span>

<span data-ttu-id="eb99e-120">此方法使用 OData 查询参数构造响应。</span><span class="sxs-lookup"><span data-stu-id="eb99e-120">This method uses OData query parameters to construct the response.</span></span> <span data-ttu-id="eb99e-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="eb99e-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb99e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb99e-122">Request headers</span></span>

| <span data-ttu-id="eb99e-123">名称</span><span class="sxs-lookup"><span data-stu-id="eb99e-123">Name</span></span>      |<span data-ttu-id="eb99e-124">说明</span><span class="sxs-lookup"><span data-stu-id="eb99e-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eb99e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb99e-125">Authorization</span></span> | <span data-ttu-id="eb99e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eb99e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb99e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb99e-128">Request body</span></span>

<span data-ttu-id="eb99e-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eb99e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb99e-130">响应</span><span class="sxs-lookup"><span data-stu-id="eb99e-130">Response</span></span>

<span data-ttu-id="eb99e-131">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [accessPackageResourceRole](../resources/accesspackageresourcerole.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="eb99e-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb99e-132">示例</span><span class="sxs-lookup"><span data-stu-id="eb99e-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eb99e-133">请求</span><span class="sxs-lookup"><span data-stu-id="eb99e-133">Request</span></span>

<span data-ttu-id="eb99e-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="eb99e-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eb99e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb99e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceroles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/15d889df-3eb8-4e9b-bfb4-b1908849aec4/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%27a35bef72-a8aa-4ca3-af30-f6b2ece7208f%27)&$expand=accessPackageResource
```
# <a name="c"></a>[<span data-ttu-id="eb99e-136">C#</span><span class="sxs-lookup"><span data-stu-id="eb99e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourceroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb99e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb99e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourceroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb99e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb99e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourceroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb99e-139">Java</span><span class="sxs-lookup"><span data-stu-id="eb99e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourceroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eb99e-140">响应</span><span class="sxs-lookup"><span data-stu-id="eb99e-140">Response</span></span>

<span data-ttu-id="eb99e-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="eb99e-141">The following is an example of the response.</span></span>

> <span data-ttu-id="eb99e-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="eb99e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "displayName": "Member",
      "description": "description-value",
      "originId": "originId-value",
      "originSystem": "originSystem-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


