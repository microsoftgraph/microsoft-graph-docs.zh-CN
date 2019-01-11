---
title: 时间戳资源类型
description: 日期和时间点时间信息。
localization_priority: Normal
ms.openlocfilehash: b3e6e7384c9efdcb0e606f91d7357272f27ceaa1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830224"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="270bc-103">时间戳资源类型</span><span class="sxs-lookup"><span data-stu-id="270bc-103">timeStamp resource type</span></span>

> <span data-ttu-id="270bc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="270bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="270bc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="270bc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="270bc-106">日期和时间点时间信息。</span><span class="sxs-lookup"><span data-stu-id="270bc-106">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="270bc-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="270bc-107">JSON representation</span></span>

<span data-ttu-id="270bc-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="270bc-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="270bc-109">属性</span><span class="sxs-lookup"><span data-stu-id="270bc-109">Properties</span></span>
| <span data-ttu-id="270bc-110">属性</span><span class="sxs-lookup"><span data-stu-id="270bc-110">Property</span></span>     | <span data-ttu-id="270bc-111">类型</span><span class="sxs-lookup"><span data-stu-id="270bc-111">Type</span></span>   |<span data-ttu-id="270bc-112">说明</span><span class="sxs-lookup"><span data-stu-id="270bc-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="270bc-113">date</span><span class="sxs-lookup"><span data-stu-id="270bc-113">date</span></span>|<span data-ttu-id="270bc-114">Date</span><span class="sxs-lookup"><span data-stu-id="270bc-114">Date</span></span>|<span data-ttu-id="270bc-115">时间戳日期部分。</span><span class="sxs-lookup"><span data-stu-id="270bc-115">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="270bc-116">time</span><span class="sxs-lookup"><span data-stu-id="270bc-116">time</span></span>|<span data-ttu-id="270bc-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="270bc-117">TimeOfDay</span></span>|<span data-ttu-id="270bc-118">时间戳时间部分中。</span><span class="sxs-lookup"><span data-stu-id="270bc-118">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="270bc-119">timeZone</span><span class="sxs-lookup"><span data-stu-id="270bc-119">timeZone</span></span>|<span data-ttu-id="270bc-120">字符串</span><span class="sxs-lookup"><span data-stu-id="270bc-120">String</span></span>|<span data-ttu-id="270bc-121">时间戳，这是一个世界上 24 纵向方面 timezone 部分。</span><span class="sxs-lookup"><span data-stu-id="270bc-121">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
