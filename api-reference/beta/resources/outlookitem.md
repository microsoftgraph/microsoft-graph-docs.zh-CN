---
title: outlookItem 资源类型
description: 下面是资源的 JSON 表示形式。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9ed43ccabfbd2b5389525ebec02ecd04edb475b3
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721815"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="d40c0-103">outlookItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="d40c0-103">outlookItem resource type</span></span>

<span data-ttu-id="d40c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d40c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="d40c0-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d40c0-105">JSON representation</span></span>

<span data-ttu-id="d40c0-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d40c0-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
## <a name="properties"></a><span data-ttu-id="d40c0-107">属性</span><span class="sxs-lookup"><span data-stu-id="d40c0-107">Properties</span></span>
| <span data-ttu-id="d40c0-108">属性</span><span class="sxs-lookup"><span data-stu-id="d40c0-108">Property</span></span>     | <span data-ttu-id="d40c0-109">类型</span><span class="sxs-lookup"><span data-stu-id="d40c0-109">Type</span></span>   |<span data-ttu-id="d40c0-110">说明</span><span class="sxs-lookup"><span data-stu-id="d40c0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d40c0-111">categories</span><span class="sxs-lookup"><span data-stu-id="d40c0-111">categories</span></span>|<span data-ttu-id="d40c0-112">String 集合</span><span class="sxs-lookup"><span data-stu-id="d40c0-112">String collection</span></span>||
|<span data-ttu-id="d40c0-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="d40c0-113">changeKey</span></span>|<span data-ttu-id="d40c0-114">String</span><span class="sxs-lookup"><span data-stu-id="d40c0-114">String</span></span>||
|<span data-ttu-id="d40c0-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d40c0-115">createdDateTime</span></span>|<span data-ttu-id="d40c0-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d40c0-116">DateTimeOffset</span></span>|<span data-ttu-id="d40c0-117">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="d40c0-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d40c0-118">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="d40c0-118">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="d40c0-119">id</span><span class="sxs-lookup"><span data-stu-id="d40c0-119">id</span></span>|<span data-ttu-id="d40c0-120">String</span><span class="sxs-lookup"><span data-stu-id="d40c0-120">String</span></span>| <span data-ttu-id="d40c0-121">只读。</span><span class="sxs-lookup"><span data-stu-id="d40c0-121">Read-only.</span></span>|
|<span data-ttu-id="d40c0-122">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d40c0-122">lastModifiedDateTime</span></span>|<span data-ttu-id="d40c0-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d40c0-123">DateTimeOffset</span></span>|<span data-ttu-id="d40c0-124">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="d40c0-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d40c0-125">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="d40c0-125">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="d40c0-126">关系</span><span class="sxs-lookup"><span data-stu-id="d40c0-126">Relationships</span></span>
<span data-ttu-id="d40c0-127">无</span><span class="sxs-lookup"><span data-stu-id="d40c0-127">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


