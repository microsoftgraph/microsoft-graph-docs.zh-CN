---
title: timeZoneBase 资源类型
description: 时区的基本表示形式。
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5399aa644d4ebc3622639f885cac3dcf7c1d772c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090730"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="1def6-103">timeZoneBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="1def6-103">timeZoneBase resource type</span></span>

<span data-ttu-id="1def6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1def6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1def6-105">时区的基本表示形式。</span><span class="sxs-lookup"><span data-stu-id="1def6-105">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="1def6-106">属性</span><span class="sxs-lookup"><span data-stu-id="1def6-106">Properties</span></span>
| <span data-ttu-id="1def6-107">属性</span><span class="sxs-lookup"><span data-stu-id="1def6-107">Property</span></span>     | <span data-ttu-id="1def6-108">类型</span><span class="sxs-lookup"><span data-stu-id="1def6-108">Type</span></span>   |<span data-ttu-id="1def6-109">说明</span><span class="sxs-lookup"><span data-stu-id="1def6-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1def6-110">name</span><span class="sxs-lookup"><span data-stu-id="1def6-110">name</span></span> | <span data-ttu-id="1def6-111">string</span><span class="sxs-lookup"><span data-stu-id="1def6-111">string</span></span> | <span data-ttu-id="1def6-112">时区的名称。</span><span class="sxs-lookup"><span data-stu-id="1def6-112">The name of a time zone.</span></span> <span data-ttu-id="1def6-113">它可以是一个标准时区名称，例如“夏威夷-阿留申标准时间”，或自定义时区的“自定义时区”。</span><span class="sxs-lookup"><span data-stu-id="1def6-113">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="1def6-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1def6-114">JSON representation</span></span>

<span data-ttu-id="1def6-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1def6-115">Here is a JSON representation of the resource.</span></span>

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

