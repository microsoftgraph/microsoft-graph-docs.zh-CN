---
title: 获取 reviewSetQuery
description: 检索电子数据展示 reviewsetquery 对象的属性和关系。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 8add5af1daa40d1bce177cb22b3c44242ea0a0c4
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510013"
---
# <a name="get-reviewsetquery"></a><span data-ttu-id="6ffc0-103">获取 reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="6ffc0-103">Get reviewSetQuery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ffc0-104">检索电子数据展示[reviewSetQuery](../resources/reviewsetquery.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6ffc0-104">Retrieve the properties and relationships of an eDiscovery [reviewSetQuery](../resources/reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ffc0-105">权限</span><span class="sxs-lookup"><span data-stu-id="6ffc0-105">Permissions</span></span>

<span data-ttu-id="6ffc0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ffc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6ffc0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ffc0-108">Permission type</span></span>                        | <span data-ttu-id="6ffc0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ffc0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6ffc0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ffc0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6ffc0-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="6ffc0-111">User.Read</span></span> |
| <span data-ttu-id="6ffc0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ffc0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ffc0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ffc0-113">Not supported.</span></span> |
| <span data-ttu-id="6ffc0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ffc0-114">Application</span></span>                            | <span data-ttu-id="6ffc0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ffc0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ffc0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ffc0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6ffc0-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6ffc0-117">Optional query parameters</span></span>

<span data-ttu-id="6ffc0-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6ffc0-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6ffc0-119">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6ffc0-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ffc0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ffc0-120">Request headers</span></span>

| <span data-ttu-id="6ffc0-121">名称</span><span class="sxs-lookup"><span data-stu-id="6ffc0-121">Name</span></span>      |<span data-ttu-id="6ffc0-122">说明</span><span class="sxs-lookup"><span data-stu-id="6ffc0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6ffc0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ffc0-123">Authorization</span></span> | <span data-ttu-id="6ffc0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ffc0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ffc0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ffc0-126">Request body</span></span>

<span data-ttu-id="6ffc0-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6ffc0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ffc0-128">响应</span><span class="sxs-lookup"><span data-stu-id="6ffc0-128">Response</span></span>

<span data-ttu-id="6ffc0-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[reviewSetQuery](../resources/reviewsetquery.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6ffc0-129">If successful, this method returns a `200 OK` response code and the requested [reviewSetQuery](../resources/reviewsetquery.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6ffc0-130">示例</span><span class="sxs-lookup"><span data-stu-id="6ffc0-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6ffc0-131">请求</span><span class="sxs-lookup"><span data-stu-id="6ffc0-131">Request</span></span>

<span data-ttu-id="6ffc0-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6ffc0-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_reviewsetquery"
}-->

```http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
```

### <a name="response"></a><span data-ttu-id="6ffc0-133">响应</span><span class="sxs-lookup"><span data-stu-id="6ffc0-133">Response</span></span>

<span data-ttu-id="6ffc0-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6ffc0-134">The following is an example of the response.</span></span>

> <span data-ttu-id="6ffc0-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6ffc0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSetQuery"
} -->

```http
HTTP/1.1 200 OK
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
    "query": "subject:\"Quarterly Financials\""
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get reviewSetQuery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
