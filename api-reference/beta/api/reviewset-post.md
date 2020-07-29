---
title: 创建 reviewSet
description: 创建电子数据展示检查集。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: c16ef3c9e325e3c144cdec532cc81e6e31623138
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510018"
---
# <a name="create-reviewset"></a><span data-ttu-id="bada3-103">创建 reviewSet</span><span class="sxs-lookup"><span data-stu-id="bada3-103">Create reviewSet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bada3-104">创建新的[reviewSet](../resources/reviewset.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bada3-104">Create a new [reviewSet](../resources/reviewset.md) object.</span></span> <span data-ttu-id="bada3-105">请求正文包含审阅集的显示名称，该名称是唯一的可写属性。</span><span class="sxs-lookup"><span data-stu-id="bada3-105">The request body contains the display name of the review set, which is the only writable property.</span></span>

## <a name="permissions"></a><span data-ttu-id="bada3-106">权限</span><span class="sxs-lookup"><span data-stu-id="bada3-106">Permissions</span></span>

<span data-ttu-id="bada3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bada3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bada3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bada3-109">Permission type</span></span>                        | <span data-ttu-id="bada3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bada3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bada3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bada3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bada3-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="bada3-112">User.Read</span></span> |
| <span data-ttu-id="bada3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bada3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bada3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bada3-114">Not supported.</span></span> |
| <span data-ttu-id="bada3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bada3-115">Application</span></span>                            | <span data-ttu-id="bada3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bada3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bada3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bada3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases/{id}/reviewSets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bada3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bada3-118">Request headers</span></span>

| <span data-ttu-id="bada3-119">名称</span><span class="sxs-lookup"><span data-stu-id="bada3-119">Name</span></span>       | <span data-ttu-id="bada3-120">说明</span><span class="sxs-lookup"><span data-stu-id="bada3-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bada3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bada3-121">Authorization</span></span> | <span data-ttu-id="bada3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bada3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bada3-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="bada3-124">Request body</span></span>

<span data-ttu-id="bada3-125">在请求正文中，提供[reviewSet](../resources/reviewset.md)的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bada3-125">In the request body, supply JSON representation of the [reviewSet](../resources/reviewset.md).</span></span>  <span data-ttu-id="bada3-126">下表列出了必需的属性。</span><span class="sxs-lookup"><span data-stu-id="bada3-126">The following table lists the required properties.</span></span>

| <span data-ttu-id="bada3-127">属性</span><span class="sxs-lookup"><span data-stu-id="bada3-127">Property</span></span>     | <span data-ttu-id="bada3-128">类型</span><span class="sxs-lookup"><span data-stu-id="bada3-128">Type</span></span>        | <span data-ttu-id="bada3-129">说明</span><span class="sxs-lookup"><span data-stu-id="bada3-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bada3-130">displayName</span><span class="sxs-lookup"><span data-stu-id="bada3-130">displayName</span></span>  | <span data-ttu-id="bada3-131">string</span><span class="sxs-lookup"><span data-stu-id="bada3-131">string</span></span>      | <span data-ttu-id="bada3-132">评审集的名称。</span><span class="sxs-lookup"><span data-stu-id="bada3-132">The name of the review set.</span></span> |

## <a name="response"></a><span data-ttu-id="bada3-133">响应</span><span class="sxs-lookup"><span data-stu-id="bada3-133">Response</span></span>

<span data-ttu-id="bada3-134">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[reviewSet](../resources/reviewset.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bada3-134">If successful, this method returns a `201 Created` response code and a [reviewSet](../resources/reviewset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bada3-135">示例</span><span class="sxs-lookup"><span data-stu-id="bada3-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bada3-136">请求</span><span class="sxs-lookup"><span data-stu-id="bada3-136">Request</span></span>

<span data-ttu-id="bada3-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bada3-137">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bada3-138">响应</span><span class="sxs-lookup"><span data-stu-id="bada3-138">Response</span></span>

<span data-ttu-id="bada3-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bada3-139">The following is an example of the response.</span></span>

> <span data-ttu-id="bada3-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bada3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSet"
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
