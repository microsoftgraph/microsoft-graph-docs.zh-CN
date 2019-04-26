---
title: timeZoneBase 资源类型
description: 时区的基本表示形式。
localization_priority: Normal
ms.openlocfilehash: 8d968b8177da942c1b8940618c8ba965c362c914
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341867"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="6b210-103">timeZoneBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b210-103">timeZoneBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b210-104">时区的基本表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b210-104">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="6b210-105">属性</span><span class="sxs-lookup"><span data-stu-id="6b210-105">Properties</span></span>
| <span data-ttu-id="6b210-106">属性</span><span class="sxs-lookup"><span data-stu-id="6b210-106">Property</span></span>     | <span data-ttu-id="6b210-107">类型</span><span class="sxs-lookup"><span data-stu-id="6b210-107">Type</span></span>   |<span data-ttu-id="6b210-108">说明</span><span class="sxs-lookup"><span data-stu-id="6b210-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6b210-109">name</span><span class="sxs-lookup"><span data-stu-id="6b210-109">name</span></span> | <span data-ttu-id="6b210-110">string</span><span class="sxs-lookup"><span data-stu-id="6b210-110">string</span></span> | <span data-ttu-id="6b210-111">时区的名称。</span><span class="sxs-lookup"><span data-stu-id="6b210-111">The name of a time zone.</span></span> <span data-ttu-id="6b210-112">它可以是一个标准时区名称，例如“夏威夷-阿留申标准时间”，或自定义时区的“自定义时区”。</span><span class="sxs-lookup"><span data-stu-id="6b210-112">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="6b210-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b210-113">JSON representation</span></span>

<span data-ttu-id="6b210-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b210-114">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
