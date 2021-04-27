---
title: 创建 reviewSetQuery
description: 使用此 API 创建新的 reviewSetQuery。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: b42cfb7c45b1cd4dcc0a3d2c66f3e0ae94415dd1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044576"
---
# <a name="create-reviewsetquery"></a><span data-ttu-id="b5cef-103">创建 reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="b5cef-103">Create reviewSetQuery</span></span>

<span data-ttu-id="b5cef-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="b5cef-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5cef-105">创建新的 [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b5cef-105">Create a new [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5cef-106">权限</span><span class="sxs-lookup"><span data-stu-id="b5cef-106">Permissions</span></span>

<span data-ttu-id="b5cef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5cef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5cef-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5cef-109">Permission type</span></span>|<span data-ttu-id="b5cef-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5cef-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5cef-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5cef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b5cef-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5cef-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="b5cef-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5cef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5cef-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5cef-114">Not supported.</span></span>|
|<span data-ttu-id="b5cef-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5cef-115">Application</span></span>|<span data-ttu-id="b5cef-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5cef-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5cef-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5cef-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries
```

## <a name="request-headers"></a><span data-ttu-id="b5cef-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5cef-118">Request headers</span></span>

| <span data-ttu-id="b5cef-119">名称</span><span class="sxs-lookup"><span data-stu-id="b5cef-119">Name</span></span>          | <span data-ttu-id="b5cef-120">说明</span><span class="sxs-lookup"><span data-stu-id="b5cef-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b5cef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5cef-121">Authorization</span></span> | <span data-ttu-id="b5cef-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b5cef-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5cef-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5cef-124">Request body</span></span>

<span data-ttu-id="b5cef-125">在请求正文中，提供 [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5cef-125">In the request body, supply a JSON representation of [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object.</span></span> <span data-ttu-id="b5cef-126">下表列出了所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b5cef-126">The following table lists the required properties.</span></span>

| <span data-ttu-id="b5cef-127">属性</span><span class="sxs-lookup"><span data-stu-id="b5cef-127">Property</span></span>     | <span data-ttu-id="b5cef-128">类型</span><span class="sxs-lookup"><span data-stu-id="b5cef-128">Type</span></span>        | <span data-ttu-id="b5cef-129">说明</span><span class="sxs-lookup"><span data-stu-id="b5cef-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b5cef-130">displayName</span><span class="sxs-lookup"><span data-stu-id="b5cef-130">displayName</span></span>  | <span data-ttu-id="b5cef-131">string</span><span class="sxs-lookup"><span data-stu-id="b5cef-131">string</span></span>      | <span data-ttu-id="b5cef-132">审阅集查询的名称</span><span class="sxs-lookup"><span data-stu-id="b5cef-132">The name of the review set query</span></span> |

## <a name="response"></a><span data-ttu-id="b5cef-133">响应</span><span class="sxs-lookup"><span data-stu-id="b5cef-133">Response</span></span>

<span data-ttu-id="b5cef-134">如果成功，此方法在响应正文中返回 响应代码和新的 `201 Created` [microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b5cef-134">If successful, this method returns a `201 Created` response code and a new [microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b5cef-135">示例</span><span class="sxs-lookup"><span data-stu-id="b5cef-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b5cef-136">请求</span><span class="sxs-lookup"><span data-stu-id="b5cef-136">Request</span></span>

<span data-ttu-id="b5cef-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b5cef-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5cef-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5cef-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reviewsetquery"
}-->

```http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries
Content-type: application/json

{
   "displayName":"My Query 1",
   "query":"(subject:\"Quarterly Financials\")"
}
```
# <a name="c"></a>[<span data-ttu-id="b5cef-139">C#</span><span class="sxs-lookup"><span data-stu-id="b5cef-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5cef-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5cef-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5cef-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5cef-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5cef-142">Java</span><span class="sxs-lookup"><span data-stu-id="b5cef-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reviewsetquery-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b5cef-143">响应</span><span class="sxs-lookup"><span data-stu-id="b5cef-143">Response</span></span>

<span data-ttu-id="b5cef-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b5cef-144">The following is an example of the response.</span></span>

> <span data-ttu-id="b5cef-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b5cef-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('2eef613a-ca2d-42f4-89fe-84d5198ddedf')/reviewSets('b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8')/queries/$entity",
    "id": "6b5358b0-2ce2-4369-b9cf-65392fe56807",
    "displayName": "My Query 1",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-03-09T09:05:12.3756813Z",
    "lastModifiedBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "lastModifiedDateTime": "2020-03-09T09:05:12.3756813Z",
    "query": "(subject:\"Quarterly Financials\")"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create reviewSetQuery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


