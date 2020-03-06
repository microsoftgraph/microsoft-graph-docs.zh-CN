---
title: outlookItem 资源类型
description: 下面是资源的 JSON 表示形式。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: aa5e4af03171029e8557e38d3a75062161435318
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534106"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="a75fb-103">outlookItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="a75fb-103">outlookItem resource type</span></span>

<span data-ttu-id="a75fb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a75fb-104">Namespace: microsoft.graph</span></span>



## <a name="json-representation"></a><span data-ttu-id="a75fb-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a75fb-105">JSON representation</span></span>

<span data-ttu-id="a75fb-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a75fb-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="a75fb-107">属性</span><span class="sxs-lookup"><span data-stu-id="a75fb-107">Properties</span></span>
| <span data-ttu-id="a75fb-108">属性</span><span class="sxs-lookup"><span data-stu-id="a75fb-108">Property</span></span>     | <span data-ttu-id="a75fb-109">类型</span><span class="sxs-lookup"><span data-stu-id="a75fb-109">Type</span></span>   |<span data-ttu-id="a75fb-110">说明</span><span class="sxs-lookup"><span data-stu-id="a75fb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a75fb-111">categories</span><span class="sxs-lookup"><span data-stu-id="a75fb-111">categories</span></span>|<span data-ttu-id="a75fb-112">String collection</span><span class="sxs-lookup"><span data-stu-id="a75fb-112">String collection</span></span>|<span data-ttu-id="a75fb-113">与项目关联的类别</span><span class="sxs-lookup"><span data-stu-id="a75fb-113">The categories associated with the item</span></span>|
|<span data-ttu-id="a75fb-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="a75fb-114">changeKey</span></span>|<span data-ttu-id="a75fb-115">String</span><span class="sxs-lookup"><span data-stu-id="a75fb-115">String</span></span>|<span data-ttu-id="a75fb-116">标识项目的版本。</span><span class="sxs-lookup"><span data-stu-id="a75fb-116">Identifies the version of the item.</span></span> <span data-ttu-id="a75fb-117">每次更改项目时，changeKey 也会更改。</span><span class="sxs-lookup"><span data-stu-id="a75fb-117">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="a75fb-118">这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="a75fb-118">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="a75fb-119">只读。</span><span class="sxs-lookup"><span data-stu-id="a75fb-119">Read-only.</span></span>|
|<span data-ttu-id="a75fb-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a75fb-120">createdDateTime</span></span>|<span data-ttu-id="a75fb-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a75fb-121">DateTimeOffset</span></span>|<span data-ttu-id="a75fb-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a75fb-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a75fb-124">id</span><span class="sxs-lookup"><span data-stu-id="a75fb-124">id</span></span>|<span data-ttu-id="a75fb-125">字符串</span><span class="sxs-lookup"><span data-stu-id="a75fb-125">String</span></span>| <span data-ttu-id="a75fb-126">只读。</span><span class="sxs-lookup"><span data-stu-id="a75fb-126">Read-only.</span></span>|
|<span data-ttu-id="a75fb-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a75fb-127">lastModifiedDateTime</span></span>|<span data-ttu-id="a75fb-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a75fb-128">DateTimeOffset</span></span>|<span data-ttu-id="a75fb-p103">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a75fb-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="a75fb-131">关系</span><span class="sxs-lookup"><span data-stu-id="a75fb-131">Relationships</span></span>
<span data-ttu-id="a75fb-132">无</span><span class="sxs-lookup"><span data-stu-id="a75fb-132">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
