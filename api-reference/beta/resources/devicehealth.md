---
title: deviceHealth 资源类型
description: 表示设备的运行状况，包括任何错误。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7da256308ee63607d7d2d0e7ba62cb3030db4835
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049854"
---
# <a name="devicehealth-resource-type"></a><span data-ttu-id="a9c7d-103">deviceHealth 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9c7d-103">deviceHealth resource type</span></span>

<span data-ttu-id="a9c7d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9c7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9c7d-105">表示设备的运行状况，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="a9c7d-105">Represents a device's health, including any errors.</span></span>

## <a name="properties"></a><span data-ttu-id="a9c7d-106">属性</span><span class="sxs-lookup"><span data-stu-id="a9c7d-106">Properties</span></span>
| <span data-ttu-id="a9c7d-107">属性</span><span class="sxs-lookup"><span data-stu-id="a9c7d-107">Property</span></span>     | <span data-ttu-id="a9c7d-108">类型</span><span class="sxs-lookup"><span data-stu-id="a9c7d-108">Type</span></span>        | <span data-ttu-id="a9c7d-109">说明</span><span class="sxs-lookup"><span data-stu-id="a9c7d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a9c7d-110">lastConnectionTime</span><span class="sxs-lookup"><span data-stu-id="a9c7d-110">lastConnectionTime</span></span>|<span data-ttu-id="a9c7d-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9c7d-111">DateTimeOffset</span></span>|<span data-ttu-id="a9c7d-112">上次连接设备的时间。</span><span class="sxs-lookup"><span data-stu-id="a9c7d-112">The last time the device was connected.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a9c7d-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9c7d-113">JSON representation</span></span>

<span data-ttu-id="a9c7d-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9c7d-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceHealth"
}-->

```json
{
    "lastConnectionTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceHealth resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

