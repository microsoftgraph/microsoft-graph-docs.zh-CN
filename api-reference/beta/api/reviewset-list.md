---
title: 列出 reviewSets
description: 检索 ediscoveryCase 对象中的 reviewSet 对象的列表。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 6fb2c5c1874e9c4fdd6dc59bf4b52783b6e1f88b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085421"
---
# <a name="list-reviewsets"></a><span data-ttu-id="ac0ff-103">列出 reviewSets</span><span class="sxs-lookup"><span data-stu-id="ac0ff-103">List reviewSets</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac0ff-104">检索[ediscoveryCase](../resources/ediscoverycase.md)对象中的[reviewSet](../resources/reviewset.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ac0ff-104">Retrieve the list of [reviewSet](../resources/reviewset.md) objects in an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac0ff-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="ac0ff-105">Permissions</span></span>

<span data-ttu-id="ac0ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac0ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ac0ff-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac0ff-108">Permission type</span></span>                        | <span data-ttu-id="ac0ff-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac0ff-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ac0ff-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac0ff-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac0ff-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="ac0ff-111">User.Read</span></span> |
| <span data-ttu-id="ac0ff-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac0ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac0ff-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac0ff-113">Not supported.</span></span> |
| <span data-ttu-id="ac0ff-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac0ff-114">Application</span></span>                            | <span data-ttu-id="ac0ff-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac0ff-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac0ff-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac0ff-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets
```

## <a name="request-headers"></a><span data-ttu-id="ac0ff-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac0ff-117">Request headers</span></span>

| <span data-ttu-id="ac0ff-118">名称</span><span class="sxs-lookup"><span data-stu-id="ac0ff-118">Name</span></span>          | <span data-ttu-id="ac0ff-119">说明</span><span class="sxs-lookup"><span data-stu-id="ac0ff-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ac0ff-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac0ff-120">Authorization</span></span> | <span data-ttu-id="ac0ff-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ac0ff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac0ff-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac0ff-123">Request body</span></span>

<span data-ttu-id="ac0ff-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ac0ff-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac0ff-125">响应</span><span class="sxs-lookup"><span data-stu-id="ac0ff-125">Response</span></span>

<span data-ttu-id="ac0ff-126">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [reviewSet](../resources/reviewset.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="ac0ff-126">If successful, this method returns a `200 OK` response code and the requested [reviewSet](../resources/reviewset.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ac0ff-127">示例</span><span class="sxs-lookup"><span data-stu-id="ac0ff-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ac0ff-128">请求</span><span class="sxs-lookup"><span data-stu-id="ac0ff-128">Request</span></span>

<span data-ttu-id="ac0ff-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ac0ff-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac0ff-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac0ff-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_reviewset",
  "@odata.type": "microsoft.graph.reviewSet"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets
```
# <a name="c"></a>[<span data-ttu-id="ac0ff-131">C#</span><span class="sxs-lookup"><span data-stu-id="ac0ff-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-reviewset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac0ff-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac0ff-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-reviewset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac0ff-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac0ff-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-reviewset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ac0ff-134">响应</span><span class="sxs-lookup"><span data-stu-id="ac0ff-134">Response</span></span>

<span data-ttu-id="ac0ff-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ac0ff-135">The following is an example of the response.</span></span>

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


