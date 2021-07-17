---
title: 创建 accessPackageResourceRoleScope
description: 创建新的 accessPackageResourceRoleScope，以将资源角色添加到访问包。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6b4abe2f9c2c0060e97560a26c22d19ed53e01b7
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53466958"
---
# <a name="create-accesspackageresourcerolescope"></a><span data-ttu-id="47025-103">创建 accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="47025-103">Create accessPackageResourceRoleScope</span></span>

<span data-ttu-id="47025-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47025-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47025-105">创建新的 [accessPackageResourceRoleScope，](../resources/accesspackageresourcerolescope.md) 以将资源角色添加到访问包。</span><span class="sxs-lookup"><span data-stu-id="47025-105">Create a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) for adding a resource role to an access package.</span></span> <span data-ttu-id="47025-106">访问包资源（对于组、应用或 SharePoint Online 网站）必须已存在于访问包目录中，并且资源角色的 **originId** 从资源角色列表中 [检索](accesspackagecatalog-list-accesspackageresourceroles.md)。</span><span class="sxs-lookup"><span data-stu-id="47025-106">The access package resource, for a group, an app, or a SharePoint Online site, must already exist in the access package catalog, and the **originId** for the resource role retrieved from the [list of the resource roles](accesspackagecatalog-list-accesspackageresourceroles.md).</span></span> <span data-ttu-id="47025-107">将资源角色作用域添加到访问包后，用户通过任何当前和将来的访问包分配接收此资源角色。</span><span class="sxs-lookup"><span data-stu-id="47025-107">Once you add the resource role scope to the access package, the user will receive this resource role through any current and future access package assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="47025-108">权限</span><span class="sxs-lookup"><span data-stu-id="47025-108">Permissions</span></span>

<span data-ttu-id="47025-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47025-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="47025-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="47025-111">Permission type</span></span>                        | <span data-ttu-id="47025-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="47025-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="47025-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47025-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="47025-114">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47025-114">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="47025-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47025-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47025-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="47025-116">Not supported.</span></span> |
| <span data-ttu-id="47025-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="47025-117">Application</span></span>                            | <span data-ttu-id="47025-118">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47025-118">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47025-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47025-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes
```

## <a name="request-headers"></a><span data-ttu-id="47025-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="47025-120">Request headers</span></span>

| <span data-ttu-id="47025-121">名称</span><span class="sxs-lookup"><span data-stu-id="47025-121">Name</span></span>          | <span data-ttu-id="47025-122">说明</span><span class="sxs-lookup"><span data-stu-id="47025-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="47025-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="47025-123">Authorization</span></span> | <span data-ttu-id="47025-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="47025-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="47025-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="47025-126">Content-Type</span></span>  | <span data-ttu-id="47025-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="47025-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47025-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="47025-129">Request body</span></span>

<span data-ttu-id="47025-130">在请求正文中，提供 [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47025-130">In the request body, supply a JSON representation of an [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.</span></span>  <span data-ttu-id="47025-131">在 对象中包括[与 accessPackageResourceRole](../resources/accesspackageresourcerole.md)对象的关系（可以从列出目录中资源的访问包资源角色的请求[](accesspackagecatalog-list-accesspackageresourceroles.md)获取）和[accessPackageResourceScope](../resources/accesspackageresourcescope.md)对象（可以从请求获取，以使用 列出[访问](accesspackagecatalog-list-accesspackageresources.md)包资源 `$expand=accessPackageResourceScopes` ）</span><span class="sxs-lookup"><span data-stu-id="47025-131">Include in the object the relationships to an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object, which can be obtained from a request to [list access package resource roles of a resource in a catalog](accesspackagecatalog-list-accesspackageresourceroles.md), and an [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object, which can be obtained from a request to [list access package resources](accesspackagecatalog-list-accesspackageresources.md) with `$expand=accessPackageResourceScopes`.</span></span>

## <a name="response"></a><span data-ttu-id="47025-132">响应</span><span class="sxs-lookup"><span data-stu-id="47025-132">Response</span></span>

<span data-ttu-id="47025-133">如果成功，此方法在响应正文中返回 200 系列响应代码和新 [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="47025-133">If successful, this method returns a 200-series response code and a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47025-134">示例</span><span class="sxs-lookup"><span data-stu-id="47025-134">Examples</span></span>

### <a name="example-1-add-group-membership-as-a-resource-role-to-an-access-package"></a><span data-ttu-id="47025-135">示例 1：将组成员身份作为资源角色添加到访问包</span><span class="sxs-lookup"><span data-stu-id="47025-135">Example 1: Add group membership as a resource role to an access package</span></span>

#### <a name="request"></a><span data-ttu-id="47025-136">请求</span><span class="sxs-lookup"><span data-stu-id="47025-136">Request</span></span>

<span data-ttu-id="47025-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="47025-137">The following is an example of the request.</span></span>  <span data-ttu-id="47025-138">在此请求之前，该组的访问包资源必须已添加到包含此访问包的访问 `1d08498d-72a1-403f-8511-6b1f875746a0` `b31fe1f1-3651-488f-bd9a-1711887fd4ca` 包目录中。</span><span class="sxs-lookup"><span data-stu-id="47025-138">Prior to this request, the access package resource `1d08498d-72a1-403f-8511-6b1f875746a0` for the group `b31fe1f1-3651-488f-bd9a-1711887fd4ca` must already have been added to the access package catalog containing this access package.</span></span>  <span data-ttu-id="47025-139">资源可以通过创建访问包资源请求 添加到 [目录中](accesspackageresourcerequest-post.md)。</span><span class="sxs-lookup"><span data-stu-id="47025-139">The resource could have been added to the catalog by [creating an access package resource request](accesspackageresourcerequest-post.md).</span></span>

# <a name="http"></a>[<span data-ttu-id="47025-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="47025-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerolescope_from_accesspackage"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes
Content-type: application/json

{
  "accessPackageResourceRole":{
    "originId":"Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca",
    "displayName":"Member",
    "originSystem":"AadGroup",
    "accessPackageResource":{"id":"1d08498d-72a1-403f-8511-6b1f875746a0","resourceType":"O365 Group","originId":"b31fe1f1-3651-488f-bd9a-1711887fd4ca","originSystem":"AadGroup"}
  },
 "accessPackageResourceScope":{
   "originId":"b31fe1f1-3651-488f-bd9a-1711887fd4ca","originSystem":"AadGroup"
 }
}
```
# <a name="c"></a>[<span data-ttu-id="47025-141">C#</span><span class="sxs-lookup"><span data-stu-id="47025-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerolescope-from-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47025-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47025-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerolescope-from-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47025-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47025-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerolescope-from-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47025-144">Java</span><span class="sxs-lookup"><span data-stu-id="47025-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerolescope-from-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="47025-145">响应</span><span class="sxs-lookup"><span data-stu-id="47025-145">Response</span></span>

