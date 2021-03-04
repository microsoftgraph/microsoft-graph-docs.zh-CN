---
title: 创建 accessPackageResourceRoleScope
description: 创建新的 accessPackageResourceRoleScope，以将资源角色添加到访问包。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ffaedc45cc512b554fda3ce4dd06794fba716b16
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439805"
---
# <a name="create-accesspackageresourcerolescope"></a><span data-ttu-id="c22c6-103">创建 accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="c22c6-103">Create accessPackageResourceRoleScope</span></span>

<span data-ttu-id="c22c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c22c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c22c6-105">创建新的 [accessPackageResourceRoleScope，](../resources/accesspackageresourcerolescope.md) 用于向访问包添加资源角色。</span><span class="sxs-lookup"><span data-stu-id="c22c6-105">Create a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) for adding a resource role to an access package.</span></span>  <span data-ttu-id="c22c6-106">访问包资源必须已存在于访问包目录中。</span><span class="sxs-lookup"><span data-stu-id="c22c6-106">The access package resource must already exist in the access package catalog.</span></span>  <span data-ttu-id="c22c6-107">对此访问包的任何后续访问包分配请求都将包含此资源角色。</span><span class="sxs-lookup"><span data-stu-id="c22c6-107">Any subsequent access package assignment requests to this access package will include this resource role.</span></span>  

## <a name="permissions"></a><span data-ttu-id="c22c6-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="c22c6-108">Permissions</span></span>

<span data-ttu-id="c22c6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c22c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c22c6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c22c6-111">Permission type</span></span>                        | <span data-ttu-id="c22c6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c22c6-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c22c6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c22c6-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c22c6-114">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c22c6-114">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="c22c6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c22c6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c22c6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c22c6-116">Not supported.</span></span> |
| <span data-ttu-id="c22c6-117">Application</span><span class="sxs-lookup"><span data-stu-id="c22c6-117">Application</span></span>                            | <span data-ttu-id="c22c6-118">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c22c6-118">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c22c6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c22c6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes
```

## <a name="request-headers"></a><span data-ttu-id="c22c6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c22c6-120">Request headers</span></span>

| <span data-ttu-id="c22c6-121">名称</span><span class="sxs-lookup"><span data-stu-id="c22c6-121">Name</span></span>          | <span data-ttu-id="c22c6-122">说明</span><span class="sxs-lookup"><span data-stu-id="c22c6-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c22c6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c22c6-123">Authorization</span></span> | <span data-ttu-id="c22c6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c22c6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c22c6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c22c6-126">Content-Type</span></span>  | <span data-ttu-id="c22c6-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c22c6-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c22c6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c22c6-129">Request body</span></span>

<span data-ttu-id="c22c6-130">在请求正文中，提供 [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c22c6-130">In the request body, supply a JSON representation of an [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.</span></span>  <span data-ttu-id="c22c6-131">在对象中包括 [与 accessPackageResourceRole](../resources/accesspackageresourcerole.md) 和 [accessPackageResourceScope 的关系](../resources/accesspackageresourcescope.md)。</span><span class="sxs-lookup"><span data-stu-id="c22c6-131">Include in the object the relationships to an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) and [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span></span>  

## <a name="response"></a><span data-ttu-id="c22c6-132">响应</span><span class="sxs-lookup"><span data-stu-id="c22c6-132">Response</span></span>

<span data-ttu-id="c22c6-133">如果成功，此方法在响应正文中返回 200 系列响应代码和新的 [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c22c6-133">If successful, this method returns a 200-series response code and a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c22c6-134">示例</span><span class="sxs-lookup"><span data-stu-id="c22c6-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c22c6-135">请求</span><span class="sxs-lookup"><span data-stu-id="c22c6-135">Request</span></span>

<span data-ttu-id="c22c6-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c22c6-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c22c6-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c22c6-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c22c6-138">C#</span><span class="sxs-lookup"><span data-stu-id="c22c6-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerolescope-from-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c22c6-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c22c6-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerolescope-from-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c22c6-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c22c6-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerolescope-from-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c22c6-141">Java</span><span class="sxs-lookup"><span data-stu-id="c22c6-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerolescope-from-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c22c6-142">响应</span><span class="sxs-lookup"><span data-stu-id="c22c6-142">Response</span></span>

<span data-ttu-id="c22c6-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c22c6-143">The following is an example of the response.</span></span>

> <span data-ttu-id="c22c6-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c22c6-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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


