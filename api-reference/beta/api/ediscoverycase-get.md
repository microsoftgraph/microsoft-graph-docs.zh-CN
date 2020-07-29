---
title: 获取 ediscoveryCase
description: 检索 ediscoverycase 对象的属性和关系。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 258019d4c675b39f4450e05e5846f4f5414c10d5
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509989"
---
# <a name="get-ediscoverycase"></a><span data-ttu-id="5c1a9-103">获取 ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="5c1a9-103">Get ediscoveryCase</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c1a9-104">检索[ediscoveryCase](../resources/ediscoverycase.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5c1a9-104">Retrieve the properties and relationships of an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c1a9-105">权限</span><span class="sxs-lookup"><span data-stu-id="5c1a9-105">Permissions</span></span>

<span data-ttu-id="5c1a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c1a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5c1a9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c1a9-108">Permission type</span></span>                        | <span data-ttu-id="5c1a9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5c1a9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5c1a9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c1a9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c1a9-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="5c1a9-111">User.Read</span></span>      |
| <span data-ttu-id="5c1a9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c1a9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c1a9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c1a9-113">Not supported.</span></span> |
| <span data-ttu-id="5c1a9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c1a9-114">Application</span></span>                            | <span data-ttu-id="5c1a9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c1a9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c1a9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c1a9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c1a9-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5c1a9-117">Optional query parameters</span></span>

<span data-ttu-id="5c1a9-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5c1a9-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5c1a9-119">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5c1a9-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c1a9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c1a9-120">Request headers</span></span>

| <span data-ttu-id="5c1a9-121">名称</span><span class="sxs-lookup"><span data-stu-id="5c1a9-121">Name</span></span>      |<span data-ttu-id="5c1a9-122">说明</span><span class="sxs-lookup"><span data-stu-id="5c1a9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5c1a9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c1a9-123">Authorization</span></span> | <span data-ttu-id="5c1a9-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="5c1a9-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c1a9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c1a9-125">Request body</span></span>

<span data-ttu-id="5c1a9-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5c1a9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c1a9-127">响应</span><span class="sxs-lookup"><span data-stu-id="5c1a9-127">Response</span></span>

<span data-ttu-id="5c1a9-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[ediscoveryCase](../resources/ediscoverycase.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5c1a9-128">If successful, this method returns a `200 OK` response code and the requested [ediscoveryCase](../resources/ediscoverycase.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c1a9-129">示例</span><span class="sxs-lookup"><span data-stu-id="5c1a9-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c1a9-130">请求</span><span class="sxs-lookup"><span data-stu-id="5c1a9-130">Request</span></span>

<span data-ttu-id="5c1a9-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5c1a9-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_ediscoverycase"
}-->

```http
GET https://graph.microsoft.com/beta/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
```

### <a name="response"></a><span data-ttu-id="5c1a9-132">响应</span><span class="sxs-lookup"><span data-stu-id="5c1a9-132">Response</span></span>

<span data-ttu-id="5c1a9-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5c1a9-133">The following is an example of the response.</span></span>

> <span data-ttu-id="5c1a9-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5c1a9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscoveryCase"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "061b9a92-8926-4bd9-b41d-abf35edc7583",
    "displayName": "My Case 1",
    "description": "",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-02-20T22:42:28.5505500Z",
    "lastModifiedBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "lastModifiedDateTime": "2020-02-20T22:42:28.5505500Z",
    "status": "active",
    "closedBy": null,
    "closedDateTime": null,
    "externalId": ""
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ediscoveryCase",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->