---
title: 创建 accessPackageCatalog
description: 创建新的 accessPackageCatalog。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 783744f3e2cfc59f20e2105468b5f2cdc2d7ee7d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439525"
---
# <a name="create-accesspackagecatalog"></a><span data-ttu-id="9cc86-103">创建 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="9cc86-103">Create accessPackageCatalog</span></span>

<span data-ttu-id="9cc86-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cc86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cc86-105">创建新的 [accessPackageCatalog](../resources/accesspackagecatalog.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9cc86-105">Create a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cc86-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9cc86-106">Permissions</span></span>

<span data-ttu-id="9cc86-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9cc86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9cc86-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cc86-109">Permission type</span></span>                        | <span data-ttu-id="9cc86-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cc86-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9cc86-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cc86-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9cc86-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cc86-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="9cc86-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cc86-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cc86-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cc86-114">Not supported.</span></span> |
| <span data-ttu-id="9cc86-115">Application</span><span class="sxs-lookup"><span data-stu-id="9cc86-115">Application</span></span>                            | <span data-ttu-id="9cc86-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cc86-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cc86-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cc86-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="request-headers"></a><span data-ttu-id="9cc86-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cc86-118">Request headers</span></span>

| <span data-ttu-id="9cc86-119">名称</span><span class="sxs-lookup"><span data-stu-id="9cc86-119">Name</span></span>          | <span data-ttu-id="9cc86-120">说明</span><span class="sxs-lookup"><span data-stu-id="9cc86-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9cc86-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cc86-121">Authorization</span></span> | <span data-ttu-id="9cc86-122">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="9cc86-122">Bearer \{token\}.</span></span> <span data-ttu-id="9cc86-123">必需。</span><span class="sxs-lookup"><span data-stu-id="9cc86-123">Required.</span></span> |
| <span data-ttu-id="9cc86-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9cc86-124">Content-Type</span></span>  | <span data-ttu-id="9cc86-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9cc86-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9cc86-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cc86-126">Request body</span></span>

<span data-ttu-id="9cc86-127">在请求正文中，提供 [accessPackageCatalog](../resources/accesspackagecatalog.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9cc86-127">In the request body, supply a JSON representation of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>  <span data-ttu-id="9cc86-128">包括 **displayname** **、description** 和 **isExternallyVisible** 属性。</span><span class="sxs-lookup"><span data-stu-id="9cc86-128">Include the **displayname**, **description**, and **isExternallyVisible** properties.</span></span>

## <a name="response"></a><span data-ttu-id="9cc86-129">响应</span><span class="sxs-lookup"><span data-stu-id="9cc86-129">Response</span></span>

<span data-ttu-id="9cc86-130">如果成功，此方法在响应正文中返回 200 系列响应代码和新的 [accessPackageCatalog](../resources/accesspackagecatalog.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9cc86-130">If successful, this method returns a 200-series response code and a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9cc86-131">示例</span><span class="sxs-lookup"><span data-stu-id="9cc86-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9cc86-132">请求</span><span class="sxs-lookup"><span data-stu-id="9cc86-132">Request</span></span>

<span data-ttu-id="9cc86-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9cc86-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9cc86-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc86-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackagecatalog_from_accesspackagecatalogs"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs
Content-type: application/json

{
  "displayName": "sales",
  "description": "for employees working with sales and outside sales partners",
  "isExternallyVisible": true
}
```
# <a name="c"></a>[<span data-ttu-id="9cc86-135">C#</span><span class="sxs-lookup"><span data-stu-id="9cc86-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackagecatalog-from-accesspackagecatalogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cc86-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cc86-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackagecatalog-from-accesspackagecatalogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cc86-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cc86-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackagecatalog-from-accesspackagecatalogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9cc86-138">Java</span><span class="sxs-lookup"><span data-stu-id="9cc86-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackagecatalog-from-accesspackagecatalogs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9cc86-139">响应</span><span class="sxs-lookup"><span data-stu-id="9cc86-139">Response</span></span>

<span data-ttu-id="9cc86-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9cc86-140">The following is an example of the response.</span></span>

> <span data-ttu-id="9cc86-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9cc86-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageCatalog"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
  "displayName": "sales",
  "description": "for employees working with sales and outside sales partners",
  "catalogType": "UserManaged",
  "catalogStatus": "Published",
  "isExternallyVisible": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


