---
title: 列出 accessPackageResources
description: 检索 accesspackageresource 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4f1fc80de9a879de24d70265cd336c8613ee41a0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951925"
---
# <a name="list-accesspackageresources"></a><span data-ttu-id="7629e-103">列出 accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="7629e-103">List accessPackageResources</span></span>

<span data-ttu-id="7629e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7629e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7629e-105">检索[accessPackageCatalog](../resources/accesspackagecatalog.md)中的[accessPackageResource](../resources/accesspackageresource.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="7629e-105">Retrieve a list of [accessPackageResource](../resources/accesspackageresource.md) objects in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7629e-106">权限</span><span class="sxs-lookup"><span data-stu-id="7629e-106">Permissions</span></span>

<span data-ttu-id="7629e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7629e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7629e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7629e-109">Permission type</span></span>                        | <span data-ttu-id="7629e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7629e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7629e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7629e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7629e-112">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="7629e-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="7629e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7629e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7629e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7629e-114">Not supported.</span></span> |
| <span data-ttu-id="7629e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7629e-115">Application</span></span>                            | <span data-ttu-id="7629e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7629e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7629e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7629e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7629e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7629e-118">Optional query parameters</span></span>

<span data-ttu-id="7629e-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7629e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7629e-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="7629e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7629e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7629e-121">Request headers</span></span>

| <span data-ttu-id="7629e-122">名称</span><span class="sxs-lookup"><span data-stu-id="7629e-122">Name</span></span>      |<span data-ttu-id="7629e-123">说明</span><span class="sxs-lookup"><span data-stu-id="7629e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7629e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7629e-124">Authorization</span></span> | <span data-ttu-id="7629e-125">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="7629e-125">Bearer \{token\}.</span></span> <span data-ttu-id="7629e-126">必填。</span><span class="sxs-lookup"><span data-stu-id="7629e-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7629e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7629e-127">Request body</span></span>

<span data-ttu-id="7629e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7629e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7629e-129">响应</span><span class="sxs-lookup"><span data-stu-id="7629e-129">Response</span></span>

<span data-ttu-id="7629e-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [accessPackageResource](../resources/accesspackageresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7629e-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResource](../resources/accesspackageresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7629e-131">示例</span><span class="sxs-lookup"><span data-stu-id="7629e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7629e-132">请求</span><span class="sxs-lookup"><span data-stu-id="7629e-132">Request</span></span>

<span data-ttu-id="7629e-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7629e-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7629e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7629e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```
# <a name="c"></a>[<span data-ttu-id="7629e-135">C#</span><span class="sxs-lookup"><span data-stu-id="7629e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7629e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7629e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7629e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7629e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7629e-138">Java</span><span class="sxs-lookup"><span data-stu-id="7629e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7629e-139">响应</span><span class="sxs-lookup"><span data-stu-id="7629e-139">Response</span></span>

<span data-ttu-id="7629e-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7629e-140">The following is an example of the response.</span></span>

> <span data-ttu-id="7629e-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7629e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "400279ff-8e85-4dcf-b1d6-d3a6be372951",
      "displayName": "Faculty cafeteria ordering",
      "description": "Example application",
      "url": "https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/",
      "resourceType": "Application",
      "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


