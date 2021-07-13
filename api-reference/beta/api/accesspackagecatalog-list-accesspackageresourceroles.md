---
title: 列出 accessPackageResourceRoles
description: 检索 accessPackageResourceRole 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2facea352db9eb04265aaf6b86e77b89249631c3
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400997"
---
# <a name="list-accesspackageresourceroles"></a><span data-ttu-id="83e98-103">列出 accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="83e98-103">List accessPackageResourceRoles</span></span>

<span data-ttu-id="83e98-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83e98-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83e98-105">在[accessPackageCatalog](../resources/accesspackagecatalog.md)中检索[accessPackageResource 的 accessPackageResourceRole](../resources/accesspackageresourcerole.md)对象列表。 [](../resources/accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="83e98-105">Retrieve a list of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects of an [accessPackageResource](../resources/accesspackageresource.md) in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span> <span data-ttu-id="83e98-106">资源应该已经通过创建 [accessPackageResourceRequest](accesspackageresourcerequest-post.md)添加到目录中。</span><span class="sxs-lookup"><span data-stu-id="83e98-106">The resource should have been added to the catalog by [creating an accessPackageResourceRequest](accesspackageresourcerequest-post.md).</span></span> <span data-ttu-id="83e98-107">然后，调用方可以使用此角色列表来选择角色，随后创建 [accessPackageResourceRoleScope 时需要此角色](accesspackage-post-accesspackageresourcerolescopes.md)。</span><span class="sxs-lookup"><span data-stu-id="83e98-107">This list of roles can then be used by the caller to select a role, which is needed when subsequently [creating an accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="83e98-108">权限</span><span class="sxs-lookup"><span data-stu-id="83e98-108">Permissions</span></span>

<span data-ttu-id="83e98-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83e98-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83e98-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="83e98-111">Permission type</span></span>                        | <span data-ttu-id="83e98-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="83e98-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="83e98-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83e98-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="83e98-114">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83e98-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="83e98-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83e98-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83e98-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="83e98-116">Not supported.</span></span> |
| <span data-ttu-id="83e98-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="83e98-117">Application</span></span>                            | <span data-ttu-id="83e98-118">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83e98-118">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83e98-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83e98-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{catalogId}/accessPackageResourceRoles?$filter=(originSystem+eq+%27{originSystemType}%27+and+accessPackageResource/id+eq+%27{resourceId}%27)&$expand=accessPackageResource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="83e98-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="83e98-120">Optional query parameters</span></span>

<span data-ttu-id="83e98-121">此方法使用 OData 查询参数构造响应。</span><span class="sxs-lookup"><span data-stu-id="83e98-121">This method uses OData query parameters to construct the response.</span></span> <span data-ttu-id="83e98-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="83e98-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="83e98-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="83e98-123">Request headers</span></span>

| <span data-ttu-id="83e98-124">名称</span><span class="sxs-lookup"><span data-stu-id="83e98-124">Name</span></span>      |<span data-ttu-id="83e98-125">说明</span><span class="sxs-lookup"><span data-stu-id="83e98-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="83e98-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="83e98-126">Authorization</span></span> | <span data-ttu-id="83e98-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="83e98-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83e98-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="83e98-129">Request body</span></span>

<span data-ttu-id="83e98-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="83e98-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83e98-131">响应</span><span class="sxs-lookup"><span data-stu-id="83e98-131">Response</span></span>

<span data-ttu-id="83e98-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackageResourceRole](../resources/accesspackageresourcerole.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="83e98-132">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83e98-133">示例</span><span class="sxs-lookup"><span data-stu-id="83e98-133">Examples</span></span>

### <a name="example-1-retrieving-the-roles-of-a-resource-for-a-group"></a><span data-ttu-id="83e98-134">示例 1：检索组的资源的角色</span><span class="sxs-lookup"><span data-stu-id="83e98-134">Example 1: Retrieving the roles of a resource for a group</span></span>

#### <a name="request"></a><span data-ttu-id="83e98-135">请求</span><span class="sxs-lookup"><span data-stu-id="83e98-135">Request</span></span>

<span data-ttu-id="83e98-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="83e98-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="83e98-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="83e98-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceroles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/15d889df-3eb8-4e9b-bfb4-b1908849aec4/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%27a35bef72-a8aa-4ca3-af30-f6b2ece7208f%27)&$expand=accessPackageResource
```
# <a name="c"></a>[<span data-ttu-id="83e98-138">C#</span><span class="sxs-lookup"><span data-stu-id="83e98-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourceroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83e98-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83e98-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourceroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83e98-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83e98-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourceroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="83e98-141">Java</span><span class="sxs-lookup"><span data-stu-id="83e98-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourceroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="83e98-142">响应</span><span class="sxs-lookup"><span data-stu-id="83e98-142">Response</span></span>

<span data-ttu-id="83e98-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="83e98-143">The following is an example of the response.</span></span>

> <span data-ttu-id="83e98-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="83e98-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-retrieve-the-roles-of-a-resource-for-a-sharepoint-online-site"></a><span data-ttu-id="83e98-145">示例 2：检索 SharePoint Online 网站的资源角色</span><span class="sxs-lookup"><span data-stu-id="83e98-145">Example 2: Retrieve the roles of a resource for a SharePoint Online site</span></span>

<span data-ttu-id="83e98-146">这是检索资源的角色以获取每个角色的 **originId** 的示例。</span><span class="sxs-lookup"><span data-stu-id="83e98-146">This is an example of retrieving the roles of a resource, to obtain the **originId** of each role.</span></span>  <span data-ttu-id="83e98-147">在将 SharePoint Online 网站作为资源添加到目录后，这将使用，因为需要角色的 **originId** 才能将角色添加到访问包。</span><span class="sxs-lookup"><span data-stu-id="83e98-147">This would be used after a SharePoint Online site has been added as a resource to the catalog, as the **originId** of a role is needed to add the role to an access package.</span></span>

#### <a name="request"></a><span data-ttu-id="83e98-148">请求</span><span class="sxs-lookup"><span data-stu-id="83e98-148">Request</span></span>

<span data-ttu-id="83e98-149">下面是一个请求示例，用于检索特定资源 **53c71803-a0a8-4777-aecc-075de8ee3991** 的角色，该资源具有 **SharePointOnline** 的 **originSystem，** 位于目录 **beedadfe-01d5-4025-910b-84abb9369997 中**。</span><span class="sxs-lookup"><span data-stu-id="83e98-149">The following is an example of the request, to retrieve the roles of a particular resource **53c71803-a0a8-4777-aecc-075de8ee3991** which has an **originSystem** of **SharePointOnline** and is located in catalog **beedadfe-01d5-4025-910b-84abb9369997**.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceroles2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/beedadfe-01d5-4025-910b-84abb9369997/accessPackageResourceRoles?$filter=(originSystem+eq+%27SharePointOnline%27+and+accessPackageResource/id+eq+%2753c71803-a0a8-4777-aecc-075de8ee3991%27)&$select=displayName,originId
```



#### <a name="response"></a><span data-ttu-id="83e98-150">响应</span><span class="sxs-lookup"><span data-stu-id="83e98-150">Response</span></span>

<span data-ttu-id="83e98-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="83e98-151">The following is an example of the response.</span></span>  <span data-ttu-id="83e98-152">**displayName** 与网站的 SharePoint Online 视图中显示的相同 **，originId** 是由 SharePoint Online 为角色建立的基础标识符。</span><span class="sxs-lookup"><span data-stu-id="83e98-152">The **displayName** is the same as shown in the SharePoint Online view of a site, and the **originId** is the underlying identifier established by SharePoint Online for the role.</span></span>

> <span data-ttu-id="83e98-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="83e98-153">**Note:** The response object shown here might be shortened for readability.</span></span>

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
        "displayName": "Contributors",
        "originId": "4"
    },
    {
        "displayName": "Creators",
        "originId": "3"
    },
    {
        "displayName": "Viewers",
        "originId": "5"
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
