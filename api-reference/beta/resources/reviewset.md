---
title: reviewSet 资源类型
description: 表示收集用于诉讼、调查或监管请求的静态电子存储信息集。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: b6234fafbf0d6e36d5dcbb4143956447e26d3a0f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153499"
---
# <a name="reviewset-resource-type"></a><span data-ttu-id="844d0-103">reviewSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="844d0-103">reviewSet resource type</span></span>

<span data-ttu-id="844d0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="844d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="844d0-105">表示收集用于诉讼、调查或监管请求的静态存储信息集。</span><span class="sxs-lookup"><span data-stu-id="844d0-105">Represents static set of electronically stored information collected for use in a litigation, investigation, or regulatory request.</span></span>

## <a name="methods"></a><span data-ttu-id="844d0-106">方法</span><span class="sxs-lookup"><span data-stu-id="844d0-106">Methods</span></span>

| <span data-ttu-id="844d0-107">方法</span><span class="sxs-lookup"><span data-stu-id="844d0-107">Method</span></span>       | <span data-ttu-id="844d0-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="844d0-108">Return Type</span></span> | <span data-ttu-id="844d0-109">说明</span><span class="sxs-lookup"><span data-stu-id="844d0-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="844d0-110">列出 reviewSet</span><span class="sxs-lookup"><span data-stu-id="844d0-110">List reviewSet</span></span>](../api/reviewset-list.md) | <span data-ttu-id="844d0-111">[reviewSet](reviewset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="844d0-111">[reviewSet](reviewset.md) collection</span></span> | <span data-ttu-id="844d0-112">获取审阅集的集合。</span><span class="sxs-lookup"><span data-stu-id="844d0-112">Get a collection of review sets.</span></span> |
| [<span data-ttu-id="844d0-113">获取 reviewSet</span><span class="sxs-lookup"><span data-stu-id="844d0-113">Get reviewSet</span></span>](../api/reviewset-get.md) | [<span data-ttu-id="844d0-114">reviewSet</span><span class="sxs-lookup"><span data-stu-id="844d0-114">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="844d0-115">读取 **reviewSet 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="844d0-115">Read the properties and relationships of a **reviewSet** object.</span></span> |
| [<span data-ttu-id="844d0-116">创建 reviewSet</span><span class="sxs-lookup"><span data-stu-id="844d0-116">Create reviewSet</span></span>](../api/reviewset-post.md) | [<span data-ttu-id="844d0-117">reviewSet</span><span class="sxs-lookup"><span data-stu-id="844d0-117">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="844d0-118">创建新的审阅集。</span><span class="sxs-lookup"><span data-stu-id="844d0-118">Create a new review set.</span></span> |
| [<span data-ttu-id="844d0-119">列出查询</span><span class="sxs-lookup"><span data-stu-id="844d0-119">List queries</span></span>](../api/reviewsetquery-list.md)|<span data-ttu-id="844d0-120">[reviewSetQuery](../resources/reviewsetquery.md) 集合</span><span class="sxs-lookup"><span data-stu-id="844d0-120">[reviewSetQuery](../resources/reviewsetquery.md) collection</span></span>|<span data-ttu-id="844d0-121">从查询导航属性获取 reviewSetQuery 资源。</span><span class="sxs-lookup"><span data-stu-id="844d0-121">Get the reviewSetQuery resources from the queries navigation property.</span></span>|
| [<span data-ttu-id="844d0-122">创建查询</span><span class="sxs-lookup"><span data-stu-id="844d0-122">Create queries</span></span>](../api/reviewsetquery-post.md)|[<span data-ttu-id="844d0-123">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="844d0-123">reviewSetQuery</span></span>](../resources/reviewsetquery.md)|<span data-ttu-id="844d0-124">创建新的 reviewSetQuery 对象。</span><span class="sxs-lookup"><span data-stu-id="844d0-124">Create a new reviewSetQuery object.</span></span>|

## <a name="properties"></a><span data-ttu-id="844d0-125">属性</span><span class="sxs-lookup"><span data-stu-id="844d0-125">Properties</span></span>

| <span data-ttu-id="844d0-126">属性</span><span class="sxs-lookup"><span data-stu-id="844d0-126">Property</span></span>     | <span data-ttu-id="844d0-127">类型</span><span class="sxs-lookup"><span data-stu-id="844d0-127">Type</span></span>        | <span data-ttu-id="844d0-128">说明</span><span class="sxs-lookup"><span data-stu-id="844d0-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="844d0-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="844d0-129">createdBy</span></span>        | [<span data-ttu-id="844d0-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="844d0-130">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="844d0-131">创建审阅集的用户。</span><span class="sxs-lookup"><span data-stu-id="844d0-131">The user who created the review set.</span></span> <span data-ttu-id="844d0-132">只读。</span><span class="sxs-lookup"><span data-stu-id="844d0-132">Read-only.</span></span> |
|<span data-ttu-id="844d0-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="844d0-133">createdDateTime</span></span>  |<span data-ttu-id="844d0-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="844d0-134">DateTimeOffset</span></span>| <span data-ttu-id="844d0-135">创建审阅集的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="844d0-135">The datetime when the review set was created.</span></span> <span data-ttu-id="844d0-136">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="844d0-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="844d0-137">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="844d0-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="844d0-138">只读。</span><span class="sxs-lookup"><span data-stu-id="844d0-138">Read-only.</span></span> |
|<span data-ttu-id="844d0-139">displayName</span><span class="sxs-lookup"><span data-stu-id="844d0-139">displayName</span></span>      |<span data-ttu-id="844d0-140">String</span><span class="sxs-lookup"><span data-stu-id="844d0-140">String</span></span>| <span data-ttu-id="844d0-141">审阅集名称。</span><span class="sxs-lookup"><span data-stu-id="844d0-141">The review set name.</span></span> <span data-ttu-id="844d0-142">名称是唯一的，最大限制为 64 个字符。</span><span class="sxs-lookup"><span data-stu-id="844d0-142">Name is unique with a maximum limit of 64 characters.</span></span> |
|<span data-ttu-id="844d0-143">id</span><span class="sxs-lookup"><span data-stu-id="844d0-143">id</span></span>               |<span data-ttu-id="844d0-144">String</span><span class="sxs-lookup"><span data-stu-id="844d0-144">String</span></span>| <span data-ttu-id="844d0-145">审阅集唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="844d0-145">The review set unique identifier.</span></span> <span data-ttu-id="844d0-146">只读。</span><span class="sxs-lookup"><span data-stu-id="844d0-146">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="844d0-147">关系</span><span class="sxs-lookup"><span data-stu-id="844d0-147">Relationships</span></span>

| <span data-ttu-id="844d0-148">关系</span><span class="sxs-lookup"><span data-stu-id="844d0-148">Relationship</span></span> | <span data-ttu-id="844d0-149">类型</span><span class="sxs-lookup"><span data-stu-id="844d0-149">Type</span></span>        | <span data-ttu-id="844d0-150">说明</span><span class="sxs-lookup"><span data-stu-id="844d0-150">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="844d0-151">审阅集查询</span><span class="sxs-lookup"><span data-stu-id="844d0-151">Review set query</span></span> |<span data-ttu-id="844d0-152">[reviewSetQuery](reviewsetquery.md) 集合</span><span class="sxs-lookup"><span data-stu-id="844d0-152">[reviewSetQuery](reviewsetquery.md) collection</span></span>| <span data-ttu-id="844d0-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="844d0-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="844d0-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="844d0-155">JSON representation</span></span>

<span data-ttu-id="844d0-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="844d0-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSet",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.reviewSet",
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
