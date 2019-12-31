---
title: 列出 accessPackageResourceRoles
description: 检索 accessPackageResourceRole 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 435f093173e112324e02987826b42b17a8c18138
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911635"
---
# <a name="list-accesspackageresourceroles"></a><span data-ttu-id="808aa-103">列出 accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="808aa-103">List accessPackageResourceRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="808aa-104">在[accessPackageCatalog](../resources/accesspackagecatalog.md)中检索[accessPackageResource](../resources/accesspackageresource.md)的[accessPackageResourceRole](../resources/accesspackageresourcerole.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="808aa-104">Retrieve a list of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects of an [accessPackageResource](../resources/accesspackageresource.md) in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>  <span data-ttu-id="808aa-105">然后，调用方可以使用此角色列表来选择角色，在随后[创建 accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md)时需要该角色。</span><span class="sxs-lookup"><span data-stu-id="808aa-105">This list of roles can then be used by the caller to select a role, which is needed when subsequently [creating an accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="808aa-106">权限</span><span class="sxs-lookup"><span data-stu-id="808aa-106">Permissions</span></span>

<span data-ttu-id="808aa-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="808aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="808aa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="808aa-109">Permission type</span></span>                        | <span data-ttu-id="808aa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="808aa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="808aa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="808aa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="808aa-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="808aa-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="808aa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="808aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="808aa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="808aa-114">Not supported.</span></span> |
| <span data-ttu-id="808aa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="808aa-115">Application</span></span>                            | <span data-ttu-id="808aa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="808aa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="808aa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="808aa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{catalogId}/accessPackageResourceRoles?$filter=(originSystem+eq+%27{originSystemType}%27+and+accessPackageResource/id+eq+%27{resourceId}%27)&$expand=accessPackageResource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="808aa-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="808aa-118">Optional query parameters</span></span>

<span data-ttu-id="808aa-119">此方法使用 OData 查询参数构造响应。</span><span class="sxs-lookup"><span data-stu-id="808aa-119">This method uses OData query parameters to construct the response.</span></span> <span data-ttu-id="808aa-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="808aa-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="808aa-121">请求头</span><span class="sxs-lookup"><span data-stu-id="808aa-121">Request headers</span></span>

| <span data-ttu-id="808aa-122">名称</span><span class="sxs-lookup"><span data-stu-id="808aa-122">Name</span></span>      |<span data-ttu-id="808aa-123">说明</span><span class="sxs-lookup"><span data-stu-id="808aa-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="808aa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="808aa-124">Authorization</span></span> | <span data-ttu-id="808aa-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="808aa-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="808aa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="808aa-127">Request body</span></span>

<span data-ttu-id="808aa-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="808aa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="808aa-129">响应</span><span class="sxs-lookup"><span data-stu-id="808aa-129">Response</span></span>

<span data-ttu-id="808aa-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[accessPackageResourceRole](../resources/accesspackageresourcerole.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="808aa-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="808aa-131">示例</span><span class="sxs-lookup"><span data-stu-id="808aa-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="808aa-132">请求</span><span class="sxs-lookup"><span data-stu-id="808aa-132">Request</span></span>

<span data-ttu-id="808aa-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="808aa-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="808aa-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="808aa-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceroles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/15d889df-3eb8-4e9b-bfb4-b1908849aec4/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%27a35bef72-a8aa-4ca3-af30-f6b2ece7208f%27)&$expand=accessPackageResource
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="808aa-135">C#</span><span class="sxs-lookup"><span data-stu-id="808aa-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourceroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="808aa-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="808aa-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourceroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="808aa-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="808aa-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourceroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="808aa-138">响应</span><span class="sxs-lookup"><span data-stu-id="808aa-138">Response</span></span>

<span data-ttu-id="808aa-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="808aa-139">The following is an example of the response.</span></span>

> <span data-ttu-id="808aa-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="808aa-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
