---
title: reviewSet 资源类型
description: 表示收集用于诉讼、调查或监管请求的静态电子存储信息集。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 25c33dd911d9c14d91131508fad37c1fea149b9a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446152"
---
# <a name="reviewset-resource-type"></a><span data-ttu-id="15807-103">reviewSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="15807-103">reviewSet resource type</span></span>

<span data-ttu-id="15807-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="15807-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15807-105">表示收集用于诉讼、调查或监管请求的静态电子存储信息集。</span><span class="sxs-lookup"><span data-stu-id="15807-105">Represents static set of electronically stored information collected for use in a litigation, investigation, or regulatory request.</span></span>

## <a name="methods"></a><span data-ttu-id="15807-106">Methods</span><span class="sxs-lookup"><span data-stu-id="15807-106">Methods</span></span>

| <span data-ttu-id="15807-107">方法</span><span class="sxs-lookup"><span data-stu-id="15807-107">Method</span></span>       | <span data-ttu-id="15807-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="15807-108">Return Type</span></span> | <span data-ttu-id="15807-109">说明</span><span class="sxs-lookup"><span data-stu-id="15807-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="15807-110">列出 reviewSets</span><span class="sxs-lookup"><span data-stu-id="15807-110">List reviewSets</span></span>](../api/ediscovery-case-list-reviewsets.md) | <span data-ttu-id="15807-111">[microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="15807-111">[microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) collection</span></span> | <span data-ttu-id="15807-112">获取 **reviewset 对象** 的集合。</span><span class="sxs-lookup"><span data-stu-id="15807-112">Get a collection of **reviewset** objects.</span></span> |
| [<span data-ttu-id="15807-113">创建 reviewSet</span><span class="sxs-lookup"><span data-stu-id="15807-113">Create reviewSet</span></span>](../api/ediscovery-case-post-reviewsets.md) | [<span data-ttu-id="15807-114">microsoft.graph.ediscovery.reviewSet</span><span class="sxs-lookup"><span data-stu-id="15807-114">microsoft.graph.ediscovery.reviewSet</span></span>](../resources/ediscovery-reviewset.md) | <span data-ttu-id="15807-115">创建新的 **审阅集**。</span><span class="sxs-lookup"><span data-stu-id="15807-115">Create a new **reviewset**.</span></span> |
| [<span data-ttu-id="15807-116">获取 reviewSet</span><span class="sxs-lookup"><span data-stu-id="15807-116">Get reviewSet</span></span>](../api/ediscovery-reviewset-get.md) | [<span data-ttu-id="15807-117">microsoft.graph.ediscovery.reviewSet</span><span class="sxs-lookup"><span data-stu-id="15807-117">microsoft.graph.ediscovery.reviewSet</span></span>](../resources/ediscovery-reviewset.md) | <span data-ttu-id="15807-118">读取 **reviewSet 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="15807-118">Read the properties and relationships of a **reviewSet** object.</span></span> |
| [<span data-ttu-id="15807-119">列出查询</span><span class="sxs-lookup"><span data-stu-id="15807-119">List queries</span></span>](../api/ediscovery-reviewsetquery-list.md)|<span data-ttu-id="15807-120">[microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) 集合</span><span class="sxs-lookup"><span data-stu-id="15807-120">[microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) collection</span></span>|<span data-ttu-id="15807-121">获取 **reviewSetQuery 资源** 的列表。</span><span class="sxs-lookup"><span data-stu-id="15807-121">Get a list of **reviewSetQuery** resources.</span></span>|
| [<span data-ttu-id="15807-122">export</span><span class="sxs-lookup"><span data-stu-id="15807-122">export</span></span>](../api/ediscovery-reviewset-export.md) | <span data-ttu-id="15807-123">无</span><span class="sxs-lookup"><span data-stu-id="15807-123">None</span></span> | <span data-ttu-id="15807-124">启动从审阅集导出 **数据**。</span><span class="sxs-lookup"><span data-stu-id="15807-124">Initiate an export of data from the **reviewset**.</span></span> |
| [<span data-ttu-id="15807-125">addToReviewSet</span><span class="sxs-lookup"><span data-stu-id="15807-125">addToReviewSet</span></span>](../api/ediscovery-reviewset-addtoreviewset.md)|<span data-ttu-id="15807-126">无</span><span class="sxs-lookup"><span data-stu-id="15807-126">None</span></span>|<span data-ttu-id="15807-127">将数据从 **sourceCollection** 添加到 **审阅集**。</span><span class="sxs-lookup"><span data-stu-id="15807-127">Add data from a **sourceCollection** to a **reviewset**.</span></span>|

## <a name="properties"></a><span data-ttu-id="15807-128">属性</span><span class="sxs-lookup"><span data-stu-id="15807-128">Properties</span></span>

| <span data-ttu-id="15807-129">属性</span><span class="sxs-lookup"><span data-stu-id="15807-129">Property</span></span>     | <span data-ttu-id="15807-130">类型</span><span class="sxs-lookup"><span data-stu-id="15807-130">Type</span></span>        | <span data-ttu-id="15807-131">说明</span><span class="sxs-lookup"><span data-stu-id="15807-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="15807-132">createdBy</span><span class="sxs-lookup"><span data-stu-id="15807-132">createdBy</span></span>        | [<span data-ttu-id="15807-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="15807-133">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="15807-134">创建审阅集的用户。</span><span class="sxs-lookup"><span data-stu-id="15807-134">The user who created the review set.</span></span> <span data-ttu-id="15807-135">只读。</span><span class="sxs-lookup"><span data-stu-id="15807-135">Read-only.</span></span> |
|<span data-ttu-id="15807-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15807-136">createdDateTime</span></span>  |<span data-ttu-id="15807-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15807-137">DateTimeOffset</span></span>| <span data-ttu-id="15807-138">创建审阅集的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="15807-138">The datetime when the review set was created.</span></span> <span data-ttu-id="15807-139">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="15807-139">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="15807-140">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="15807-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="15807-141">只读。</span><span class="sxs-lookup"><span data-stu-id="15807-141">Read-only.</span></span> |
|<span data-ttu-id="15807-142">displayName</span><span class="sxs-lookup"><span data-stu-id="15807-142">displayName</span></span>      |<span data-ttu-id="15807-143">String</span><span class="sxs-lookup"><span data-stu-id="15807-143">String</span></span>| <span data-ttu-id="15807-144">审阅集名称。</span><span class="sxs-lookup"><span data-stu-id="15807-144">The review set name.</span></span> <span data-ttu-id="15807-145">该名称是唯一的，最大限制为 64 个字符。</span><span class="sxs-lookup"><span data-stu-id="15807-145">The name is unique with a maximum limit of 64 characters.</span></span> |
|<span data-ttu-id="15807-146">id</span><span class="sxs-lookup"><span data-stu-id="15807-146">id</span></span>               |<span data-ttu-id="15807-147">String</span><span class="sxs-lookup"><span data-stu-id="15807-147">String</span></span>| <span data-ttu-id="15807-148">审阅集唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="15807-148">The review set unique identifier.</span></span> <span data-ttu-id="15807-149">只读。</span><span class="sxs-lookup"><span data-stu-id="15807-149">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="15807-150">关系</span><span class="sxs-lookup"><span data-stu-id="15807-150">Relationships</span></span>

| <span data-ttu-id="15807-151">关系</span><span class="sxs-lookup"><span data-stu-id="15807-151">Relationship</span></span> | <span data-ttu-id="15807-152">类型</span><span class="sxs-lookup"><span data-stu-id="15807-152">Type</span></span>        | <span data-ttu-id="15807-153">说明</span><span class="sxs-lookup"><span data-stu-id="15807-153">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="15807-154">查询</span><span class="sxs-lookup"><span data-stu-id="15807-154">queries</span></span> |<span data-ttu-id="15807-155">[microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) 集合</span><span class="sxs-lookup"><span data-stu-id="15807-155">[microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) collection</span></span>| <span data-ttu-id="15807-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="15807-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="15807-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15807-158">JSON representation</span></span>

<span data-ttu-id="15807-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15807-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ediscovery.reviewSet",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.ediscovery.reviewSet",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reviewSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
