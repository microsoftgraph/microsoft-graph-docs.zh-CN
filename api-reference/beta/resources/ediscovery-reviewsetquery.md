---
title: reviewSetQuery 资源类型
description: 表示审阅集查询，用于查询和剔除电子数据展示 reviewSet 中存储的数据。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: f9c535cb1adbb62f33aee1324b6dc06a910f4b46
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446151"
---
# <a name="reviewsetquery-resource-type"></a><span data-ttu-id="76f6f-103">reviewSetQuery 资源类型</span><span class="sxs-lookup"><span data-stu-id="76f6f-103">reviewSetQuery resource type</span></span>

<span data-ttu-id="76f6f-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="76f6f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76f6f-105">表示审阅集查询，用于查询和剔除电子数据展示 [reviewSet 中存储的数据](ediscovery-reviewset.md)。</span><span class="sxs-lookup"><span data-stu-id="76f6f-105">Represents a review set query, which is used to query and cull data stored in an eDiscovery [reviewSet](ediscovery-reviewset.md).</span></span>

## <a name="methods"></a><span data-ttu-id="76f6f-106">Methods</span><span class="sxs-lookup"><span data-stu-id="76f6f-106">Methods</span></span>

| <span data-ttu-id="76f6f-107">方法</span><span class="sxs-lookup"><span data-stu-id="76f6f-107">Method</span></span>       | <span data-ttu-id="76f6f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="76f6f-108">Return Type</span></span> | <span data-ttu-id="76f6f-109">说明</span><span class="sxs-lookup"><span data-stu-id="76f6f-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="76f6f-110">列出查询</span><span class="sxs-lookup"><span data-stu-id="76f6f-110">List queries</span></span>](../api/ediscovery-reviewsetquery-list.md) | <span data-ttu-id="76f6f-111">[microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) 集合</span><span class="sxs-lookup"><span data-stu-id="76f6f-111">[microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) collection</span></span> | <span data-ttu-id="76f6f-112">在审阅集内列出审阅集查询。</span><span class="sxs-lookup"><span data-stu-id="76f6f-112">List the review set queries in a review set.</span></span> |
| [<span data-ttu-id="76f6f-113">创建查询</span><span class="sxs-lookup"><span data-stu-id="76f6f-113">Create queries</span></span>](../api/ediscovery-reviewsetquery-post.md) | [<span data-ttu-id="76f6f-114">microsoft.graph.ediscovery.reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="76f6f-114">microsoft.graph.ediscovery.reviewSetQuery</span></span>](ediscovery-reviewsetquery.md) | <span data-ttu-id="76f6f-115">创建新的审阅集查询。</span><span class="sxs-lookup"><span data-stu-id="76f6f-115">Create a new review set query.</span></span> |
| [<span data-ttu-id="76f6f-116">获取查询</span><span class="sxs-lookup"><span data-stu-id="76f6f-116">Get queries</span></span>](../api/ediscovery-reviewsetquery-get.md) | [<span data-ttu-id="76f6f-117">microsoft.graph.ediscovery.reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="76f6f-117">microsoft.graph.ediscovery.reviewSetQuery</span></span>](ediscovery-reviewsetquery.md) | <span data-ttu-id="76f6f-118">读取 **reviewSetQuery** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="76f6f-118">Read the properties and relationships of a **reviewSetQuery** object.</span></span> |
| [<span data-ttu-id="76f6f-119">更新 reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="76f6f-119">Update reviewSetQuery</span></span>](../api/ediscovery-reviewsetquery-update.md) | <span data-ttu-id="76f6f-120">无</span><span class="sxs-lookup"><span data-stu-id="76f6f-120">None</span></span> | <span data-ttu-id="76f6f-121">更新审阅集查询。</span><span class="sxs-lookup"><span data-stu-id="76f6f-121">Update a review set query.</span></span> |
| [<span data-ttu-id="76f6f-122">删除 reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="76f6f-122">Delete reviewSetQuery</span></span>](../api/ediscovery-reviewsetquery-delete.md) | <span data-ttu-id="76f6f-123">无</span><span class="sxs-lookup"><span data-stu-id="76f6f-123">None</span></span> | <span data-ttu-id="76f6f-124">删除审阅集查询。</span><span class="sxs-lookup"><span data-stu-id="76f6f-124">Delete review set query.</span></span> |
| [<span data-ttu-id="76f6f-125">applyTags</span><span class="sxs-lookup"><span data-stu-id="76f6f-125">applyTags</span></span>](../api/ediscovery-reviewsetquery-applytags.md)|<span data-ttu-id="76f6f-126">无</span><span class="sxs-lookup"><span data-stu-id="76f6f-126">None</span></span>|<span data-ttu-id="76f6f-127">将标记应用于与指定查询匹配的文档。</span><span class="sxs-lookup"><span data-stu-id="76f6f-127">Apply tags to documents that match the specified query.</span></span>|

