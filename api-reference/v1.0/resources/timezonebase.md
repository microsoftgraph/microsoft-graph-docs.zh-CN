---
title: timeZoneBase 资源类型
description: 时区的基本表示形式。
localization_priority: Normal
ms.openlocfilehash: 4c112a3118bf3f4d00be790d7923bc0fe82dc72f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860632"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="ba0be-103">timeZoneBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba0be-103">timeZoneBase resource type</span></span>

<span data-ttu-id="ba0be-104">时区的基本表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba0be-104">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="ba0be-105">属性</span><span class="sxs-lookup"><span data-stu-id="ba0be-105">Properties</span></span>
| <span data-ttu-id="ba0be-106">属性</span><span class="sxs-lookup"><span data-stu-id="ba0be-106">Property</span></span>     | <span data-ttu-id="ba0be-107">类型</span><span class="sxs-lookup"><span data-stu-id="ba0be-107">Type</span></span>   |<span data-ttu-id="ba0be-108">说明</span><span class="sxs-lookup"><span data-stu-id="ba0be-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ba0be-109">name</span><span class="sxs-lookup"><span data-stu-id="ba0be-109">name</span></span> | <span data-ttu-id="ba0be-110">string</span><span class="sxs-lookup"><span data-stu-id="ba0be-110">string</span></span> | <span data-ttu-id="ba0be-111">时区的名称。</span><span class="sxs-lookup"><span data-stu-id="ba0be-111">The name of a time zone.</span></span> <span data-ttu-id="ba0be-112">它可以是一个标准时区名称，例如“夏威夷-阿留申标准时间”，或自定义时区的“自定义时区”。</span><span class="sxs-lookup"><span data-stu-id="ba0be-112">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="ba0be-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba0be-113">JSON representation</span></span>

<span data-ttu-id="ba0be-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba0be-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
