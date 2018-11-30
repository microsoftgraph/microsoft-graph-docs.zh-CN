---
title: timeSlot 资源类型
description: 时间段。
ms.openlocfilehash: 43ce20e006f2a6946877a4ffd2bf730d45d6d1c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009638"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="82b11-103">timeSlot 资源类型</span><span class="sxs-lookup"><span data-stu-id="82b11-103">timeSlot resource type</span></span>

<span data-ttu-id="82b11-104">时间段。</span><span class="sxs-lookup"><span data-stu-id="82b11-104">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="82b11-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82b11-105">JSON representation</span></span>

<span data-ttu-id="82b11-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82b11-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="82b11-107">属性</span><span class="sxs-lookup"><span data-stu-id="82b11-107">Properties</span></span>
| <span data-ttu-id="82b11-108">属性</span><span class="sxs-lookup"><span data-stu-id="82b11-108">Property</span></span>     | <span data-ttu-id="82b11-109">类型</span><span class="sxs-lookup"><span data-stu-id="82b11-109">Type</span></span>   |<span data-ttu-id="82b11-110">说明</span><span class="sxs-lookup"><span data-stu-id="82b11-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82b11-111">end</span><span class="sxs-lookup"><span data-stu-id="82b11-111">end</span></span>|[<span data-ttu-id="82b11-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="82b11-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="82b11-113">时间段的开始时间。</span><span class="sxs-lookup"><span data-stu-id="82b11-113">The time a period begins.</span></span>|
|<span data-ttu-id="82b11-114">start</span><span class="sxs-lookup"><span data-stu-id="82b11-114">start</span></span>|[<span data-ttu-id="82b11-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="82b11-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="82b11-116">时间段的结束时间。</span><span class="sxs-lookup"><span data-stu-id="82b11-116">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->