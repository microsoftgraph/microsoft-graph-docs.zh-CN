---
title: timeZoneBase 资源类型
description: 时区的基本表示形式。
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e8ec3a7d71bfc767b3ea54d9b4b8626d3ca953c4
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808849"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="53f0d-103">timeZoneBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="53f0d-103">timeZoneBase resource type</span></span>

<span data-ttu-id="53f0d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53f0d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="53f0d-105">时区的基本表示形式。</span><span class="sxs-lookup"><span data-stu-id="53f0d-105">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="53f0d-106">属性</span><span class="sxs-lookup"><span data-stu-id="53f0d-106">Properties</span></span>
| <span data-ttu-id="53f0d-107">属性</span><span class="sxs-lookup"><span data-stu-id="53f0d-107">Property</span></span>     | <span data-ttu-id="53f0d-108">类型</span><span class="sxs-lookup"><span data-stu-id="53f0d-108">Type</span></span>   |<span data-ttu-id="53f0d-109">说明</span><span class="sxs-lookup"><span data-stu-id="53f0d-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="53f0d-110">name</span><span class="sxs-lookup"><span data-stu-id="53f0d-110">name</span></span> | <span data-ttu-id="53f0d-111">string</span><span class="sxs-lookup"><span data-stu-id="53f0d-111">string</span></span> | <span data-ttu-id="53f0d-112">时区的名称。</span><span class="sxs-lookup"><span data-stu-id="53f0d-112">The name of a time zone.</span></span> <span data-ttu-id="53f0d-113">它可以是一个标准时区名称，例如“夏威夷-阿留申标准时间”，或自定义时区的“自定义时区”。</span><span class="sxs-lookup"><span data-stu-id="53f0d-113">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="53f0d-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53f0d-114">JSON representation</span></span>

<span data-ttu-id="53f0d-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53f0d-115">Here is a JSON representation of the resource.</span></span>

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
