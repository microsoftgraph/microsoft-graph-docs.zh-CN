---
title: bookingWorkTimeSlot 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 2c9caa1f5a9a2b78911e77df27b84079efd70ab2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507878"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="3dbe2-104">bookingWorkTimeSlot 资源类型</span><span class="sxs-lookup"><span data-stu-id="3dbe2-104">bookingWorkTimeSlot resource type</span></span>

<span data-ttu-id="3dbe2-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3dbe2-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="3dbe2-106">工作的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="3dbe2-106">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="3dbe2-107">属性</span><span class="sxs-lookup"><span data-stu-id="3dbe2-107">Properties</span></span>
| <span data-ttu-id="3dbe2-108">属性</span><span class="sxs-lookup"><span data-stu-id="3dbe2-108">Property</span></span>     | <span data-ttu-id="3dbe2-109">类型</span><span class="sxs-lookup"><span data-stu-id="3dbe2-109">Type</span></span>   |<span data-ttu-id="3dbe2-110">说明</span><span class="sxs-lookup"><span data-stu-id="3dbe2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3dbe2-111">end</span><span class="sxs-lookup"><span data-stu-id="3dbe2-111">end</span></span>|<span data-ttu-id="3dbe2-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="3dbe2-112">TimeOfDay</span></span>|<span data-ttu-id="3dbe2-113">一天中开始工作的时间。</span><span class="sxs-lookup"><span data-stu-id="3dbe2-113">The time of the day that work starts.</span></span> <span data-ttu-id="3dbe2-114">例如，08：00：00.0000000。</span><span class="sxs-lookup"><span data-stu-id="3dbe2-114">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="3dbe2-115">start</span><span class="sxs-lookup"><span data-stu-id="3dbe2-115">start</span></span>|<span data-ttu-id="3dbe2-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="3dbe2-116">TimeOfDay</span></span>|<span data-ttu-id="3dbe2-117">一天中停止工作的时间。</span><span class="sxs-lookup"><span data-stu-id="3dbe2-117">The time of the day that work stops.</span></span> <span data-ttu-id="3dbe2-118">例如，17：00：00.0000000。</span><span class="sxs-lookup"><span data-stu-id="3dbe2-118">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3dbe2-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3dbe2-119">JSON representation</span></span>

<span data-ttu-id="3dbe2-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3dbe2-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingWorkTimeSlot"
}-->

```json
{
  "end": "String (timestamp)",
  "start": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingWorkTimeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