<span data-ttu-id="47025-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="47025-146">The following is an example of the response.</span></span>

> <span data-ttu-id="47025-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="47025-147">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageResourceRoleScopes/$entity",
    "id": "ad5c7636-e481-4528-991f-198e3b38dd56_ffd4004a-f4a9-4b22-b027-759e55c0d1db",
    "createdBy": "admin@example.com",
    "createdDateTime": "2019-12-11T01:35:26.4754081Z",
    "modifiedBy": "admin@example.com",
    "modifiedDateTime": "2019-12-11T01:35:26.4754081Z"
}
```

### <a name="example-2-add-a-sharepoint-online-site-role-to-an-access-package"></a><span data-ttu-id="47025-148">示例 2：将 SharePoint Online 网站角色添加到访问包</span><span class="sxs-lookup"><span data-stu-id="47025-148">Example 2: Add a SharePoint Online site role to an access package</span></span>

#### <a name="request"></a><span data-ttu-id="47025-149">请求</span><span class="sxs-lookup"><span data-stu-id="47025-149">Request</span></span>

<span data-ttu-id="47025-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="47025-150">The following is an example of the request.</span></span>  <span data-ttu-id="47025-151">网站的访问包资源必须已添加到包含此访问包的访问包目录中。</span><span class="sxs-lookup"><span data-stu-id="47025-151">The access package resource for the site must already have been added to the access package catalog containing this access package.</span></span>


# <a name="http"></a>[<span data-ttu-id="47025-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="47025-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerolescope_from_accesspackage2"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes
Content-type: application/json

{
    "accessPackageResourceRole": {
        "originId": "4",
        "originSystem": "SharePointOnline",
        "accessPackageResource": {
            "id": "53c71803-a0a8-4777-aecc-075de8ee3991"
        }
    },
    "accessPackageResourceScope": {
        "id": "5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33",
        "originId": "https://microsoft.sharepoint.com/portals/Community",
        "originSystem": "SharePointOnline"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="47025-153">C#</span><span class="sxs-lookup"><span data-stu-id="47025-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerolescope-from-accesspackage2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47025-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47025-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerolescope-from-accesspackage2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47025-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47025-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerolescope-from-accesspackage2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47025-156">Java</span><span class="sxs-lookup"><span data-stu-id="47025-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerolescope-from-accesspackage2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="47025-157">响应</span><span class="sxs-lookup"><span data-stu-id="47025-157">Response</span></span>

<span data-ttu-id="47025-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="47025-158">The following is an example of the response.</span></span>

> <span data-ttu-id="47025-159">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="47025-159">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "id": "6646a29e-da03-49f6-bcd9-dec124492de3_5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageResourceRoleScope",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
