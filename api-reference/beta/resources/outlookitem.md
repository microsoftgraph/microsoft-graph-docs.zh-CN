---
title: outlookItem 资源类型
description: 下面是资源的 JSON 表示形式。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 59510469101b0b35865a945c8170025ad80ef3db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522093"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="11cfa-103">outlookItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="11cfa-103">outlookItem resource type</span></span>

<span data-ttu-id="11cfa-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="11cfa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="11cfa-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11cfa-105">JSON representation</span></span>

<span data-ttu-id="11cfa-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11cfa-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="11cfa-107">属性</span><span class="sxs-lookup"><span data-stu-id="11cfa-107">Properties</span></span>
| <span data-ttu-id="11cfa-108">属性</span><span class="sxs-lookup"><span data-stu-id="11cfa-108">Property</span></span>     | <span data-ttu-id="11cfa-109">类型</span><span class="sxs-lookup"><span data-stu-id="11cfa-109">Type</span></span>   |<span data-ttu-id="11cfa-110">说明</span><span class="sxs-lookup"><span data-stu-id="11cfa-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11cfa-111">categories</span><span class="sxs-lookup"><span data-stu-id="11cfa-111">categories</span></span>|<span data-ttu-id="11cfa-112">String 集合</span><span class="sxs-lookup"><span data-stu-id="11cfa-112">String collection</span></span>||
|<span data-ttu-id="11cfa-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="11cfa-113">changeKey</span></span>|<span data-ttu-id="11cfa-114">String</span><span class="sxs-lookup"><span data-stu-id="11cfa-114">String</span></span>||
|<span data-ttu-id="11cfa-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11cfa-115">createdDateTime</span></span>|<span data-ttu-id="11cfa-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11cfa-116">DateTimeOffset</span></span>|<span data-ttu-id="11cfa-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="11cfa-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="11cfa-119">id</span><span class="sxs-lookup"><span data-stu-id="11cfa-119">id</span></span>|<span data-ttu-id="11cfa-120">字符串</span><span class="sxs-lookup"><span data-stu-id="11cfa-120">String</span></span>| <span data-ttu-id="11cfa-121">只读。</span><span class="sxs-lookup"><span data-stu-id="11cfa-121">Read-only.</span></span>|
|<span data-ttu-id="11cfa-122">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11cfa-122">lastModifiedDateTime</span></span>|<span data-ttu-id="11cfa-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11cfa-123">DateTimeOffset</span></span>|<span data-ttu-id="11cfa-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="11cfa-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="11cfa-126">关系</span><span class="sxs-lookup"><span data-stu-id="11cfa-126">Relationships</span></span>
<span data-ttu-id="11cfa-127">无</span><span class="sxs-lookup"><span data-stu-id="11cfa-127">None</span></span>


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
