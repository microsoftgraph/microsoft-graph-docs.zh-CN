---
title: 创建 reviewSetQuery
description: 使用此 API 创建新的 reviewSetQuery。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 86f84a37965ddbcc6d0577024b8e1e747d5615b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085326"
---
# <a name="create-reviewsetquery"></a><span data-ttu-id="1592f-103">创建 reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="1592f-103">Create reviewSetQuery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1592f-104">创建新的 [reviewSetQuery](../resources/reviewsetquery.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1592f-104">Create a new [reviewSetQuery](../resources/reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1592f-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="1592f-105">Permissions</span></span>

<span data-ttu-id="1592f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1592f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1592f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1592f-108">Permission type</span></span>                        | <span data-ttu-id="1592f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1592f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1592f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1592f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1592f-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="1592f-111">User.Read</span></span> |
| <span data-ttu-id="1592f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1592f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1592f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1592f-113">Not supported.</span></span> |
| <span data-ttu-id="1592f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1592f-114">Application</span></span>                            | <span data-ttu-id="1592f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1592f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1592f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1592f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries
```

## <a name="request-headers"></a><span data-ttu-id="1592f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1592f-117">Request headers</span></span>

| <span data-ttu-id="1592f-118">名称</span><span class="sxs-lookup"><span data-stu-id="1592f-118">Name</span></span>          | <span data-ttu-id="1592f-119">说明</span><span class="sxs-lookup"><span data-stu-id="1592f-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1592f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1592f-120">Authorization</span></span> | <span data-ttu-id="1592f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1592f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1592f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1592f-123">Request body</span></span>

<span data-ttu-id="1592f-124">在请求正文中，提供 [reviewSetQuery](../resources/reviewsetquery.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1592f-124">In the request body, supply a JSON representation of [reviewSetQuery](../resources/reviewsetquery.md) object.</span></span> <span data-ttu-id="1592f-125">下表列出了必需的属性。</span><span class="sxs-lookup"><span data-stu-id="1592f-125">The following table lists the required properties.</span></span>

| <span data-ttu-id="1592f-126">属性</span><span class="sxs-lookup"><span data-stu-id="1592f-126">Property</span></span>     | <span data-ttu-id="1592f-127">类型</span><span class="sxs-lookup"><span data-stu-id="1592f-127">Type</span></span>        | <span data-ttu-id="1592f-128">说明</span><span class="sxs-lookup"><span data-stu-id="1592f-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1592f-129">displayName</span><span class="sxs-lookup"><span data-stu-id="1592f-129">displayName</span></span>  | <span data-ttu-id="1592f-130">string</span><span class="sxs-lookup"><span data-stu-id="1592f-130">string</span></span>      | <span data-ttu-id="1592f-131">审阅集查询的名称</span><span class="sxs-lookup"><span data-stu-id="1592f-131">The name of the review set query</span></span> |

## <a name="response"></a><span data-ttu-id="1592f-132">响应</span><span class="sxs-lookup"><span data-stu-id="1592f-132">Response</span></span>

<span data-ttu-id="1592f-133">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的 [reviewSetQuery](../resources/reviewsetquery.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1592f-133">If successful, this method returns a `201 Created` response code and a new [reviewSetQuery](../resources/reviewsetquery.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1592f-134">示例</span><span class="sxs-lookup"><span data-stu-id="1592f-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1592f-135">请求</span><span class="sxs-lookup"><span data-stu-id="1592f-135">Request</span></span>

<span data-ttu-id="1592f-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1592f-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1592f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="1592f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reviewsetquery"
}-->

```http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries
Content-type: application/json

{
     "displayName" : "My Query 1",
     "query": "(subject:\"Quarterly Financials\")"
}
```
# <a name="c"></a>[<span data-ttu-id="1592f-138">C#</span><span class="sxs-lookup"><span data-stu-id="1592f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1592f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1592f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1592f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1592f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1592f-141">响应</span><span class="sxs-lookup"><span data-stu-id="1592f-141">Response</span></span>

<span data-ttu-id="1592f-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1592f-142">The following is an example of the response.</span></span>

> <span data-ttu-id="1592f-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1592f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSetQuery"
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


