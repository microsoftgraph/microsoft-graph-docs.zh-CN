---
title: outlookItem 资源类型
description: 下面是资源的 JSON 表示形式。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 37a9d548e0eac3d07a66ca4b28c243c076a743bb
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721535"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="51d73-103">outlookItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="51d73-103">outlookItem resource type</span></span>

<span data-ttu-id="51d73-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51d73-104">Namespace: microsoft.graph</span></span>



## <a name="json-representation"></a><span data-ttu-id="51d73-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51d73-105">JSON representation</span></span>

<span data-ttu-id="51d73-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51d73-106">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookItem"
}-->

```json
{
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="51d73-107">属性</span><span class="sxs-lookup"><span data-stu-id="51d73-107">Properties</span></span>
| <span data-ttu-id="51d73-108">属性</span><span class="sxs-lookup"><span data-stu-id="51d73-108">Property</span></span>     | <span data-ttu-id="51d73-109">类型</span><span class="sxs-lookup"><span data-stu-id="51d73-109">Type</span></span>   |<span data-ttu-id="51d73-110">说明</span><span class="sxs-lookup"><span data-stu-id="51d73-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51d73-111">categories</span><span class="sxs-lookup"><span data-stu-id="51d73-111">categories</span></span>|<span data-ttu-id="51d73-112">String collection</span><span class="sxs-lookup"><span data-stu-id="51d73-112">String collection</span></span>|<span data-ttu-id="51d73-113">与项目关联的类别</span><span class="sxs-lookup"><span data-stu-id="51d73-113">The categories associated with the item</span></span>|
|<span data-ttu-id="51d73-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="51d73-114">changeKey</span></span>|<span data-ttu-id="51d73-115">字符串</span><span class="sxs-lookup"><span data-stu-id="51d73-115">String</span></span>|<span data-ttu-id="51d73-116">标识项目的版本。</span><span class="sxs-lookup"><span data-stu-id="51d73-116">Identifies the version of the item.</span></span> <span data-ttu-id="51d73-117">每次项目更改时，changeKey 也更改。</span><span class="sxs-lookup"><span data-stu-id="51d73-117">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="51d73-118">这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="51d73-118">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="51d73-119">只读。</span><span class="sxs-lookup"><span data-stu-id="51d73-119">Read-only.</span></span>|
|<span data-ttu-id="51d73-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51d73-120">createdDateTime</span></span>|<span data-ttu-id="51d73-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51d73-121">DateTimeOffset</span></span>|<span data-ttu-id="51d73-122">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="51d73-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="51d73-123">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="51d73-123">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="51d73-124">id</span><span class="sxs-lookup"><span data-stu-id="51d73-124">id</span></span>|<span data-ttu-id="51d73-125">字符串</span><span class="sxs-lookup"><span data-stu-id="51d73-125">String</span></span>| <span data-ttu-id="51d73-126">只读。</span><span class="sxs-lookup"><span data-stu-id="51d73-126">Read-only.</span></span>|
|<span data-ttu-id="51d73-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51d73-127">lastModifiedDateTime</span></span>|<span data-ttu-id="51d73-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51d73-128">DateTimeOffset</span></span>|<span data-ttu-id="51d73-129">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="51d73-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="51d73-130">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="51d73-130">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="51d73-131">关系</span><span class="sxs-lookup"><span data-stu-id="51d73-131">Relationships</span></span>
<span data-ttu-id="51d73-132">无</span><span class="sxs-lookup"><span data-stu-id="51d73-132">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

