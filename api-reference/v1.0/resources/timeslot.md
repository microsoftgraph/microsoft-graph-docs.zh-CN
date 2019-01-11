---
title: timeSlot 资源类型
description: 时间段。
localization_priority: Normal
ms.openlocfilehash: e01b8d0f34a21eb18bc92e8bcc4e1b8365541d5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860562"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="6e260-103">timeSlot 资源类型</span><span class="sxs-lookup"><span data-stu-id="6e260-103">timeSlot resource type</span></span>

<span data-ttu-id="6e260-104">时间段。</span><span class="sxs-lookup"><span data-stu-id="6e260-104">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e260-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6e260-105">JSON representation</span></span>

<span data-ttu-id="6e260-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e260-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeSlot"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a><span data-ttu-id="6e260-107">属性</span><span class="sxs-lookup"><span data-stu-id="6e260-107">Properties</span></span>
| <span data-ttu-id="6e260-108">属性</span><span class="sxs-lookup"><span data-stu-id="6e260-108">Property</span></span>     | <span data-ttu-id="6e260-109">类型</span><span class="sxs-lookup"><span data-stu-id="6e260-109">Type</span></span>   |<span data-ttu-id="6e260-110">说明</span><span class="sxs-lookup"><span data-stu-id="6e260-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e260-111">end</span><span class="sxs-lookup"><span data-stu-id="6e260-111">end</span></span>|[<span data-ttu-id="6e260-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6e260-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6e260-113">时间段的开始时间。</span><span class="sxs-lookup"><span data-stu-id="6e260-113">The time a period begins.</span></span>|
|<span data-ttu-id="6e260-114">start</span><span class="sxs-lookup"><span data-stu-id="6e260-114">start</span></span>|[<span data-ttu-id="6e260-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6e260-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6e260-116">时间段的结束时间。</span><span class="sxs-lookup"><span data-stu-id="6e260-116">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
