---
title: 列出 publishedResources
description: 检索 publishedResource 对象的列表。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9182d2ed5764d0f35940153c8b240466acffccc2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973382"
---
# <a name="list-publishedresources"></a><span data-ttu-id="86772-103">列出 publishedResources</span><span class="sxs-lookup"><span data-stu-id="86772-103">List publishedResources</span></span>

<span data-ttu-id="86772-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86772-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86772-105">检索 [publishedResource](../resources/publishedresource.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="86772-105">Retrieve a list of [publishedResource](../resources/publishedresource.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="86772-106">权限</span><span class="sxs-lookup"><span data-stu-id="86772-106">Permissions</span></span>

<span data-ttu-id="86772-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86772-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86772-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="86772-109">Permission type</span></span>                        | <span data-ttu-id="86772-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86772-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="86772-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86772-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="86772-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86772-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="86772-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86772-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86772-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="86772-114">Not supported.</span></span> |
| <span data-ttu-id="86772-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="86772-115">Application</span></span>                            | <span data-ttu-id="86772-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="86772-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86772-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86772-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="86772-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="86772-118">Optional query parameters</span></span>

<span data-ttu-id="86772-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="86772-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86772-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="86772-120">Request headers</span></span>

| <span data-ttu-id="86772-121">名称</span><span class="sxs-lookup"><span data-stu-id="86772-121">Name</span></span>      |<span data-ttu-id="86772-122">说明</span><span class="sxs-lookup"><span data-stu-id="86772-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="86772-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86772-123">Authorization</span></span> | <span data-ttu-id="86772-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="86772-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="86772-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="86772-125">Request body</span></span>

<span data-ttu-id="86772-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="86772-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86772-127">响应</span><span class="sxs-lookup"><span data-stu-id="86772-127">Response</span></span>

<span data-ttu-id="86772-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [publishedResource](../resources/publishedresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="86772-128">If successful, this method returns a `200 OK` response code and a collection of [publishedResource](../resources/publishedresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="86772-129">示例</span><span class="sxs-lookup"><span data-stu-id="86772-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86772-130">请求</span><span class="sxs-lookup"><span data-stu-id="86772-130">Request</span></span>

<span data-ttu-id="86772-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="86772-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="86772-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="86772-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_publishedresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/{publishingType}/publishedResources?$expand=agentGroups
```
# <a name="c"></a>[<span data-ttu-id="86772-133">C#</span><span class="sxs-lookup"><span data-stu-id="86772-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-publishedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86772-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86772-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-publishedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86772-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86772-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-publishedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86772-136">Java</span><span class="sxs-lookup"><span data-stu-id="86772-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-publishedresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="86772-137">响应</span><span class="sxs-lookup"><span data-stu-id="86772-137">Response</span></span>

<span data-ttu-id="86772-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="86772-138">The following is an example of the response.</span></span>

> <span data-ttu-id="86772-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="86772-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List publishedResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


