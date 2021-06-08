---
title: timeClockSettings 资源类型
description: 表示计划的 timeclock 设置。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 96ffddc0730ffaff73d21a8ab051acf9ea140ccc
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786365"
---
# <a name="timeclocksettings-resource-type"></a><span data-ttu-id="b08f7-103">timeClockSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="b08f7-103">timeClockSettings resource type</span></span>

<span data-ttu-id="b08f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b08f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b08f7-105">表示计划的 timeclock [设置](schedule.md)。</span><span class="sxs-lookup"><span data-stu-id="b08f7-105">Represents timeclock settings for a [schedule](schedule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b08f7-106">属性</span><span class="sxs-lookup"><span data-stu-id="b08f7-106">Properties</span></span>
|<span data-ttu-id="b08f7-107">属性</span><span class="sxs-lookup"><span data-stu-id="b08f7-107">Property</span></span>               |<span data-ttu-id="b08f7-108">类型</span><span class="sxs-lookup"><span data-stu-id="b08f7-108">Type</span></span>           |<span data-ttu-id="b08f7-109">说明</span><span class="sxs-lookup"><span data-stu-id="b08f7-109">Description</span></span>                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| <span data-ttu-id="b08f7-110">approvedLocation</span><span class="sxs-lookup"><span data-stu-id="b08f7-110">approvedLocation</span></span> | [<span data-ttu-id="b08f7-111">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="b08f7-111">geoCoordinates</span></span>](geocoordinates.md)  |<span data-ttu-id="b08f7-112">**timeClock 的已审批位置**。</span><span class="sxs-lookup"><span data-stu-id="b08f7-112">The aprroved location of the **timeClock**.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="b08f7-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b08f7-113">JSON representation</span></span>

<span data-ttu-id="b08f7-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b08f7-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeClockSettings"
}-->
```json
{ 
   "approvedLocation": {

           "altitude": {"@odata.type": "microsoft.graph.GeoCoordinates"},

           "latitude": {"@odata.type": "microsoft.graph.GeoCoordinates"},

           "longitude": {"@odata.type": "microsoft.graph.GeoCoordinates"}

        }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeClockSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
