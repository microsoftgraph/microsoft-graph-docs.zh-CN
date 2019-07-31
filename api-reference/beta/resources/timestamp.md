---
title: 时间戳资源类型
description: 时间点的日期和时间信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: cda000674241ee57347d6809d04d7acd9d59ff0b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964278"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="e9485-103">时间戳资源类型</span><span class="sxs-lookup"><span data-stu-id="e9485-103">timeStamp resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9485-104">时间点的日期和时间信息。</span><span class="sxs-lookup"><span data-stu-id="e9485-104">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9485-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9485-105">JSON representation</span></span>

<span data-ttu-id="e9485-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9485-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a><span data-ttu-id="e9485-107">属性</span><span class="sxs-lookup"><span data-stu-id="e9485-107">Properties</span></span>
| <span data-ttu-id="e9485-108">属性</span><span class="sxs-lookup"><span data-stu-id="e9485-108">Property</span></span>     | <span data-ttu-id="e9485-109">类型</span><span class="sxs-lookup"><span data-stu-id="e9485-109">Type</span></span>   |<span data-ttu-id="e9485-110">说明</span><span class="sxs-lookup"><span data-stu-id="e9485-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9485-111">date</span><span class="sxs-lookup"><span data-stu-id="e9485-111">date</span></span>|<span data-ttu-id="e9485-112">Date</span><span class="sxs-lookup"><span data-stu-id="e9485-112">Date</span></span>|<span data-ttu-id="e9485-113">时间戳的日期部分。</span><span class="sxs-lookup"><span data-stu-id="e9485-113">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="e9485-114">time</span><span class="sxs-lookup"><span data-stu-id="e9485-114">time</span></span>|<span data-ttu-id="e9485-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="e9485-115">TimeOfDay</span></span>|<span data-ttu-id="e9485-116">时间戳的时间部分。</span><span class="sxs-lookup"><span data-stu-id="e9485-116">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="e9485-117">timeZone</span><span class="sxs-lookup"><span data-stu-id="e9485-117">timeZone</span></span>|<span data-ttu-id="e9485-118">字符串</span><span class="sxs-lookup"><span data-stu-id="e9485-118">String</span></span>|<span data-ttu-id="e9485-119">时间戳的时区部分, 是世界上的 24 longitudinal 区域之一。</span><span class="sxs-lookup"><span data-stu-id="e9485-119">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