## <a name="properties"></a><span data-ttu-id="76f6f-128">属性</span><span class="sxs-lookup"><span data-stu-id="76f6f-128">Properties</span></span>

| <span data-ttu-id="76f6f-129">属性</span><span class="sxs-lookup"><span data-stu-id="76f6f-129">Property</span></span>     | <span data-ttu-id="76f6f-130">类型</span><span class="sxs-lookup"><span data-stu-id="76f6f-130">Type</span></span>        | <span data-ttu-id="76f6f-131">说明</span><span class="sxs-lookup"><span data-stu-id="76f6f-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="76f6f-132">createdBy</span><span class="sxs-lookup"><span data-stu-id="76f6f-132">createdBy</span></span> | [<span data-ttu-id="76f6f-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="76f6f-133">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="76f6f-134">创建查询的用户。</span><span class="sxs-lookup"><span data-stu-id="76f6f-134">The user who created the query.</span></span> |
| <span data-ttu-id="76f6f-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76f6f-135">createdDateTime</span></span> |<span data-ttu-id="76f6f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76f6f-136">DateTimeOffset</span></span>| <span data-ttu-id="76f6f-137">创建查询的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="76f6f-137">The time and date when the query was created.</span></span> <span data-ttu-id="76f6f-138">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="76f6f-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="76f6f-139">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="76f6f-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="76f6f-140">displayName</span><span class="sxs-lookup"><span data-stu-id="76f6f-140">displayName</span></span> | <span data-ttu-id="76f6f-141">String</span><span class="sxs-lookup"><span data-stu-id="76f6f-141">String</span></span> | <span data-ttu-id="76f6f-142">查询的名称。</span><span class="sxs-lookup"><span data-stu-id="76f6f-142">The name of the query.</span></span>|
| <span data-ttu-id="76f6f-143">id</span><span class="sxs-lookup"><span data-stu-id="76f6f-143">id</span></span> |<span data-ttu-id="76f6f-144">String</span><span class="sxs-lookup"><span data-stu-id="76f6f-144">String</span></span>| <span data-ttu-id="76f6f-145">查询的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="76f6f-145">The unique identifier of the query.</span></span> <span data-ttu-id="76f6f-146">只读。</span><span class="sxs-lookup"><span data-stu-id="76f6f-146">Read-only.</span></span>|
| <span data-ttu-id="76f6f-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="76f6f-147">lastModifiedBy</span></span> | [<span data-ttu-id="76f6f-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="76f6f-148">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="76f6f-149">上次修改查询的用户。</span><span class="sxs-lookup"><span data-stu-id="76f6f-149">The user who last modified the query.</span></span> |
| <span data-ttu-id="76f6f-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76f6f-150">lastModifiedDateTime</span></span> |<span data-ttu-id="76f6f-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76f6f-151">DateTimeOffset</span></span> | <span data-ttu-id="76f6f-152">上次修改查询的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="76f6f-152">The date and time the query was last modified.</span></span> <span data-ttu-id="76f6f-153">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="76f6f-153">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="76f6f-154">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="76f6f-154">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="76f6f-155">查询</span><span class="sxs-lookup"><span data-stu-id="76f6f-155">query</span></span> | <span data-ttu-id="76f6f-156">String</span><span class="sxs-lookup"><span data-stu-id="76f6f-156">String</span></span> | <span data-ttu-id="76f6f-157">KQL 中的查询字符串 (关键字查询语言) 查询。</span><span class="sxs-lookup"><span data-stu-id="76f6f-157">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="76f6f-158">有关详细信息，请参阅 [高级电子数据展示中的文档元数据字段](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery)。</span><span class="sxs-lookup"><span data-stu-id="76f6f-158">For details, see [Document metadata fields in Advanced eDiscovery](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span></span>  <span data-ttu-id="76f6f-159">此字段直接映射到关键字条件。</span><span class="sxs-lookup"><span data-stu-id="76f6f-159">This field maps directly to the keywords condition.</span></span>  <span data-ttu-id="76f6f-160">您可以使用与值配对的可搜索字段 *名称中列出的字段来* 优化搜索;例如 *，subject："Quarterly Financials" and Date>=06/01/2016 AND Date<=07/01/2016*.</span><span class="sxs-lookup"><span data-stu-id="76f6f-160">You can refine searches by using fields listed in the *searchable field name* paired with values; for example, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*.</span></span> |

## <a name="relationships"></a><span data-ttu-id="76f6f-161">关系</span><span class="sxs-lookup"><span data-stu-id="76f6f-161">Relationships</span></span>

<span data-ttu-id="76f6f-162">无。</span><span class="sxs-lookup"><span data-stu-id="76f6f-162">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="76f6f-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76f6f-163">JSON representation</span></span>

<span data-ttu-id="76f6f-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76f6f-164">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.ediscovery.reviewSetQuery",
  "query": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reviewSetQuery resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
