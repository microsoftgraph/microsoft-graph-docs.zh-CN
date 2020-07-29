---
title: reviewSetQuery 资源类型
description: 审阅集查询用于查询和精选电子数据展示 reviewSet 中存储的数据
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 2030d2f3403af2967100cbbc7de2571b8493895d
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510157"
---
# <a name="reviewsetquery-resource-type"></a><span data-ttu-id="c845f-103">reviewSetQuery 资源类型</span><span class="sxs-lookup"><span data-stu-id="c845f-103">reviewSetQuery resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c845f-104">审查集查询用于查询和挑选电子数据展示[reviewSet](reviewset.md)中存储的数据。</span><span class="sxs-lookup"><span data-stu-id="c845f-104">Review set queries are used to query and cull data stored in an eDiscovery [reviewSet](reviewset.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c845f-105">方法</span><span class="sxs-lookup"><span data-stu-id="c845f-105">Methods</span></span>

| <span data-ttu-id="c845f-106">方法</span><span class="sxs-lookup"><span data-stu-id="c845f-106">Method</span></span>       | <span data-ttu-id="c845f-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="c845f-107">Return Type</span></span> | <span data-ttu-id="c845f-108">说明</span><span class="sxs-lookup"><span data-stu-id="c845f-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c845f-109">List</span><span class="sxs-lookup"><span data-stu-id="c845f-109">List</span></span>](../api/reviewsetquery-list.md) | <span data-ttu-id="c845f-110">[reviewSetQuery](reviewsetquery.md)集合</span><span class="sxs-lookup"><span data-stu-id="c845f-110">[reviewSetQuery](reviewsetquery.md) collection</span></span> | <span data-ttu-id="c845f-111">在审阅集中列出审阅集查询。</span><span class="sxs-lookup"><span data-stu-id="c845f-111">List the review set queries in a review set.</span></span> |
| [<span data-ttu-id="c845f-112">创建</span><span class="sxs-lookup"><span data-stu-id="c845f-112">Create</span></span>](../api/reviewsetquery-post.md) | [<span data-ttu-id="c845f-113">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="c845f-113">reviewSetQuery</span></span>](reviewsetquery.md) | <span data-ttu-id="c845f-114">创建新的审阅集查询。</span><span class="sxs-lookup"><span data-stu-id="c845f-114">Create a new review set query.</span></span> |
| [<span data-ttu-id="c845f-115">获取</span><span class="sxs-lookup"><span data-stu-id="c845f-115">Get</span></span>](../api/reviewsetquery-get.md) | [<span data-ttu-id="c845f-116">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="c845f-116">reviewSetQuery</span></span>](reviewsetquery.md) | <span data-ttu-id="c845f-117">读取**reviewSetQuery**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c845f-117">Read the properties and relationships of a **reviewSetQuery** object.</span></span> |
| [<span data-ttu-id="c845f-118">更新</span><span class="sxs-lookup"><span data-stu-id="c845f-118">Update</span></span>](../api/reviewsetquery-update.md) | <span data-ttu-id="c845f-119">无</span><span class="sxs-lookup"><span data-stu-id="c845f-119">None</span></span> | <span data-ttu-id="c845f-120">更新审阅集查询。</span><span class="sxs-lookup"><span data-stu-id="c845f-120">Update a review set query.</span></span> |
| [<span data-ttu-id="c845f-121">删除</span><span class="sxs-lookup"><span data-stu-id="c845f-121">Delete</span></span>](../api/reviewsetquery-delete.md) | <span data-ttu-id="c845f-122">无</span><span class="sxs-lookup"><span data-stu-id="c845f-122">None</span></span> | <span data-ttu-id="c845f-123">删除审阅集查询。</span><span class="sxs-lookup"><span data-stu-id="c845f-123">Delete review set query.</span></span> |

## <a name="properties"></a><span data-ttu-id="c845f-124">属性</span><span class="sxs-lookup"><span data-stu-id="c845f-124">Properties</span></span>

