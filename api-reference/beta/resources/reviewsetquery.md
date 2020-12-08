---
title: reviewSetQuery 资源类型
description: 审阅集查询用于查询和精选电子数据展示 reviewSet 中存储的数据
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 7ffea670daffb6c8ce53925096dbd4f2d4986477
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597257"
---
# <a name="reviewsetquery-resource-type"></a><span data-ttu-id="de227-103">reviewSetQuery 资源类型</span><span class="sxs-lookup"><span data-stu-id="de227-103">reviewSetQuery resource type</span></span>

<span data-ttu-id="de227-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de227-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de227-105">审查集查询用于查询和挑选电子数据展示 [reviewSet](reviewset.md)中存储的数据。</span><span class="sxs-lookup"><span data-stu-id="de227-105">Review set queries are used to query and cull data stored in an eDiscovery [reviewSet](reviewset.md).</span></span>

## <a name="methods"></a><span data-ttu-id="de227-106">方法</span><span class="sxs-lookup"><span data-stu-id="de227-106">Methods</span></span>

| <span data-ttu-id="de227-107">方法</span><span class="sxs-lookup"><span data-stu-id="de227-107">Method</span></span>       | <span data-ttu-id="de227-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="de227-108">Return Type</span></span> | <span data-ttu-id="de227-109">Description</span><span class="sxs-lookup"><span data-stu-id="de227-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="de227-110">列出查询</span><span class="sxs-lookup"><span data-stu-id="de227-110">List queries</span></span>](../api/reviewsetquery-list.md) | <span data-ttu-id="de227-111">[reviewSetQuery](reviewsetquery.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de227-111">[reviewSetQuery](reviewsetquery.md) collection</span></span> | <span data-ttu-id="de227-112">在审阅集中列出审阅集查询。</span><span class="sxs-lookup"><span data-stu-id="de227-112">List the review set queries in a review set.</span></span> |
| [<span data-ttu-id="de227-113">创建查询</span><span class="sxs-lookup"><span data-stu-id="de227-113">Create queries</span></span>](../api/reviewsetquery-post.md) | [<span data-ttu-id="de227-114">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="de227-114">reviewSetQuery</span></span>](reviewsetquery.md) | <span data-ttu-id="de227-115">创建新的审阅集查询。</span><span class="sxs-lookup"><span data-stu-id="de227-115">Create a new review set query.</span></span> |
| [<span data-ttu-id="de227-116">获取查询</span><span class="sxs-lookup"><span data-stu-id="de227-116">Get queries</span></span>](../api/reviewsetquery-get.md) | [<span data-ttu-id="de227-117">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="de227-117">reviewSetQuery</span></span>](reviewsetquery.md) | <span data-ttu-id="de227-118">读取 **reviewSetQuery** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="de227-118">Read the properties and relationships of a **reviewSetQuery** object.</span></span> |
| [<span data-ttu-id="de227-119">更新查询</span><span class="sxs-lookup"><span data-stu-id="de227-119">Update queries</span></span>](../api/reviewsetquery-update.md) | <span data-ttu-id="de227-120">无</span><span class="sxs-lookup"><span data-stu-id="de227-120">None</span></span> | <span data-ttu-id="de227-121">更新审阅集查询。</span><span class="sxs-lookup"><span data-stu-id="de227-121">Update a review set query.</span></span> |
| [<span data-ttu-id="de227-122">删除查询</span><span class="sxs-lookup"><span data-stu-id="de227-122">Delete queries</span></span>](../api/reviewsetquery-delete.md) | <span data-ttu-id="de227-123">无</span><span class="sxs-lookup"><span data-stu-id="de227-123">None</span></span> | <span data-ttu-id="de227-124">删除审阅集查询。</span><span class="sxs-lookup"><span data-stu-id="de227-124">Delete review set query.</span></span> |

## <a name="properties"></a><span data-ttu-id="de227-125">属性</span><span class="sxs-lookup"><span data-stu-id="de227-125">Properties</span></span>

| <span data-ttu-id="de227-126">属性</span><span class="sxs-lookup"><span data-stu-id="de227-126">Property</span></span>     | <span data-ttu-id="de227-127">类型</span><span class="sxs-lookup"><span data-stu-id="de227-127">Type</span></span>        | <span data-ttu-id="de227-128">说明</span><span class="sxs-lookup"><span data-stu-id="de227-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="de227-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="de227-129">createdBy</span></span> | [<span data-ttu-id="de227-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="de227-130">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="de227-131">创建查询的用户。</span><span class="sxs-lookup"><span data-stu-id="de227-131">The user who created the query.</span></span> |
| <span data-ttu-id="de227-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de227-132">createdDateTime</span></span> |<span data-ttu-id="de227-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de227-133">DateTimeOffset</span></span>| <span data-ttu-id="de227-134">创建查询的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="de227-134">The time and date when the query was created.</span></span> <span data-ttu-id="de227-135">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="de227-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="de227-136">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="de227-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="de227-137">displayName</span><span class="sxs-lookup"><span data-stu-id="de227-137">displayName</span></span> | <span data-ttu-id="de227-138">String</span><span class="sxs-lookup"><span data-stu-id="de227-138">String</span></span> | <span data-ttu-id="de227-139">查询的名称</span><span class="sxs-lookup"><span data-stu-id="de227-139">The name of the query</span></span>|
| <span data-ttu-id="de227-140">id</span><span class="sxs-lookup"><span data-stu-id="de227-140">id</span></span> |<span data-ttu-id="de227-141">String</span><span class="sxs-lookup"><span data-stu-id="de227-141">String</span></span>| <span data-ttu-id="de227-142">查询的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="de227-142">The unique identifier of the query.</span></span> <span data-ttu-id="de227-143">只读。</span><span class="sxs-lookup"><span data-stu-id="de227-143">Read-only.</span></span>|
| <span data-ttu-id="de227-144">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="de227-144">lastModifiedBy</span></span> | [<span data-ttu-id="de227-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="de227-145">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="de227-146">上次修改查询的用户。</span><span class="sxs-lookup"><span data-stu-id="de227-146">The user who last modified the query.</span></span> |
| <span data-ttu-id="de227-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de227-147">lastModifiedDateTime</span></span> |<span data-ttu-id="de227-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de227-148">DateTimeOffset</span></span> | <span data-ttu-id="de227-149">上次修改查询的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="de227-149">The date and time the query was last modified.</span></span> <span data-ttu-id="de227-150">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="de227-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="de227-151">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="de227-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="de227-152">查询</span><span class="sxs-lookup"><span data-stu-id="de227-152">query</span></span> | <span data-ttu-id="de227-153">String</span><span class="sxs-lookup"><span data-stu-id="de227-153">String</span></span> | <span data-ttu-id="de227-154">KQL (关键字查询语言) 查询中的查询字符串。</span><span class="sxs-lookup"><span data-stu-id="de227-154">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="de227-155">有关详细信息，请参阅 [高级电子数据展示中的文档元数据字段](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery)。</span><span class="sxs-lookup"><span data-stu-id="de227-155">For details, see [Document metadata fields in Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span></span>  <span data-ttu-id="de227-156">此字段直接映射到关键字条件。</span><span class="sxs-lookup"><span data-stu-id="de227-156">This field maps directly to the keywords condition.</span></span>  <span data-ttu-id="de227-157">您可以使用与值配对的可 *搜索字段名称* 中列出的字段来优化搜索。例如， *subject： "季度财务" 和日期>= 06/01/2016 和日期<= 07/01/2016*</span><span class="sxs-lookup"><span data-stu-id="de227-157">You can refine searches by using fields listed in the *searchable field name* paired with values; for example, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*</span></span> |

## <a name="relationships"></a><span data-ttu-id="de227-158">关系</span><span class="sxs-lookup"><span data-stu-id="de227-158">Relationships</span></span>

<span data-ttu-id="de227-159">无。</span><span class="sxs-lookup"><span data-stu-id="de227-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="de227-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de227-160">JSON representation</span></span>

<span data-ttu-id="de227-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de227-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSetQuery",
  "baseType": "",
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
