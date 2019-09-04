---
title: 获取 publishedResource
description: 检索[publishedResource](../resources/publishedresource.md)对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 798c01ca6b26dea59b536877a5874f74b4fd5e26
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36725463"
---
# <a name="get-publishedresource"></a><span data-ttu-id="19ae2-103">获取 publishedResource</span><span class="sxs-lookup"><span data-stu-id="19ae2-103">Get publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19ae2-104">检索[publishedResource](../resources/publishedresource.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="19ae2-104">Retrieve the properties and relationships of [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="19ae2-105">权限</span><span class="sxs-lookup"><span data-stu-id="19ae2-105">Permissions</span></span>

<span data-ttu-id="19ae2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19ae2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19ae2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="19ae2-108">Permission type</span></span>                        | <span data-ttu-id="19ae2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19ae2-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="19ae2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19ae2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="19ae2-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="19ae2-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="19ae2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19ae2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19ae2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="19ae2-113">Not supported.</span></span> |
| <span data-ttu-id="19ae2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="19ae2-114">Application</span></span>                            | <span data-ttu-id="19ae2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="19ae2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19ae2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19ae2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19ae2-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="19ae2-117">Optional query parameters</span></span>

<span data-ttu-id="19ae2-118">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="19ae2-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19ae2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="19ae2-119">Request headers</span></span>

| <span data-ttu-id="19ae2-120">名称</span><span class="sxs-lookup"><span data-stu-id="19ae2-120">Name</span></span>      |<span data-ttu-id="19ae2-121">说明</span><span class="sxs-lookup"><span data-stu-id="19ae2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="19ae2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="19ae2-122">Authorization</span></span> | <span data-ttu-id="19ae2-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="19ae2-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="19ae2-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="19ae2-124">Request body</span></span>

<span data-ttu-id="19ae2-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="19ae2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19ae2-126">响应</span><span class="sxs-lookup"><span data-stu-id="19ae2-126">Response</span></span>

<span data-ttu-id="19ae2-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和请求的[publishedResource](../resources/publishedresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="19ae2-127">If successful, this method returns a `200 OK` response code and the requested [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="19ae2-128">示例</span><span class="sxs-lookup"><span data-stu-id="19ae2-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="19ae2-129">请求</span><span class="sxs-lookup"><span data-stu-id="19ae2-129">Request</span></span>

<span data-ttu-id="19ae2-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="19ae2-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="19ae2-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="19ae2-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_publishedresource"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/aed0b780-965f-4149-85c5-a8c73e58b67d/?$expand=agentGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="19ae2-132">C#</span><span class="sxs-lookup"><span data-stu-id="19ae2-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19ae2-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19ae2-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19ae2-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="19ae2-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="19ae2-135">响应</span><span class="sxs-lookup"><span data-stu-id="19ae2-135">Response</span></span>

<span data-ttu-id="19ae2-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="19ae2-136">The following is an example of the response.</span></span>

> <span data-ttu-id="19ae2-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="19ae2-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
