---
title: timeSlot 资源类型
description: 时间段。
localization_priority: Normal
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0631f618e644d9502d670ac988253f491fd2eeb6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075425"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="06dd2-103">timeSlot 资源类型</span><span class="sxs-lookup"><span data-stu-id="06dd2-103">timeSlot resource type</span></span>

<span data-ttu-id="06dd2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06dd2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06dd2-105">表示会议的时间段。</span><span class="sxs-lookup"><span data-stu-id="06dd2-105">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="06dd2-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06dd2-106">JSON representation</span></span>

<span data-ttu-id="06dd2-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06dd2-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="06dd2-108">属性</span><span class="sxs-lookup"><span data-stu-id="06dd2-108">Properties</span></span>
| <span data-ttu-id="06dd2-109">属性</span><span class="sxs-lookup"><span data-stu-id="06dd2-109">Property</span></span>     | <span data-ttu-id="06dd2-110">类型</span><span class="sxs-lookup"><span data-stu-id="06dd2-110">Type</span></span>   |<span data-ttu-id="06dd2-111">说明</span><span class="sxs-lookup"><span data-stu-id="06dd2-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06dd2-112">end</span><span class="sxs-lookup"><span data-stu-id="06dd2-112">end</span></span>|[<span data-ttu-id="06dd2-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="06dd2-113">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="06dd2-114">时间段开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="06dd2-114">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="06dd2-115">start</span><span class="sxs-lookup"><span data-stu-id="06dd2-115">start</span></span>|[<span data-ttu-id="06dd2-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="06dd2-116">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="06dd2-117">时间段结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="06dd2-117">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


