---
title: 创建 accessPackageCatalog
description: 创建新的 accessPackageCatalog。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 38f0683a1160b9deaf30b4ebc782b405417ef4db
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935276"
---
# <a name="create-accesspackagecatalog"></a><span data-ttu-id="a0dad-103">创建 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="a0dad-103">Create accessPackageCatalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0dad-104">创建新的[accessPackageCatalog](../resources/accesspackagecatalog.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a0dad-104">Create a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0dad-105">权限</span><span class="sxs-lookup"><span data-stu-id="a0dad-105">Permissions</span></span>

<span data-ttu-id="a0dad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0dad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a0dad-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0dad-108">Permission type</span></span>                        | <span data-ttu-id="a0dad-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0dad-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a0dad-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0dad-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a0dad-111">EntitlementManagement</span><span class="sxs-lookup"><span data-stu-id="a0dad-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="a0dad-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0dad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0dad-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0dad-113">Not supported.</span></span> |
| <span data-ttu-id="a0dad-114">Application</span><span class="sxs-lookup"><span data-stu-id="a0dad-114">Application</span></span>                            | <span data-ttu-id="a0dad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0dad-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0dad-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0dad-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="request-headers"></a><span data-ttu-id="a0dad-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0dad-117">Request headers</span></span>

| <span data-ttu-id="a0dad-118">名称</span><span class="sxs-lookup"><span data-stu-id="a0dad-118">Name</span></span>          | <span data-ttu-id="a0dad-119">说明</span><span class="sxs-lookup"><span data-stu-id="a0dad-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a0dad-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0dad-120">Authorization</span></span> | <span data-ttu-id="a0dad-121">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="a0dad-121">Bearer \{token\}.</span></span> <span data-ttu-id="a0dad-122">必填。</span><span class="sxs-lookup"><span data-stu-id="a0dad-122">Required.</span></span> |
| <span data-ttu-id="a0dad-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0dad-123">Content-Type</span></span>  | <span data-ttu-id="a0dad-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a0dad-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0dad-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0dad-125">Request body</span></span>

<span data-ttu-id="a0dad-126">在请求正文中，提供[accessPackageCatalog](../resources/accesspackagecatalog.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0dad-126">In the request body, supply a JSON representation of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>  <span data-ttu-id="a0dad-127">包括**displayname**、 **description**和**isExternallyVisible**属性。</span><span class="sxs-lookup"><span data-stu-id="a0dad-127">Include the **displayname**, **description**, and **isExternallyVisible** properties.</span></span>

## <a name="response"></a><span data-ttu-id="a0dad-128">响应</span><span class="sxs-lookup"><span data-stu-id="a0dad-128">Response</span></span>

<span data-ttu-id="a0dad-129">如果成功，此方法在响应正文中返回一个200系列响应代码和一个新的[accessPackageCatalog](../resources/accesspackagecatalog.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a0dad-129">If successful, this method returns a 200-series response code and a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0dad-130">示例</span><span class="sxs-lookup"><span data-stu-id="a0dad-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a0dad-131">请求</span><span class="sxs-lookup"><span data-stu-id="a0dad-131">Request</span></span>

<span data-ttu-id="a0dad-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a0dad-132">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a0dad-133">响应</span><span class="sxs-lookup"><span data-stu-id="a0dad-133">Response</span></span>

<span data-ttu-id="a0dad-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a0dad-134">The following is an example of the response.</span></span>

> <span data-ttu-id="a0dad-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a0dad-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
