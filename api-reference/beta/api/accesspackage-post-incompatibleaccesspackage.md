---
title: 将 accessPackage 添加到 incompatibleAccessPackages
description: 添加链接以指示访问包与指定的访问包不兼容。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 4ddb6953346a5ea571a480dc073e29dca14cca31
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439826"
---
# <a name="add-accesspackage-to-incompatibleaccesspackages"></a><span data-ttu-id="7b15c-103">将 accessPackage 添加到 incompatibleAccessPackages</span><span class="sxs-lookup"><span data-stu-id="7b15c-103">Add accessPackage to incompatibleAccessPackages</span></span>

<span data-ttu-id="7b15c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b15c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b15c-105">将 [accessPackage 添加到 accessPackage](../resources/accesspackage.md) 上标记为不兼容的访问 [包列表](../resources/accesspackage.md)。</span><span class="sxs-lookup"><span data-stu-id="7b15c-105">Add an [accessPackage](../resources/accesspackage.md) to the list of access packages that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="7b15c-106">权限</span><span class="sxs-lookup"><span data-stu-id="7b15c-106">Permissions</span></span>

<span data-ttu-id="7b15c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b15c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b15c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b15c-109">Permission type</span></span>                        | <span data-ttu-id="7b15c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b15c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7b15c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b15c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b15c-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b15c-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="7b15c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b15c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b15c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b15c-114">Not supported.</span></span> |
| <span data-ttu-id="7b15c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b15c-115">Application</span></span>                            | <span data-ttu-id="7b15c-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b15c-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b15c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b15c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/$ref
```

## <a name="request-headers"></a><span data-ttu-id="7b15c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b15c-118">Request headers</span></span>

| <span data-ttu-id="7b15c-119">名称</span><span class="sxs-lookup"><span data-stu-id="7b15c-119">Name</span></span>          | <span data-ttu-id="7b15c-120">说明</span><span class="sxs-lookup"><span data-stu-id="7b15c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7b15c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b15c-121">Authorization</span></span> | <span data-ttu-id="7b15c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7b15c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7b15c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b15c-124">Content-Type</span></span>  | <span data-ttu-id="7b15c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7b15c-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7b15c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b15c-127">Request body</span></span>

<span data-ttu-id="7b15c-128">在请求正文中，使用 [accessPackage](../resources/accesspackage.md) 对象的 URI 的 OData ID 提供结构的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b15c-128">In the request body, supply a JSON representation of a structure with the OData id of the URI of an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7b15c-129">响应</span><span class="sxs-lookup"><span data-stu-id="7b15c-129">Response</span></span>

<span data-ttu-id="7b15c-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7b15c-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7b15c-132">示例</span><span class="sxs-lookup"><span data-stu-id="7b15c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7b15c-133">请求</span><span class="sxs-lookup"><span data-stu-id="7b15c-133">Request</span></span>

<span data-ttu-id="7b15c-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7b15c-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7b15c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b15c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_incompatibleaccesspackage_to_accesspackage"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/$ref
Content-type: application/json

{
    "@odata.id": "https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2"
}
```
# <a name="c"></a>[<span data-ttu-id="7b15c-136">C#</span><span class="sxs-lookup"><span data-stu-id="7b15c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-incompatibleaccesspackage-to-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b15c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b15c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-incompatibleaccesspackage-to-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b15c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b15c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-incompatibleaccesspackage-to-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b15c-139">Java</span><span class="sxs-lookup"><span data-stu-id="7b15c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-incompatibleaccesspackage-to-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7b15c-140">响应</span><span class="sxs-lookup"><span data-stu-id="7b15c-140">Response</span></span>

<span data-ttu-id="7b15c-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7b15c-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 Created
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Add incompatibleAccessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

