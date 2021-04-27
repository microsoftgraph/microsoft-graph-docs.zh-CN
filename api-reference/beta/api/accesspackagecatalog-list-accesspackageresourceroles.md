---
title: 列出 accessPackageResourceRoles
description: 检索 accessPackageResourceRole 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 29e83c3254cfa4931f3faeb869d6312335565019
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048566"
---
# <a name="list-accesspackageresourceroles"></a><span data-ttu-id="34e7c-103">列出 accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="34e7c-103">List accessPackageResourceRoles</span></span>

<span data-ttu-id="34e7c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34e7c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34e7c-105">在[accessPackageCatalog](../resources/accesspackagecatalog.md)中检索[accessPackageResource 的 accessPackageResourceRole](../resources/accesspackageresourcerole.md)对象列表。 [](../resources/accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="34e7c-105">Retrieve a list of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects of an [accessPackageResource](../resources/accesspackageresource.md) in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>  <span data-ttu-id="34e7c-106">然后，调用方可以使用此角色列表来选择角色，随后创建 [accessPackageResourceRoleScope 时需要此角色](accesspackage-post-accesspackageresourcerolescopes.md)。</span><span class="sxs-lookup"><span data-stu-id="34e7c-106">This list of roles can then be used by the caller to select a role, which is needed when subsequently [creating an accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="34e7c-107">权限</span><span class="sxs-lookup"><span data-stu-id="34e7c-107">Permissions</span></span>

<span data-ttu-id="34e7c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34e7c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="34e7c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="34e7c-110">Permission type</span></span>                        | <span data-ttu-id="34e7c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="34e7c-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="34e7c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34e7c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="34e7c-113">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34e7c-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="34e7c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34e7c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34e7c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="34e7c-115">Not supported.</span></span> |
| <span data-ttu-id="34e7c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="34e7c-116">Application</span></span>                            | <span data-ttu-id="34e7c-117">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34e7c-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="34e7c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34e7c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{catalogId}/accessPackageResourceRoles?$filter=(originSystem+eq+%27{originSystemType}%27+and+accessPackageResource/id+eq+%27{resourceId}%27)&$expand=accessPackageResource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="34e7c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="34e7c-119">Optional query parameters</span></span>

<span data-ttu-id="34e7c-120">此方法使用 OData 查询参数构造响应。</span><span class="sxs-lookup"><span data-stu-id="34e7c-120">This method uses OData query parameters to construct the response.</span></span> <span data-ttu-id="34e7c-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="34e7c-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="34e7c-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="34e7c-122">Request headers</span></span>

| <span data-ttu-id="34e7c-123">名称</span><span class="sxs-lookup"><span data-stu-id="34e7c-123">Name</span></span>      |<span data-ttu-id="34e7c-124">说明</span><span class="sxs-lookup"><span data-stu-id="34e7c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="34e7c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="34e7c-125">Authorization</span></span> | <span data-ttu-id="34e7c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="34e7c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34e7c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="34e7c-128">Request body</span></span>

<span data-ttu-id="34e7c-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="34e7c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34e7c-130">响应</span><span class="sxs-lookup"><span data-stu-id="34e7c-130">Response</span></span>

<span data-ttu-id="34e7c-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackageResourceRole](../resources/accesspackageresourcerole.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="34e7c-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="34e7c-132">示例</span><span class="sxs-lookup"><span data-stu-id="34e7c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="34e7c-133">请求</span><span class="sxs-lookup"><span data-stu-id="34e7c-133">Request</span></span>

<span data-ttu-id="34e7c-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="34e7c-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="34e7c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="34e7c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceroles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/15d889df-3eb8-4e9b-bfb4-b1908849aec4/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%27a35bef72-a8aa-4ca3-af30-f6b2ece7208f%27)&$expand=accessPackageResource
```
# <a name="c"></a>[<span data-ttu-id="34e7c-136">C#</span><span class="sxs-lookup"><span data-stu-id="34e7c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourceroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="34e7c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34e7c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourceroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="34e7c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34e7c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourceroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="34e7c-139">Java</span><span class="sxs-lookup"><span data-stu-id="34e7c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourceroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="34e7c-140">响应</span><span class="sxs-lookup"><span data-stu-id="34e7c-140">Response</span></span>

<span data-ttu-id="34e7c-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="34e7c-141">The following is an example of the response.</span></span>

> <span data-ttu-id="34e7c-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="34e7c-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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


