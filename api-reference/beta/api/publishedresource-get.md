---
title: 获取 publishedResource
description: 检索 [publishedResource 对象的属性和](../resources/publishedresource.md) 关系。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 6b0f84de5dfdcde391094e71dbcde451dc4fe3b0
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135532"
---
# <a name="get-publishedresource"></a><span data-ttu-id="9bf16-103">获取 publishedResource</span><span class="sxs-lookup"><span data-stu-id="9bf16-103">Get publishedResource</span></span>

<span data-ttu-id="9bf16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bf16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bf16-105">检索 [publishedResource 对象的属性和](../resources/publishedresource.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="9bf16-105">Retrieve the properties and relationships of [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9bf16-106">权限</span><span class="sxs-lookup"><span data-stu-id="9bf16-106">Permissions</span></span>

<span data-ttu-id="9bf16-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9bf16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9bf16-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9bf16-109">Permission type</span></span>                        | <span data-ttu-id="9bf16-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9bf16-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="9bf16-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9bf16-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9bf16-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bf16-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="9bf16-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9bf16-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bf16-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bf16-114">Not supported.</span></span> |
| <span data-ttu-id="9bf16-115">Application</span><span class="sxs-lookup"><span data-stu-id="9bf16-115">Application</span></span>                            | <span data-ttu-id="9bf16-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bf16-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9bf16-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9bf16-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9bf16-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9bf16-118">Optional query parameters</span></span>

<span data-ttu-id="9bf16-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9bf16-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9bf16-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9bf16-120">Request headers</span></span>

| <span data-ttu-id="9bf16-121">名称</span><span class="sxs-lookup"><span data-stu-id="9bf16-121">Name</span></span>      |<span data-ttu-id="9bf16-122">说明</span><span class="sxs-lookup"><span data-stu-id="9bf16-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9bf16-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bf16-123">Authorization</span></span> | <span data-ttu-id="9bf16-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="9bf16-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9bf16-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9bf16-125">Request body</span></span>

<span data-ttu-id="9bf16-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9bf16-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bf16-127">响应</span><span class="sxs-lookup"><span data-stu-id="9bf16-127">Response</span></span>

<span data-ttu-id="9bf16-128">如果成功，此方法在响应正文中返回响应代码和请求的 `200 OK` [publishedResource](../resources/publishedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9bf16-128">If successful, this method returns a `200 OK` response code and the requested [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9bf16-129">示例</span><span class="sxs-lookup"><span data-stu-id="9bf16-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9bf16-130">请求</span><span class="sxs-lookup"><span data-stu-id="9bf16-130">Request</span></span>

<span data-ttu-id="9bf16-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9bf16-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9bf16-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bf16-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_publishedresource"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/aed0b780-965f-4149-85c5-a8c73e58b67d/?$expand=agentGroups
```
# <a name="c"></a>[<span data-ttu-id="9bf16-133">C#</span><span class="sxs-lookup"><span data-stu-id="9bf16-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9bf16-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bf16-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9bf16-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9bf16-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9bf16-136">Java</span><span class="sxs-lookup"><span data-stu-id="9bf16-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-publishedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9bf16-137">响应</span><span class="sxs-lookup"><span data-stu-id="9bf16-137">Response</span></span>

<span data-ttu-id="9bf16-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9bf16-138">The following is an example of the response.</span></span>

> <span data-ttu-id="9bf16-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9bf16-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "publishingType": "provisioning",
    "displayName": "Demo provisioning",
    "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
    "resourceName": "domain1.contoso.com",
    "agentGroups": [
        {
            "id": "2d55ed41-1619-4848-92bb-0576d3038682",
            "displayName": "Group 1"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