| <span data-ttu-id="c845f-125">属性</span><span class="sxs-lookup"><span data-stu-id="c845f-125">Property</span></span>     | <span data-ttu-id="c845f-126">类型</span><span class="sxs-lookup"><span data-stu-id="c845f-126">Type</span></span>        | <span data-ttu-id="c845f-127">说明</span><span class="sxs-lookup"><span data-stu-id="c845f-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c845f-128">createdBy</span><span class="sxs-lookup"><span data-stu-id="c845f-128">createdBy</span></span> | [<span data-ttu-id="c845f-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="c845f-129">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset) | <span data-ttu-id="c845f-130">创建查询的用户。</span><span class="sxs-lookup"><span data-stu-id="c845f-130">The user who created the query.</span></span> |
| <span data-ttu-id="c845f-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c845f-131">createdDateTime</span></span> |<span data-ttu-id="c845f-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c845f-132">DateTimeOffset</span></span>| <span data-ttu-id="c845f-133">创建查询的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="c845f-133">The time and date when the query was created.</span></span> <span data-ttu-id="c845f-134">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="c845f-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c845f-135">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c845f-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="c845f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c845f-136">displayName</span></span> | <span data-ttu-id="c845f-137">String</span><span class="sxs-lookup"><span data-stu-id="c845f-137">String</span></span> | <span data-ttu-id="c845f-138">查询的名称</span><span class="sxs-lookup"><span data-stu-id="c845f-138">The name of the query</span></span>|
| <span data-ttu-id="c845f-139">id</span><span class="sxs-lookup"><span data-stu-id="c845f-139">id</span></span> |<span data-ttu-id="c845f-140">字符串</span><span class="sxs-lookup"><span data-stu-id="c845f-140">String</span></span>| <span data-ttu-id="c845f-141">查询的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c845f-141">The unique identifier of the query.</span></span> <span data-ttu-id="c845f-142">只读。</span><span class="sxs-lookup"><span data-stu-id="c845f-142">Read-only.</span></span>|
| <span data-ttu-id="c845f-143">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c845f-143">lastModifiedBy</span></span> | [<span data-ttu-id="c845f-144">identitySet</span><span class="sxs-lookup"><span data-stu-id="c845f-144">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset) | <span data-ttu-id="c845f-145">上次修改查询的用户。</span><span class="sxs-lookup"><span data-stu-id="c845f-145">The user who last modified the query.</span></span> |
| <span data-ttu-id="c845f-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c845f-146">lastModifiedDateTime</span></span> |<span data-ttu-id="c845f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c845f-147">DateTimeOffset</span></span> | <span data-ttu-id="c845f-148">上次修改查询的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c845f-148">The date and time the query was last modified.</span></span> <span data-ttu-id="c845f-149">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="c845f-149">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c845f-150">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c845f-150">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="c845f-151">查询</span><span class="sxs-lookup"><span data-stu-id="c845f-151">query</span></span> | <span data-ttu-id="c845f-152">字符串</span><span class="sxs-lookup"><span data-stu-id="c845f-152">String</span></span> | <span data-ttu-id="c845f-153">KQL （关键字查询语言）查询中的查询字符串。</span><span class="sxs-lookup"><span data-stu-id="c845f-153">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="c845f-154">https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery有关详细信息，请参阅。</span><span class="sxs-lookup"><span data-stu-id="c845f-154">Please refer to https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery for more details.</span></span>  <span data-ttu-id="c845f-155">此字段直接映射到关键字条件。</span><span class="sxs-lookup"><span data-stu-id="c845f-155">This field maps directly to the keywords condition.</span></span>  <span data-ttu-id="c845f-156">您可以使用与值配对的可*搜索字段名称*中列出的字段来优化搜索，例如*Subject： "季度财务" 和日期>= 06/01/2016 和日期<= 07/01/2016*</span><span class="sxs-lookup"><span data-stu-id="c845f-156">You can refine searches by using fields listed in the *searchable field name* paired with values, e.g. *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*</span></span> |

## <a name="relationships"></a><span data-ttu-id="c845f-157">关系</span><span class="sxs-lookup"><span data-stu-id="c845f-157">Relationships</span></span>

<span data-ttu-id="c845f-158">无。</span><span class="sxs-lookup"><span data-stu-id="c845f-158">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c845f-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c845f-159">JSON representation</span></span>

<span data-ttu-id="c845f-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c845f-160">The following is a JSON representation of the resource.</span></span>

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
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "lastModifiedBy": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "query": "String"
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
