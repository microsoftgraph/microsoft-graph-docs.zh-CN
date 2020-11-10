---
title: 列出 accessPackageResourceRoles
description: 检索 accessPackageResourceRole 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 209cfb488ec3747b82c61b1b7b2adbb8325f3617
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951949"
---
# <a name="list-accesspackageresourceroles"></a><span data-ttu-id="849dc-103">列出 accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="849dc-103">List accessPackageResourceRoles</span></span>

<span data-ttu-id="849dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="849dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="849dc-105">在[accessPackageCatalog](../resources/accesspackagecatalog.md)中检索[accessPackageResource](../resources/accesspackageresource.md)的[accessPackageResourceRole](../resources/accesspackageresourcerole.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="849dc-105">Retrieve a list of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects of an [accessPackageResource](../resources/accesspackageresource.md) in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>  <span data-ttu-id="849dc-106">然后，调用方可以使用此角色列表来选择角色，在随后 [创建 accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md)时需要该角色。</span><span class="sxs-lookup"><span data-stu-id="849dc-106">This list of roles can then be used by the caller to select a role, which is needed when subsequently [creating an accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="849dc-107">权限</span><span class="sxs-lookup"><span data-stu-id="849dc-107">Permissions</span></span>

<span data-ttu-id="849dc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="849dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="849dc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="849dc-110">Permission type</span></span>                        | <span data-ttu-id="849dc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="849dc-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="849dc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="849dc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="849dc-113">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="849dc-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="849dc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="849dc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="849dc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="849dc-115">Not supported.</span></span> |
| <span data-ttu-id="849dc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="849dc-116">Application</span></span>                            | <span data-ttu-id="849dc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="849dc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="849dc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="849dc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{catalogId}/accessPackageResourceRoles?$filter=(originSystem+eq+%27{originSystemType}%27+and+accessPackageResource/id+eq+%27{resourceId}%27)&$expand=accessPackageResource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="849dc-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="849dc-119">Optional query parameters</span></span>

<span data-ttu-id="849dc-120">此方法使用 OData 查询参数构造响应。</span><span class="sxs-lookup"><span data-stu-id="849dc-120">This method uses OData query parameters to construct the response.</span></span> <span data-ttu-id="849dc-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="849dc-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="849dc-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="849dc-122">Request headers</span></span>

| <span data-ttu-id="849dc-123">名称</span><span class="sxs-lookup"><span data-stu-id="849dc-123">Name</span></span>      |<span data-ttu-id="849dc-124">说明</span><span class="sxs-lookup"><span data-stu-id="849dc-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="849dc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="849dc-125">Authorization</span></span> | <span data-ttu-id="849dc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="849dc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="849dc-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="849dc-128">Request body</span></span>

<span data-ttu-id="849dc-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="849dc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="849dc-130">响应</span><span class="sxs-lookup"><span data-stu-id="849dc-130">Response</span></span>

<span data-ttu-id="849dc-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [accessPackageResourceRole](../resources/accesspackageresourcerole.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="849dc-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="849dc-132">示例</span><span class="sxs-lookup"><span data-stu-id="849dc-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="849dc-133">请求</span><span class="sxs-lookup"><span data-stu-id="849dc-133">Request</span></span>

<span data-ttu-id="849dc-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="849dc-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="849dc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="849dc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceroles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/15d889df-3eb8-4e9b-bfb4-b1908849aec4/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%27a35bef72-a8aa-4ca3-af30-f6b2ece7208f%27)&$expand=accessPackageResource
```
# <a name="c"></a>[<span data-ttu-id="849dc-136">C#</span><span class="sxs-lookup"><span data-stu-id="849dc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourceroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="849dc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="849dc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourceroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="849dc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="849dc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourceroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="849dc-139">Java</span><span class="sxs-lookup"><span data-stu-id="849dc-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourceroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="849dc-140">响应</span><span class="sxs-lookup"><span data-stu-id="849dc-140">Response</span></span>

<span data-ttu-id="849dc-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="849dc-141">The following is an example of the response.</span></span>

> <span data-ttu-id="849dc-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="849dc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


