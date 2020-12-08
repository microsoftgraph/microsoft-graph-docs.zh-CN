---
title: reviewSet 资源类型
description: 表示为在诉讼、调查或管理法规请求中使用而收集的以电子方式存储的信息的静态集。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 411de013df02bcd71e851a694664ae010edaf4ab
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597260"
---
# <a name="reviewset-resource-type"></a><span data-ttu-id="94041-103">reviewSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="94041-103">reviewSet resource type</span></span>

<span data-ttu-id="94041-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94041-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94041-105">表示为在诉讼、调查或管理法规请求中使用而收集的以电子方式存储的信息的静态集。</span><span class="sxs-lookup"><span data-stu-id="94041-105">Represents static set of electronically stored information collected for use in a litigation, investigation, or regulatory request.</span></span>

## <a name="methods"></a><span data-ttu-id="94041-106">方法</span><span class="sxs-lookup"><span data-stu-id="94041-106">Methods</span></span>

| <span data-ttu-id="94041-107">方法</span><span class="sxs-lookup"><span data-stu-id="94041-107">Method</span></span>       | <span data-ttu-id="94041-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="94041-108">Return Type</span></span> | <span data-ttu-id="94041-109">Description</span><span class="sxs-lookup"><span data-stu-id="94041-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="94041-110">列出 reviewSet</span><span class="sxs-lookup"><span data-stu-id="94041-110">List reviewSet</span></span>](../api/reviewset-list.md) | <span data-ttu-id="94041-111">[reviewSet](reviewset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="94041-111">[reviewSet](reviewset.md) collection</span></span> | <span data-ttu-id="94041-112">获取审阅集的集合。</span><span class="sxs-lookup"><span data-stu-id="94041-112">Get a collection of review sets.</span></span> |
| [<span data-ttu-id="94041-113">获取 reviewSet</span><span class="sxs-lookup"><span data-stu-id="94041-113">Get reviewSet</span></span>](../api/reviewset-get.md) | [<span data-ttu-id="94041-114">reviewSet</span><span class="sxs-lookup"><span data-stu-id="94041-114">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="94041-115">读取 **reviewSet** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94041-115">Read the properties and relationships of a **reviewSet** object.</span></span> |
| [<span data-ttu-id="94041-116">创建 reviewSet</span><span class="sxs-lookup"><span data-stu-id="94041-116">Create reviewSet</span></span>](../api/reviewset-post.md) | [<span data-ttu-id="94041-117">reviewSet</span><span class="sxs-lookup"><span data-stu-id="94041-117">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="94041-118">创建新的审阅集。</span><span class="sxs-lookup"><span data-stu-id="94041-118">Create a new review set.</span></span> |
| [<span data-ttu-id="94041-119">列出查询</span><span class="sxs-lookup"><span data-stu-id="94041-119">List queries</span></span>](../api/reviewsetquery-list.md)|<span data-ttu-id="94041-120">[reviewSetQuery](../resources/reviewsetquery.md) 集合</span><span class="sxs-lookup"><span data-stu-id="94041-120">[reviewSetQuery](../resources/reviewsetquery.md) collection</span></span>|<span data-ttu-id="94041-121">从 "查询导航" 属性中获取 reviewSetQuery 资源。</span><span class="sxs-lookup"><span data-stu-id="94041-121">Get the reviewSetQuery resources from the queries navigation property.</span></span>|
| [<span data-ttu-id="94041-122">创建查询</span><span class="sxs-lookup"><span data-stu-id="94041-122">Create queries</span></span>](../api/reviewsetquery-post.md)|[<span data-ttu-id="94041-123">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="94041-123">reviewSetQuery</span></span>](../resources/reviewsetquery.md)|<span data-ttu-id="94041-124">创建新的 reviewSetQuery 对象。</span><span class="sxs-lookup"><span data-stu-id="94041-124">Create a new reviewSetQuery object.</span></span>|

## <a name="properties"></a><span data-ttu-id="94041-125">属性</span><span class="sxs-lookup"><span data-stu-id="94041-125">Properties</span></span>

| <span data-ttu-id="94041-126">属性</span><span class="sxs-lookup"><span data-stu-id="94041-126">Property</span></span>     | <span data-ttu-id="94041-127">类型</span><span class="sxs-lookup"><span data-stu-id="94041-127">Type</span></span>        | <span data-ttu-id="94041-128">说明</span><span class="sxs-lookup"><span data-stu-id="94041-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="94041-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="94041-129">createdBy</span></span>        | [<span data-ttu-id="94041-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="94041-130">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="94041-131">创建评审集的用户。</span><span class="sxs-lookup"><span data-stu-id="94041-131">The user who created the review set.</span></span> <span data-ttu-id="94041-132">只读。</span><span class="sxs-lookup"><span data-stu-id="94041-132">Read-only.</span></span> |
|<span data-ttu-id="94041-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94041-133">createdDateTime</span></span>  |<span data-ttu-id="94041-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94041-134">DateTimeOffset</span></span>| <span data-ttu-id="94041-135">创建评审集时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="94041-135">The datetime when the review set was created.</span></span> <span data-ttu-id="94041-136">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="94041-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="94041-137">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="94041-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="94041-138">只读。</span><span class="sxs-lookup"><span data-stu-id="94041-138">Read-only.</span></span> |
|<span data-ttu-id="94041-139">displayName</span><span class="sxs-lookup"><span data-stu-id="94041-139">displayName</span></span>      |<span data-ttu-id="94041-140">String</span><span class="sxs-lookup"><span data-stu-id="94041-140">String</span></span>| <span data-ttu-id="94041-141">审阅集名称。</span><span class="sxs-lookup"><span data-stu-id="94041-141">The review set name.</span></span> <span data-ttu-id="94041-142">名称是唯一的，最大限制为64个字符。</span><span class="sxs-lookup"><span data-stu-id="94041-142">Name is unique with a maximum limit of 64 characters.</span></span> |
|<span data-ttu-id="94041-143">id</span><span class="sxs-lookup"><span data-stu-id="94041-143">id</span></span>               |<span data-ttu-id="94041-144">String</span><span class="sxs-lookup"><span data-stu-id="94041-144">String</span></span>| <span data-ttu-id="94041-145">审阅集的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="94041-145">The review set unique identifier.</span></span> <span data-ttu-id="94041-146">只读。</span><span class="sxs-lookup"><span data-stu-id="94041-146">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="94041-147">关系</span><span class="sxs-lookup"><span data-stu-id="94041-147">Relationships</span></span>

| <span data-ttu-id="94041-148">关系</span><span class="sxs-lookup"><span data-stu-id="94041-148">Relationship</span></span> | <span data-ttu-id="94041-149">类型</span><span class="sxs-lookup"><span data-stu-id="94041-149">Type</span></span>        | <span data-ttu-id="94041-150">Description</span><span class="sxs-lookup"><span data-stu-id="94041-150">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="94041-151">审阅集查询</span><span class="sxs-lookup"><span data-stu-id="94041-151">Review set query</span></span> |<span data-ttu-id="94041-152">[reviewSetQuery](reviewsetquery.md) 集合</span><span class="sxs-lookup"><span data-stu-id="94041-152">[reviewSetQuery](reviewsetquery.md) collection</span></span>| <span data-ttu-id="94041-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="94041-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94041-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94041-155">JSON representation</span></span>

<span data-ttu-id="94041-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94041-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSet",
  "baseType": "",
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
