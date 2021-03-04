---
title: 列出 accessPackageResources
description: 检索 accesspackageresource 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a148144c416d91ed43d1eedcbc800b779dc2800a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439553"
---
# <a name="list-accesspackageresources"></a><span data-ttu-id="f23e1-103">列出 accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="f23e1-103">List accessPackageResources</span></span>

<span data-ttu-id="f23e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f23e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f23e1-105">检索 [accessPackageCatalog](../resources/accesspackageresource.md) 中的 [accessPackageResource 对象列表](../resources/accesspackagecatalog.md)。</span><span class="sxs-lookup"><span data-stu-id="f23e1-105">Retrieve a list of [accessPackageResource](../resources/accesspackageresource.md) objects in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>  <span data-ttu-id="f23e1-106">若要请求添加或删除 [accessPackageResource，](../resources/accesspackageresource.md)请使用创建 [accessPackageResourceRequest](accesspackageresourcerequest-post.md)。</span><span class="sxs-lookup"><span data-stu-id="f23e1-106">To request to add or remove an [accessPackageResource](../resources/accesspackageresource.md), use [create accessPackageResourceRequest](accesspackageresourcerequest-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f23e1-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="f23e1-107">Permissions</span></span>

<span data-ttu-id="f23e1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f23e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f23e1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f23e1-110">Permission type</span></span>                        | <span data-ttu-id="f23e1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f23e1-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f23e1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f23e1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f23e1-113">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f23e1-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="f23e1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f23e1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f23e1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f23e1-115">Not supported.</span></span> |
| <span data-ttu-id="f23e1-116">Application</span><span class="sxs-lookup"><span data-stu-id="f23e1-116">Application</span></span>                            | <span data-ttu-id="f23e1-117">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f23e1-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f23e1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f23e1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f23e1-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f23e1-119">Optional query parameters</span></span>

<span data-ttu-id="f23e1-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f23e1-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f23e1-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f23e1-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f23e1-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f23e1-122">Request headers</span></span>

| <span data-ttu-id="f23e1-123">名称</span><span class="sxs-lookup"><span data-stu-id="f23e1-123">Name</span></span>      |<span data-ttu-id="f23e1-124">说明</span><span class="sxs-lookup"><span data-stu-id="f23e1-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f23e1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f23e1-125">Authorization</span></span> | <span data-ttu-id="f23e1-126">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="f23e1-126">Bearer \{token\}.</span></span> <span data-ttu-id="f23e1-127">必需。</span><span class="sxs-lookup"><span data-stu-id="f23e1-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f23e1-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f23e1-128">Request body</span></span>

<span data-ttu-id="f23e1-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f23e1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f23e1-130">响应</span><span class="sxs-lookup"><span data-stu-id="f23e1-130">Response</span></span>

<span data-ttu-id="f23e1-131">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [accessPackageResource](../resources/accesspackageresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f23e1-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResource](../resources/accesspackageresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f23e1-132">示例</span><span class="sxs-lookup"><span data-stu-id="f23e1-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f23e1-133">请求</span><span class="sxs-lookup"><span data-stu-id="f23e1-133">Request</span></span>

<span data-ttu-id="f23e1-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f23e1-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f23e1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f23e1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```
# <a name="c"></a>[<span data-ttu-id="f23e1-136">C#</span><span class="sxs-lookup"><span data-stu-id="f23e1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f23e1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f23e1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f23e1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f23e1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f23e1-139">Java</span><span class="sxs-lookup"><span data-stu-id="f23e1-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f23e1-140">响应</span><span class="sxs-lookup"><span data-stu-id="f23e1-140">Response</span></span>

<span data-ttu-id="f23e1-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f23e1-141">The following is an example of the response.</span></span>

> <span data-ttu-id="f23e1-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f23e1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


