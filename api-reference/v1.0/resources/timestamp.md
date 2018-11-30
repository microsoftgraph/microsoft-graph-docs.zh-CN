---
title: 时间戳资源类型
description: 日期和时间点时间信息。
ms.openlocfilehash: 4f392e880bb165841fd8a9a31b6ed00bf2ba36fb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008356"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="368dd-103">时间戳资源类型</span><span class="sxs-lookup"><span data-stu-id="368dd-103">timeStamp resource type</span></span>

<span data-ttu-id="368dd-104">日期和时间点时间信息。</span><span class="sxs-lookup"><span data-stu-id="368dd-104">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="368dd-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="368dd-105">JSON representation</span></span>

<span data-ttu-id="368dd-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="368dd-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="368dd-107">属性</span><span class="sxs-lookup"><span data-stu-id="368dd-107">Properties</span></span>
| <span data-ttu-id="368dd-108">属性</span><span class="sxs-lookup"><span data-stu-id="368dd-108">Property</span></span>       | <span data-ttu-id="368dd-109">类型</span><span class="sxs-lookup"><span data-stu-id="368dd-109">Type</span></span>    |<span data-ttu-id="368dd-110">说明</span><span class="sxs-lookup"><span data-stu-id="368dd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="368dd-111">date</span><span class="sxs-lookup"><span data-stu-id="368dd-111">date</span></span>|<span data-ttu-id="368dd-112">Date</span><span class="sxs-lookup"><span data-stu-id="368dd-112">Date</span></span>|<span data-ttu-id="368dd-113">时间戳日期部分。</span><span class="sxs-lookup"><span data-stu-id="368dd-113">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="368dd-114">time</span><span class="sxs-lookup"><span data-stu-id="368dd-114">time</span></span>|<span data-ttu-id="368dd-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="368dd-115">TimeOfDay</span></span>|<span data-ttu-id="368dd-116">时间戳时间部分中。</span><span class="sxs-lookup"><span data-stu-id="368dd-116">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="368dd-117">timeZone</span><span class="sxs-lookup"><span data-stu-id="368dd-117">timeZone</span></span>|<span data-ttu-id="368dd-118">字符串</span><span class="sxs-lookup"><span data-stu-id="368dd-118">String</span></span>|<span data-ttu-id="368dd-119">时间戳，这是一个世界上 24 纵向方面 timezone 部分。</span><span class="sxs-lookup"><span data-stu-id="368dd-119">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->