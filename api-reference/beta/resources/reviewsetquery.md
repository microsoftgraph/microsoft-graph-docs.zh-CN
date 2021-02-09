---
title: reviewSetQuery 资源类型
description: 审阅集查询用于查询和剔除电子数据展示 reviewSet 中存储的数据
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: f622f79c9103e704be93ffd97af37c1d188736f6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153485"
---
# <a name="reviewsetquery-resource-type"></a><span data-ttu-id="e31e1-103">reviewSetQuery 资源类型</span><span class="sxs-lookup"><span data-stu-id="e31e1-103">reviewSetQuery resource type</span></span>

<span data-ttu-id="e31e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e31e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e31e1-105">审阅集查询用于查询和剔除电子数据展示 [reviewSet 中存储的数据](reviewset.md)。</span><span class="sxs-lookup"><span data-stu-id="e31e1-105">Review set queries are used to query and cull data stored in an eDiscovery [reviewSet](reviewset.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e31e1-106">方法</span><span class="sxs-lookup"><span data-stu-id="e31e1-106">Methods</span></span>

| <span data-ttu-id="e31e1-107">方法</span><span class="sxs-lookup"><span data-stu-id="e31e1-107">Method</span></span>       | <span data-ttu-id="e31e1-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="e31e1-108">Return Type</span></span> | <span data-ttu-id="e31e1-109">说明</span><span class="sxs-lookup"><span data-stu-id="e31e1-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e31e1-110">列出查询</span><span class="sxs-lookup"><span data-stu-id="e31e1-110">List queries</span></span>](../api/reviewsetquery-list.md) | <span data-ttu-id="e31e1-111">[reviewSetQuery](reviewsetquery.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e31e1-111">[reviewSetQuery](reviewsetquery.md) collection</span></span> | <span data-ttu-id="e31e1-112">在审阅集内列出审阅集查询。</span><span class="sxs-lookup"><span data-stu-id="e31e1-112">List the review set queries in a review set.</span></span> |
| [<span data-ttu-id="e31e1-113">创建查询</span><span class="sxs-lookup"><span data-stu-id="e31e1-113">Create queries</span></span>](../api/reviewsetquery-post.md) | [<span data-ttu-id="e31e1-114">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="e31e1-114">reviewSetQuery</span></span>](reviewsetquery.md) | <span data-ttu-id="e31e1-115">创建新的审阅集查询。</span><span class="sxs-lookup"><span data-stu-id="e31e1-115">Create a new review set query.</span></span> |
| [<span data-ttu-id="e31e1-116">获取查询</span><span class="sxs-lookup"><span data-stu-id="e31e1-116">Get queries</span></span>](../api/reviewsetquery-get.md) | [<span data-ttu-id="e31e1-117">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="e31e1-117">reviewSetQuery</span></span>](reviewsetquery.md) | <span data-ttu-id="e31e1-118">读取 **reviewSetQuery** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e31e1-118">Read the properties and relationships of a **reviewSetQuery** object.</span></span> |
| [<span data-ttu-id="e31e1-119">更新查询</span><span class="sxs-lookup"><span data-stu-id="e31e1-119">Update queries</span></span>](../api/reviewsetquery-update.md) | <span data-ttu-id="e31e1-120">无</span><span class="sxs-lookup"><span data-stu-id="e31e1-120">None</span></span> | <span data-ttu-id="e31e1-121">更新审阅集查询。</span><span class="sxs-lookup"><span data-stu-id="e31e1-121">Update a review set query.</span></span> |
| [<span data-ttu-id="e31e1-122">删除查询</span><span class="sxs-lookup"><span data-stu-id="e31e1-122">Delete queries</span></span>](../api/reviewsetquery-delete.md) | <span data-ttu-id="e31e1-123">无</span><span class="sxs-lookup"><span data-stu-id="e31e1-123">None</span></span> | <span data-ttu-id="e31e1-124">删除审阅集查询。</span><span class="sxs-lookup"><span data-stu-id="e31e1-124">Delete review set query.</span></span> |

## <a name="properties"></a><span data-ttu-id="e31e1-125">属性</span><span class="sxs-lookup"><span data-stu-id="e31e1-125">Properties</span></span>

| <span data-ttu-id="e31e1-126">属性</span><span class="sxs-lookup"><span data-stu-id="e31e1-126">Property</span></span>     | <span data-ttu-id="e31e1-127">类型</span><span class="sxs-lookup"><span data-stu-id="e31e1-127">Type</span></span>        | <span data-ttu-id="e31e1-128">说明</span><span class="sxs-lookup"><span data-stu-id="e31e1-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e31e1-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="e31e1-129">createdBy</span></span> | [<span data-ttu-id="e31e1-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="e31e1-130">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="e31e1-131">创建查询的用户。</span><span class="sxs-lookup"><span data-stu-id="e31e1-131">The user who created the query.</span></span> |
| <span data-ttu-id="e31e1-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e31e1-132">createdDateTime</span></span> |<span data-ttu-id="e31e1-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e31e1-133">DateTimeOffset</span></span>| <span data-ttu-id="e31e1-134">创建查询的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="e31e1-134">The time and date when the query was created.</span></span> <span data-ttu-id="e31e1-135">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="e31e1-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e31e1-136">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e31e1-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="e31e1-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e31e1-137">displayName</span></span> | <span data-ttu-id="e31e1-138">String</span><span class="sxs-lookup"><span data-stu-id="e31e1-138">String</span></span> | <span data-ttu-id="e31e1-139">查询的名称</span><span class="sxs-lookup"><span data-stu-id="e31e1-139">The name of the query</span></span>|
| <span data-ttu-id="e31e1-140">id</span><span class="sxs-lookup"><span data-stu-id="e31e1-140">id</span></span> |<span data-ttu-id="e31e1-141">String</span><span class="sxs-lookup"><span data-stu-id="e31e1-141">String</span></span>| <span data-ttu-id="e31e1-142">查询的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e31e1-142">The unique identifier of the query.</span></span> <span data-ttu-id="e31e1-143">只读。</span><span class="sxs-lookup"><span data-stu-id="e31e1-143">Read-only.</span></span>|
| <span data-ttu-id="e31e1-144">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="e31e1-144">lastModifiedBy</span></span> | [<span data-ttu-id="e31e1-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="e31e1-145">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="e31e1-146">上次修改查询的用户。</span><span class="sxs-lookup"><span data-stu-id="e31e1-146">The user who last modified the query.</span></span> |
| <span data-ttu-id="e31e1-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e31e1-147">lastModifiedDateTime</span></span> |<span data-ttu-id="e31e1-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e31e1-148">DateTimeOffset</span></span> | <span data-ttu-id="e31e1-149">上次修改查询的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e31e1-149">The date and time the query was last modified.</span></span> <span data-ttu-id="e31e1-150">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="e31e1-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e31e1-151">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e31e1-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="e31e1-152">查询</span><span class="sxs-lookup"><span data-stu-id="e31e1-152">query</span></span> | <span data-ttu-id="e31e1-153">String</span><span class="sxs-lookup"><span data-stu-id="e31e1-153">String</span></span> | <span data-ttu-id="e31e1-154">KQL 中的查询字符串 (关键字查询语言) 查询。</span><span class="sxs-lookup"><span data-stu-id="e31e1-154">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="e31e1-155">有关详细信息，请参阅 [高级电子数据展示中的文档元数据字段](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery)。</span><span class="sxs-lookup"><span data-stu-id="e31e1-155">For details, see [Document metadata fields in Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span></span>  <span data-ttu-id="e31e1-156">此字段直接映射到关键字条件。</span><span class="sxs-lookup"><span data-stu-id="e31e1-156">This field maps directly to the keywords condition.</span></span>  <span data-ttu-id="e31e1-157">您可以使用与值配对的可搜索字段名称 *中列出的字段来* 优化搜索;例如 *，subject："Quarterly Financials"AND Date>=06/01/2016 AND Date<=07/01/2016*</span><span class="sxs-lookup"><span data-stu-id="e31e1-157">You can refine searches by using fields listed in the *searchable field name* paired with values; for example, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*</span></span> |

## <a name="relationships"></a><span data-ttu-id="e31e1-158">关系</span><span class="sxs-lookup"><span data-stu-id="e31e1-158">Relationships</span></span>

<span data-ttu-id="e31e1-159">无。</span><span class="sxs-lookup"><span data-stu-id="e31e1-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e31e1-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e31e1-160">JSON representation</span></span>

<span data-ttu-id="e31e1-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e31e1-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSetQuery",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.reviewSetQuery",
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
