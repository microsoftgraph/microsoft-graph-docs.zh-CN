---
title: 创建 accessPackageResourceRoleScope
description: 创建新的 accessPackageResourceRoleScope，用于将资源角色添加到访问包中。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a05af5bb3290a17b8e732b75f771977c5126b368
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911569"
---
# <a name="create-accesspackageresourcerolescope"></a><span data-ttu-id="f7113-103">创建 accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="f7113-103">Create accessPackageResourceRoleScope</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7113-104">创建新的[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) ，用于将资源角色添加到访问包中。</span><span class="sxs-lookup"><span data-stu-id="f7113-104">Create a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) for adding a resource role to an access package.</span></span>  <span data-ttu-id="f7113-105">访问包资源必须已存在于访问包目录中。</span><span class="sxs-lookup"><span data-stu-id="f7113-105">The access package resource must already exist in the access package catalog.</span></span>  <span data-ttu-id="f7113-106">对此访问包的任何后续访问包分配请求都将包含此资源角色。</span><span class="sxs-lookup"><span data-stu-id="f7113-106">Any subsequent access package assignment requests to this access package will include this resource role.</span></span>  

## <a name="permissions"></a><span data-ttu-id="f7113-107">权限</span><span class="sxs-lookup"><span data-stu-id="f7113-107">Permissions</span></span>

<span data-ttu-id="f7113-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7113-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7113-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7113-110">Permission type</span></span>                        | <span data-ttu-id="f7113-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7113-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f7113-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7113-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7113-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7113-113">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="f7113-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7113-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7113-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7113-115">Not supported.</span></span> |
| <span data-ttu-id="f7113-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7113-116">Application</span></span>                            | <span data-ttu-id="f7113-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7113-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7113-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7113-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes
```

## <a name="request-headers"></a><span data-ttu-id="f7113-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7113-119">Request headers</span></span>

| <span data-ttu-id="f7113-120">名称</span><span class="sxs-lookup"><span data-stu-id="f7113-120">Name</span></span>          | <span data-ttu-id="f7113-121">说明</span><span class="sxs-lookup"><span data-stu-id="f7113-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f7113-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7113-122">Authorization</span></span> | <span data-ttu-id="f7113-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7113-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7113-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7113-125">Content-Type</span></span>  | <span data-ttu-id="f7113-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f7113-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7113-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7113-128">Request body</span></span>

<span data-ttu-id="f7113-129">在请求正文中，提供[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7113-129">In the request body, supply a JSON representation of an [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.</span></span>  <span data-ttu-id="f7113-130">在对象中包含与[accessPackageResourceRole](../resources/accesspackageresourcerole.md)和[accessPackageResourceScope](../resources/accesspackageresourcescope.md)的关系。</span><span class="sxs-lookup"><span data-stu-id="f7113-130">Include in the object the relationships to an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) and [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span></span>  

## <a name="response"></a><span data-ttu-id="f7113-131">响应</span><span class="sxs-lookup"><span data-stu-id="f7113-131">Response</span></span>

<span data-ttu-id="f7113-132">如果成功，此方法在响应正文中返回一个200系列响应代码和一个新的[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f7113-132">If successful, this method returns a 200-series response code and a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7113-133">示例</span><span class="sxs-lookup"><span data-stu-id="f7113-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7113-134">请求</span><span class="sxs-lookup"><span data-stu-id="f7113-134">Request</span></span>

<span data-ttu-id="f7113-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f7113-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f7113-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7113-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f7113-137">C#</span><span class="sxs-lookup"><span data-stu-id="f7113-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerolescope-from-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7113-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7113-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerolescope-from-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f7113-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7113-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerolescope-from-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f7113-140">响应</span><span class="sxs-lookup"><span data-stu-id="f7113-140">Response</span></span>

<span data-ttu-id="f7113-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f7113-141">The following is an example of the response.</span></span>

> <span data-ttu-id="f7113-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f7113-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageResourceRoleScope",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
