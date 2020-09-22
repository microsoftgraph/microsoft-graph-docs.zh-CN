---
title: reviewSet 资源类型
description: 表示为在诉讼、调查或管理法规请求中使用而收集的以电子方式存储的信息的静态集。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 76e63c5aece7f7254afa282469a1dc8ce664217f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026231"
---
# <a name="reviewset-resource-type"></a><span data-ttu-id="6d40c-103">reviewSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d40c-103">reviewSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d40c-104">表示为在诉讼、调查或管理法规请求中使用而收集的以电子方式存储的信息的静态集。</span><span class="sxs-lookup"><span data-stu-id="6d40c-104">Represents static set of electronically stored information collected for use in a litigation, investigation, or regulatory request.</span></span>

## <a name="methods"></a><span data-ttu-id="6d40c-105">方法</span><span class="sxs-lookup"><span data-stu-id="6d40c-105">Methods</span></span>

| <span data-ttu-id="6d40c-106">方法</span><span class="sxs-lookup"><span data-stu-id="6d40c-106">Method</span></span>       | <span data-ttu-id="6d40c-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="6d40c-107">Return Type</span></span> | <span data-ttu-id="6d40c-108">Description</span><span class="sxs-lookup"><span data-stu-id="6d40c-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6d40c-109">List</span><span class="sxs-lookup"><span data-stu-id="6d40c-109">List</span></span>](../api/reviewset-list.md) | <span data-ttu-id="6d40c-110">[reviewSet](reviewset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6d40c-110">[reviewSet](reviewset.md) collection</span></span> | <span data-ttu-id="6d40c-111">获取审阅集的集合。</span><span class="sxs-lookup"><span data-stu-id="6d40c-111">Get a collection of review sets.</span></span> |
| [<span data-ttu-id="6d40c-112">获取</span><span class="sxs-lookup"><span data-stu-id="6d40c-112">Get</span></span>](../api/reviewset-get.md) | [<span data-ttu-id="6d40c-113">reviewSet</span><span class="sxs-lookup"><span data-stu-id="6d40c-113">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="6d40c-114">读取 **reviewSet** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6d40c-114">Read the properties and relationships of a **reviewSet** object.</span></span> |
| [<span data-ttu-id="6d40c-115">创建</span><span class="sxs-lookup"><span data-stu-id="6d40c-115">Create</span></span>](../api/reviewset-post.md) | [<span data-ttu-id="6d40c-116">reviewSet</span><span class="sxs-lookup"><span data-stu-id="6d40c-116">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="6d40c-117">创建新的审阅集。</span><span class="sxs-lookup"><span data-stu-id="6d40c-117">Create a new review set.</span></span> |

## <a name="properties"></a><span data-ttu-id="6d40c-118">属性</span><span class="sxs-lookup"><span data-stu-id="6d40c-118">Properties</span></span>

| <span data-ttu-id="6d40c-119">属性</span><span class="sxs-lookup"><span data-stu-id="6d40c-119">Property</span></span>     | <span data-ttu-id="6d40c-120">类型</span><span class="sxs-lookup"><span data-stu-id="6d40c-120">Type</span></span>        | <span data-ttu-id="6d40c-121">说明</span><span class="sxs-lookup"><span data-stu-id="6d40c-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6d40c-122">createdBy</span><span class="sxs-lookup"><span data-stu-id="6d40c-122">createdBy</span></span>| [<span data-ttu-id="6d40c-123">identitySet</span><span class="sxs-lookup"><span data-stu-id="6d40c-123">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset) | <span data-ttu-id="6d40c-124">创建评审集的用户。</span><span class="sxs-lookup"><span data-stu-id="6d40c-124">The user who created the review set.</span></span> <span data-ttu-id="6d40c-125">只读。</span><span class="sxs-lookup"><span data-stu-id="6d40c-125">Read-only.</span></span> |
|<span data-ttu-id="6d40c-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d40c-126">createdDateTime</span></span>|<span data-ttu-id="6d40c-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d40c-127">DateTimeOffset</span></span>| <span data-ttu-id="6d40c-128">创建评审集时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="6d40c-128">The datetime when the review set was created.</span></span> <span data-ttu-id="6d40c-129">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="6d40c-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6d40c-130">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="6d40c-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="6d40c-131">只读。</span><span class="sxs-lookup"><span data-stu-id="6d40c-131">Read-only.</span></span> |
|<span data-ttu-id="6d40c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="6d40c-132">displayName</span></span>|<span data-ttu-id="6d40c-133">String</span><span class="sxs-lookup"><span data-stu-id="6d40c-133">String</span></span>| <span data-ttu-id="6d40c-134">审阅集名称。</span><span class="sxs-lookup"><span data-stu-id="6d40c-134">The review set name.</span></span> <span data-ttu-id="6d40c-135">名称是唯一的，最大限制为64个字符。</span><span class="sxs-lookup"><span data-stu-id="6d40c-135">Name is unique with a maximum limit of 64 characters.</span></span> |
|<span data-ttu-id="6d40c-136">id</span><span class="sxs-lookup"><span data-stu-id="6d40c-136">id</span></span>|<span data-ttu-id="6d40c-137">String</span><span class="sxs-lookup"><span data-stu-id="6d40c-137">String</span></span>| <span data-ttu-id="6d40c-138">审阅集的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6d40c-138">The review set unique identifier.</span></span> <span data-ttu-id="6d40c-139">只读。</span><span class="sxs-lookup"><span data-stu-id="6d40c-139">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6d40c-140">关系</span><span class="sxs-lookup"><span data-stu-id="6d40c-140">Relationships</span></span>

| <span data-ttu-id="6d40c-141">关系</span><span class="sxs-lookup"><span data-stu-id="6d40c-141">Relationship</span></span> | <span data-ttu-id="6d40c-142">类型</span><span class="sxs-lookup"><span data-stu-id="6d40c-142">Type</span></span>        | <span data-ttu-id="6d40c-143">说明</span><span class="sxs-lookup"><span data-stu-id="6d40c-143">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6d40c-144">审阅集查询</span><span class="sxs-lookup"><span data-stu-id="6d40c-144">Review set query</span></span> |<span data-ttu-id="6d40c-145">[reviewSetQuery](reviewsetquery.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6d40c-145">[reviewSetQuery](reviewsetquery.md) collection</span></span>| <span data-ttu-id="6d40c-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="6d40c-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d40c-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d40c-148">JSON representation</span></span>

<span data-ttu-id="6d40c-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d40c-149">The following is a JSON representation of the resource.</span></span>

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
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)"
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


