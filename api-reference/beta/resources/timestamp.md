---
title: 时间戳资源类型
description: 时间点的日期和时间信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: JeremyKelley
ms.openlocfilehash: 1037212f1adb0fb10326bbdf88416877e16a9fbe
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810991"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="431e3-103">时间戳资源类型</span><span class="sxs-lookup"><span data-stu-id="431e3-103">timeStamp resource type</span></span>

<span data-ttu-id="431e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="431e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="431e3-105">时间点的日期和时间信息。</span><span class="sxs-lookup"><span data-stu-id="431e3-105">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="431e3-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="431e3-106">JSON representation</span></span>

<span data-ttu-id="431e3-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="431e3-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="431e3-108">属性</span><span class="sxs-lookup"><span data-stu-id="431e3-108">Properties</span></span>
| <span data-ttu-id="431e3-109">属性</span><span class="sxs-lookup"><span data-stu-id="431e3-109">Property</span></span>     | <span data-ttu-id="431e3-110">类型</span><span class="sxs-lookup"><span data-stu-id="431e3-110">Type</span></span>   |<span data-ttu-id="431e3-111">说明</span><span class="sxs-lookup"><span data-stu-id="431e3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="431e3-112">date</span><span class="sxs-lookup"><span data-stu-id="431e3-112">date</span></span>|<span data-ttu-id="431e3-113">Date</span><span class="sxs-lookup"><span data-stu-id="431e3-113">Date</span></span>|<span data-ttu-id="431e3-114">时间戳的日期部分。</span><span class="sxs-lookup"><span data-stu-id="431e3-114">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="431e3-115">time</span><span class="sxs-lookup"><span data-stu-id="431e3-115">time</span></span>|<span data-ttu-id="431e3-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="431e3-116">TimeOfDay</span></span>|<span data-ttu-id="431e3-117">时间戳的时间部分。</span><span class="sxs-lookup"><span data-stu-id="431e3-117">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="431e3-118">timeZone</span><span class="sxs-lookup"><span data-stu-id="431e3-118">timeZone</span></span>|<span data-ttu-id="431e3-119">String</span><span class="sxs-lookup"><span data-stu-id="431e3-119">String</span></span>|<span data-ttu-id="431e3-120">时间戳的时区部分，是世界上的 24 longitudinal 区域之一。</span><span class="sxs-lookup"><span data-stu-id="431e3-120">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

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
