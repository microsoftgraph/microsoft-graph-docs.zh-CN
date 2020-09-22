---
title: timeSlot 资源类型
description: 时间段。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 874b587db2bb9e2234fcacca9b3e3b0cf5c2f89b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090751"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="811b0-103">timeSlot 资源类型</span><span class="sxs-lookup"><span data-stu-id="811b0-103">timeSlot resource type</span></span>

<span data-ttu-id="811b0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="811b0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="811b0-105">表示会议的时间段。</span><span class="sxs-lookup"><span data-stu-id="811b0-105">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="811b0-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="811b0-106">JSON representation</span></span>

<span data-ttu-id="811b0-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="811b0-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="811b0-108">属性</span><span class="sxs-lookup"><span data-stu-id="811b0-108">Properties</span></span>
| <span data-ttu-id="811b0-109">属性</span><span class="sxs-lookup"><span data-stu-id="811b0-109">Property</span></span>     | <span data-ttu-id="811b0-110">类型</span><span class="sxs-lookup"><span data-stu-id="811b0-110">Type</span></span>   |<span data-ttu-id="811b0-111">说明</span><span class="sxs-lookup"><span data-stu-id="811b0-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="811b0-112">end</span><span class="sxs-lookup"><span data-stu-id="811b0-112">end</span></span>|[<span data-ttu-id="811b0-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="811b0-113">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="811b0-114">时间段开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="811b0-114">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="811b0-115">start</span><span class="sxs-lookup"><span data-stu-id="811b0-115">start</span></span>|[<span data-ttu-id="811b0-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="811b0-116">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="811b0-117">时间段结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="811b0-117">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

