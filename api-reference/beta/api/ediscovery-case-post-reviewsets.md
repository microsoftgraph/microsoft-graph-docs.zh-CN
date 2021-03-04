---
title: 创建 reviewSet
description: 创建电子数据展示审阅集。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: b288d6617563ec524c7dc0af65ebffae0fc708de
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446081"
---
# <a name="create-reviewset"></a><span data-ttu-id="016ec-103">创建 reviewSet</span><span class="sxs-lookup"><span data-stu-id="016ec-103">Create reviewSet</span></span>

<span data-ttu-id="016ec-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="016ec-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="016ec-105">创建新的 [reviewSet](../resources/ediscovery-reviewset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="016ec-105">Create a new [reviewSet](../resources/ediscovery-reviewset.md) object.</span></span> <span data-ttu-id="016ec-106">请求正文包含显示名称审阅集，这是唯一可写属性。</span><span class="sxs-lookup"><span data-stu-id="016ec-106">The request body contains the display name of the review set, which is the only writable property.</span></span>

## <a name="permissions"></a><span data-ttu-id="016ec-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="016ec-107">Permissions</span></span>

<span data-ttu-id="016ec-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="016ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="016ec-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="016ec-110">Permission type</span></span>|<span data-ttu-id="016ec-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="016ec-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="016ec-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="016ec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="016ec-113">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="016ec-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="016ec-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="016ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="016ec-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="016ec-115">Not supported.</span></span>|
|<span data-ttu-id="016ec-116">Application</span><span class="sxs-lookup"><span data-stu-id="016ec-116">Application</span></span>|<span data-ttu-id="016ec-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="016ec-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="016ec-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="016ec-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases/{id}/reviewSets
```

## <a name="request-headers"></a><span data-ttu-id="016ec-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="016ec-119">Request headers</span></span>

| <span data-ttu-id="016ec-120">名称</span><span class="sxs-lookup"><span data-stu-id="016ec-120">Name</span></span>       | <span data-ttu-id="016ec-121">说明</span><span class="sxs-lookup"><span data-stu-id="016ec-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="016ec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="016ec-122">Authorization</span></span> | <span data-ttu-id="016ec-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="016ec-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="016ec-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="016ec-125">Request body</span></span>

<span data-ttu-id="016ec-126">在请求正文中，提供 reviewSet 的 JSON [表示形式](../resources/ediscovery-reviewset.md)。</span><span class="sxs-lookup"><span data-stu-id="016ec-126">In the request body, supply JSON representation of the [reviewSet](../resources/ediscovery-reviewset.md).</span></span>  <span data-ttu-id="016ec-127">下表列出了所需的属性。</span><span class="sxs-lookup"><span data-stu-id="016ec-127">The following table lists the required properties.</span></span>

| <span data-ttu-id="016ec-128">属性</span><span class="sxs-lookup"><span data-stu-id="016ec-128">Property</span></span>     | <span data-ttu-id="016ec-129">类型</span><span class="sxs-lookup"><span data-stu-id="016ec-129">Type</span></span>        | <span data-ttu-id="016ec-130">说明</span><span class="sxs-lookup"><span data-stu-id="016ec-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="016ec-131">displayName</span><span class="sxs-lookup"><span data-stu-id="016ec-131">displayName</span></span>  | <span data-ttu-id="016ec-132">string</span><span class="sxs-lookup"><span data-stu-id="016ec-132">string</span></span>      | <span data-ttu-id="016ec-133">审阅集的名称。</span><span class="sxs-lookup"><span data-stu-id="016ec-133">The name of the review set.</span></span> |

## <a name="response"></a><span data-ttu-id="016ec-134">响应</span><span class="sxs-lookup"><span data-stu-id="016ec-134">Response</span></span>

<span data-ttu-id="016ec-135">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="016ec-135">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="016ec-136">示例</span><span class="sxs-lookup"><span data-stu-id="016ec-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="016ec-137">请求</span><span class="sxs-lookup"><span data-stu-id="016ec-137">Request</span></span>

<span data-ttu-id="016ec-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="016ec-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="016ec-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="016ec-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reviewset"
}-->

```http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets
Content-type: application/json

{
  "displayName": "My Reviewset 3",
}
```
# <a name="c"></a>[<span data-ttu-id="016ec-140">C#</span><span class="sxs-lookup"><span data-stu-id="016ec-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reviewset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="016ec-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="016ec-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reviewset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="016ec-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="016ec-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reviewset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="016ec-143">Java</span><span class="sxs-lookup"><span data-stu-id="016ec-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reviewset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="016ec-144">响应</span><span class="sxs-lookup"><span data-stu-id="016ec-144">Response</span></span>

<span data-ttu-id="016ec-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="016ec-145">The following is an example of the response.</span></span>

> <span data-ttu-id="016ec-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="016ec-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.reviewSet"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d')/reviewSets/$entity",
    "id": "0157910c-57ce-4e48-bd4b-90f3c88ca32e",
    "displayName": "My Reviewset 3",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-03-11T08:40:14.9486058Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update reviewset",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


