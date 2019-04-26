---
title: 时间戳资源类型
description: 时间点的日期和时间信息。
localization_priority: Normal
ms.openlocfilehash: 5f96ad5c557bda93ef74787d9d909fce112cfb15
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341951"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="3ab81-103">时间戳资源类型</span><span class="sxs-lookup"><span data-stu-id="3ab81-103">timeStamp resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ab81-104">时间点的日期和时间信息。</span><span class="sxs-lookup"><span data-stu-id="3ab81-104">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ab81-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ab81-105">JSON representation</span></span>

<span data-ttu-id="3ab81-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ab81-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="3ab81-107">属性</span><span class="sxs-lookup"><span data-stu-id="3ab81-107">Properties</span></span>
| <span data-ttu-id="3ab81-108">属性</span><span class="sxs-lookup"><span data-stu-id="3ab81-108">Property</span></span>     | <span data-ttu-id="3ab81-109">类型</span><span class="sxs-lookup"><span data-stu-id="3ab81-109">Type</span></span>   |<span data-ttu-id="3ab81-110">说明</span><span class="sxs-lookup"><span data-stu-id="3ab81-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ab81-111">date</span><span class="sxs-lookup"><span data-stu-id="3ab81-111">date</span></span>|<span data-ttu-id="3ab81-112">Date</span><span class="sxs-lookup"><span data-stu-id="3ab81-112">Date</span></span>|<span data-ttu-id="3ab81-113">时间戳的日期部分。</span><span class="sxs-lookup"><span data-stu-id="3ab81-113">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="3ab81-114">time</span><span class="sxs-lookup"><span data-stu-id="3ab81-114">time</span></span>|<span data-ttu-id="3ab81-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="3ab81-115">TimeOfDay</span></span>|<span data-ttu-id="3ab81-116">时间戳的时间部分。</span><span class="sxs-lookup"><span data-stu-id="3ab81-116">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="3ab81-117">timeZone</span><span class="sxs-lookup"><span data-stu-id="3ab81-117">timeZone</span></span>|<span data-ttu-id="3ab81-118">字符串</span><span class="sxs-lookup"><span data-stu-id="3ab81-118">String</span></span>|<span data-ttu-id="3ab81-119">时间戳的时区部分, 是世界上的 24 longitudinal 区域之一。</span><span class="sxs-lookup"><span data-stu-id="3ab81-119">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

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
