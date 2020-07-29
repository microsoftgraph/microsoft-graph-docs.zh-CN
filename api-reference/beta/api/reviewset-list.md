---
title: 列出 reviewSets
description: 检索 ediscoveryCase 对象中的 reviewSet 对象的列表。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 0543a29273973e1b63735558d27998b68b1bcd25
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509985"
---
# <a name="list-reviewsets"></a><span data-ttu-id="81768-103">列出 reviewSets</span><span class="sxs-lookup"><span data-stu-id="81768-103">List reviewSets</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81768-104">检索[ediscoveryCase](../resources/ediscoverycase.md)对象中的[reviewSet](../resources/reviewset.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="81768-104">Retrieve the list of [reviewSet](../resources/reviewset.md) objects in an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="81768-105">权限</span><span class="sxs-lookup"><span data-stu-id="81768-105">Permissions</span></span>

<span data-ttu-id="81768-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="81768-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="81768-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="81768-108">Permission type</span></span>                        | <span data-ttu-id="81768-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="81768-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="81768-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81768-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="81768-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="81768-111">User.Read</span></span> |
| <span data-ttu-id="81768-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81768-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81768-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="81768-113">Not supported.</span></span> |
| <span data-ttu-id="81768-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="81768-114">Application</span></span>                            | <span data-ttu-id="81768-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="81768-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81768-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81768-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets
```

## <a name="request-headers"></a><span data-ttu-id="81768-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="81768-117">Request headers</span></span>

| <span data-ttu-id="81768-118">名称</span><span class="sxs-lookup"><span data-stu-id="81768-118">Name</span></span>          | <span data-ttu-id="81768-119">说明</span><span class="sxs-lookup"><span data-stu-id="81768-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="81768-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="81768-120">Authorization</span></span> | <span data-ttu-id="81768-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="81768-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81768-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="81768-123">Request body</span></span>

<span data-ttu-id="81768-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="81768-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81768-125">响应</span><span class="sxs-lookup"><span data-stu-id="81768-125">Response</span></span>

<span data-ttu-id="81768-126">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[reviewSet](../resources/reviewset.md)集合。</span><span class="sxs-lookup"><span data-stu-id="81768-126">If successful, this method returns a `200 OK` response code and the requested [reviewSet](../resources/reviewset.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81768-127">示例</span><span class="sxs-lookup"><span data-stu-id="81768-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="81768-128">请求</span><span class="sxs-lookup"><span data-stu-id="81768-128">Request</span></span>

<span data-ttu-id="81768-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="81768-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_reviewset",
  "@odata.type": "microsoft.graph.reviewSet"
}-->

```http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets
```

### <a name="response"></a><span data-ttu-id="81768-130">响应</span><span class="sxs-lookup"><span data-stu-id="81768-130">Response</span></span>

<span data-ttu-id="81768-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="81768-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSet"
} -->

```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#cases",
    "@odata.nextLink": "https://graph.microsoft.com/beta/compliance/ediscovery/cases?$skiptoken=<encodedPageToken>",
    "value": [
        {
            "id": "f6a91542-4ce7-4712-b275-c29545dd8507",
            "displayName": "My Reviewset 1",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-01-16T11:58:27.1408174Z"
        },
        {
            "id": "0d78ec4a-aa91-41ea-8da8-d68b030c168f",
            "displayName": "My Reviewset 2",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-01-16T12:03:32.2038960Z"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete reviewSet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
