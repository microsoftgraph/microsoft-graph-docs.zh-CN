---
title: timeZoneBase 资源类型
description: 时区的基本表示形式。
ms.openlocfilehash: 18df657ab561163b64bcf224f8902f2ba7e0039c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009721"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="d5eda-103">timeZoneBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5eda-103">timeZoneBase resource type</span></span>

<span data-ttu-id="d5eda-104">时区的基本表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5eda-104">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="d5eda-105">属性</span><span class="sxs-lookup"><span data-stu-id="d5eda-105">Properties</span></span>
| <span data-ttu-id="d5eda-106">属性</span><span class="sxs-lookup"><span data-stu-id="d5eda-106">Property</span></span>     | <span data-ttu-id="d5eda-107">类型</span><span class="sxs-lookup"><span data-stu-id="d5eda-107">Type</span></span>   |<span data-ttu-id="d5eda-108">说明</span><span class="sxs-lookup"><span data-stu-id="d5eda-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d5eda-109">name</span><span class="sxs-lookup"><span data-stu-id="d5eda-109">name</span></span> | <span data-ttu-id="d5eda-110">string</span><span class="sxs-lookup"><span data-stu-id="d5eda-110">string</span></span> | <span data-ttu-id="d5eda-111">时区的名称。</span><span class="sxs-lookup"><span data-stu-id="d5eda-111">The name of a time zone.</span></span> <span data-ttu-id="d5eda-112">它可以是一个标准时区名称，例如“夏威夷-阿留申标准时间”，或自定义时区的“自定义时区”。</span><span class="sxs-lookup"><span data-stu-id="d5eda-112">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="d5eda-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5eda-113">JSON representation</span></span>

<span data-ttu-id="d5eda-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5eda-114">Here is a JSON representation of the resource.</span></span>

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