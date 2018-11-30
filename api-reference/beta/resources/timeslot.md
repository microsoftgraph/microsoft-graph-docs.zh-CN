---
title: timeSlot 资源类型
description: 时间段。
ms.openlocfilehash: c1df6ea458bf6742dc20149e62d9760a8a6510e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048137"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="2702b-103">timeSlot 资源类型</span><span class="sxs-lookup"><span data-stu-id="2702b-103">timeSlot resource type</span></span>

> <span data-ttu-id="2702b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2702b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2702b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2702b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2702b-106">时间段。</span><span class="sxs-lookup"><span data-stu-id="2702b-106">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2702b-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2702b-107">JSON representation</span></span>

<span data-ttu-id="2702b-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2702b-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="2702b-109">属性</span><span class="sxs-lookup"><span data-stu-id="2702b-109">Properties</span></span>
| <span data-ttu-id="2702b-110">属性</span><span class="sxs-lookup"><span data-stu-id="2702b-110">Property</span></span>     | <span data-ttu-id="2702b-111">类型</span><span class="sxs-lookup"><span data-stu-id="2702b-111">Type</span></span>   |<span data-ttu-id="2702b-112">说明</span><span class="sxs-lookup"><span data-stu-id="2702b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2702b-113">end</span><span class="sxs-lookup"><span data-stu-id="2702b-113">end</span></span>|[<span data-ttu-id="2702b-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2702b-114">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2702b-115">时间段的开始时间。</span><span class="sxs-lookup"><span data-stu-id="2702b-115">The time a period begins.</span></span>|
|<span data-ttu-id="2702b-116">start</span><span class="sxs-lookup"><span data-stu-id="2702b-116">start</span></span>|[<span data-ttu-id="2702b-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2702b-117">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2702b-118">时间段的结束时间。</span><span class="sxs-lookup"><span data-stu-id="2702b-118">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->