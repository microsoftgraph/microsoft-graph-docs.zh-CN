---
title: 创建 accessPackageResourceRoleScope
description: 创建新的 accessPackageResourceRoleScope，用于将资源角色添加到访问包中。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 21111e91d87d3ff70f8edb8de826c87310b99007
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952317"
---
# <a name="create-accesspackageresourcerolescope"></a><span data-ttu-id="fbee4-103">创建 accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="fbee4-103">Create accessPackageResourceRoleScope</span></span>

<span data-ttu-id="fbee4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbee4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbee4-105">创建新的 [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) ，用于将资源角色添加到访问包中。</span><span class="sxs-lookup"><span data-stu-id="fbee4-105">Create a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) for adding a resource role to an access package.</span></span>  <span data-ttu-id="fbee4-106">访问包资源必须已存在于访问包目录中。</span><span class="sxs-lookup"><span data-stu-id="fbee4-106">The access package resource must already exist in the access package catalog.</span></span>  <span data-ttu-id="fbee4-107">对此访问包的任何后续访问包分配请求都将包含此资源角色。</span><span class="sxs-lookup"><span data-stu-id="fbee4-107">Any subsequent access package assignment requests to this access package will include this resource role.</span></span>  

## <a name="permissions"></a><span data-ttu-id="fbee4-108">权限</span><span class="sxs-lookup"><span data-stu-id="fbee4-108">Permissions</span></span>

<span data-ttu-id="fbee4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fbee4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fbee4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fbee4-111">Permission type</span></span>                        | <span data-ttu-id="fbee4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fbee4-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fbee4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fbee4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="fbee4-114">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbee4-114">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="fbee4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fbee4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbee4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbee4-116">Not supported.</span></span> |
| <span data-ttu-id="fbee4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fbee4-117">Application</span></span>                            | <span data-ttu-id="fbee4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbee4-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbee4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fbee4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes
```

## <a name="request-headers"></a><span data-ttu-id="fbee4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fbee4-120">Request headers</span></span>

| <span data-ttu-id="fbee4-121">名称</span><span class="sxs-lookup"><span data-stu-id="fbee4-121">Name</span></span>          | <span data-ttu-id="fbee4-122">说明</span><span class="sxs-lookup"><span data-stu-id="fbee4-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fbee4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbee4-123">Authorization</span></span> | <span data-ttu-id="fbee4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fbee4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fbee4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fbee4-126">Content-Type</span></span>  | <span data-ttu-id="fbee4-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="fbee4-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fbee4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="fbee4-129">Request body</span></span>

<span data-ttu-id="fbee4-130">在请求正文中，提供 [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fbee4-130">In the request body, supply a JSON representation of an [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.</span></span>  <span data-ttu-id="fbee4-131">在对象中包含与 [accessPackageResourceRole](../resources/accesspackageresourcerole.md) 和 [accessPackageResourceScope](../resources/accesspackageresourcescope.md)的关系。</span><span class="sxs-lookup"><span data-stu-id="fbee4-131">Include in the object the relationships to an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) and [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span></span>  

## <a name="response"></a><span data-ttu-id="fbee4-132">响应</span><span class="sxs-lookup"><span data-stu-id="fbee4-132">Response</span></span>

<span data-ttu-id="fbee4-133">如果成功，此方法在响应正文中返回一个200系列响应代码和一个新的 [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fbee4-133">If successful, this method returns a 200-series response code and a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fbee4-134">示例</span><span class="sxs-lookup"><span data-stu-id="fbee4-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fbee4-135">请求</span><span class="sxs-lookup"><span data-stu-id="fbee4-135">Request</span></span>

<span data-ttu-id="fbee4-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fbee4-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fbee4-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="fbee4-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fbee4-138">C#</span><span class="sxs-lookup"><span data-stu-id="fbee4-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerolescope-from-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fbee4-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fbee4-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerolescope-from-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fbee4-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fbee4-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerolescope-from-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fbee4-141">Java</span><span class="sxs-lookup"><span data-stu-id="fbee4-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerolescope-from-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fbee4-142">响应</span><span class="sxs-lookup"><span data-stu-id="fbee4-142">Response</span></span>

<span data-ttu-id="fbee4-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fbee4-143">The following is an example of the response.</span></span>

> <span data-ttu-id="fbee4-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fbee4-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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


