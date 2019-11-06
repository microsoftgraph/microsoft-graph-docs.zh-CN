---
title: 创建 accessPackageCatalog
description: 创建新的 accessPackageCatalog。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9b973310b9cb442f2b95ba4eafd9a2e76ba33fce
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994212"
---
# <a name="create-accesspackagecatalog"></a><span data-ttu-id="3e83e-103">创建 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="3e83e-103">Create accessPackageCatalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e83e-104">创建新的[accessPackageCatalog](../resources/accesspackagecatalog.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3e83e-104">Create a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e83e-105">权限</span><span class="sxs-lookup"><span data-stu-id="3e83e-105">Permissions</span></span>

<span data-ttu-id="3e83e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e83e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e83e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e83e-108">Permission type</span></span>                        | <span data-ttu-id="3e83e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e83e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3e83e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e83e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e83e-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e83e-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="3e83e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e83e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e83e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e83e-113">Not supported.</span></span> |
| <span data-ttu-id="3e83e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e83e-114">Application</span></span>                            | <span data-ttu-id="3e83e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e83e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e83e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e83e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="request-headers"></a><span data-ttu-id="3e83e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e83e-117">Request headers</span></span>

| <span data-ttu-id="3e83e-118">名称</span><span class="sxs-lookup"><span data-stu-id="3e83e-118">Name</span></span>          | <span data-ttu-id="3e83e-119">说明</span><span class="sxs-lookup"><span data-stu-id="3e83e-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3e83e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e83e-120">Authorization</span></span> | <span data-ttu-id="3e83e-121">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="3e83e-121">Bearer \{token\}.</span></span> <span data-ttu-id="3e83e-122">必填。</span><span class="sxs-lookup"><span data-stu-id="3e83e-122">Required.</span></span> |
| <span data-ttu-id="3e83e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3e83e-123">Content-Type</span></span>  | <span data-ttu-id="3e83e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3e83e-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3e83e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e83e-125">Request body</span></span>

<span data-ttu-id="3e83e-126">在请求正文中，提供[accessPackageCatalog](../resources/accesspackagecatalog.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e83e-126">In the request body, supply a JSON representation of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>  <span data-ttu-id="3e83e-127">包括**displayname**、 **description**和**isExternallyVisible**属性。</span><span class="sxs-lookup"><span data-stu-id="3e83e-127">Include the **displayname**, **description**, and **isExternallyVisible** properties.</span></span>

## <a name="response"></a><span data-ttu-id="3e83e-128">响应</span><span class="sxs-lookup"><span data-stu-id="3e83e-128">Response</span></span>

<span data-ttu-id="3e83e-129">如果成功，此方法在响应正文中返回一个200系列响应代码和一个新的[accessPackageCatalog](../resources/accesspackagecatalog.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3e83e-129">If successful, this method returns a 200-series response code and a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3e83e-130">示例</span><span class="sxs-lookup"><span data-stu-id="3e83e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3e83e-131">请求</span><span class="sxs-lookup"><span data-stu-id="3e83e-131">Request</span></span>

<span data-ttu-id="3e83e-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3e83e-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3e83e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e83e-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3e83e-134">C#</span><span class="sxs-lookup"><span data-stu-id="3e83e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackagecatalog-from-accesspackagecatalogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e83e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e83e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackagecatalog-from-accesspackagecatalogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3e83e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e83e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackagecatalog-from-accesspackagecatalogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3e83e-137">响应</span><span class="sxs-lookup"><span data-stu-id="3e83e-137">Response</span></span>

<span data-ttu-id="3e83e-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3e83e-138">The following is an example of the response.</span></span>

> <span data-ttu-id="3e83e-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3e83e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
