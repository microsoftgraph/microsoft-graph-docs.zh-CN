---
title: timeZoneBase 资源类型
description: 时区的基本表示形式。
localization_priority: Normal
ms.openlocfilehash: 95d3409c40b3cc151f7b2f4b69580b9c1bbbe1ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882451"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="9cb3a-103">timeZoneBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="9cb3a-103">timeZoneBase resource type</span></span>

> <span data-ttu-id="9cb3a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9cb3a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9cb3a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9cb3a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9cb3a-106">时区的基本表示形式。</span><span class="sxs-lookup"><span data-stu-id="9cb3a-106">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="9cb3a-107">属性</span><span class="sxs-lookup"><span data-stu-id="9cb3a-107">Properties</span></span>
| <span data-ttu-id="9cb3a-108">属性</span><span class="sxs-lookup"><span data-stu-id="9cb3a-108">Property</span></span>     | <span data-ttu-id="9cb3a-109">类型</span><span class="sxs-lookup"><span data-stu-id="9cb3a-109">Type</span></span>   |<span data-ttu-id="9cb3a-110">说明</span><span class="sxs-lookup"><span data-stu-id="9cb3a-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9cb3a-111">name</span><span class="sxs-lookup"><span data-stu-id="9cb3a-111">name</span></span> | <span data-ttu-id="9cb3a-112">string</span><span class="sxs-lookup"><span data-stu-id="9cb3a-112">string</span></span> | <span data-ttu-id="9cb3a-113">时区的名称。</span><span class="sxs-lookup"><span data-stu-id="9cb3a-113">The name of a time zone.</span></span> <span data-ttu-id="9cb3a-114">它可以是一个标准时区名称，例如“夏威夷-阿留申标准时间”，或自定义时区的“自定义时区”。</span><span class="sxs-lookup"><span data-stu-id="9cb3a-114">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="9cb3a-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9cb3a-115">JSON representation</span></span>

<span data-ttu-id="9cb3a-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9cb3a-116">Here is a JSON representation of the resource.</span></span>

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
