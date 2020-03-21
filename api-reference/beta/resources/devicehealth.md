---
title: deviceHealth 资源类型
description: 表示设备的运行状况，包括任何错误。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: efd8b1e7722eabcacd05512b0101735d677d9b89
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895642"
---
# <a name="devicehealth-resource-type"></a><span data-ttu-id="cf1d5-103">deviceHealth 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf1d5-103">deviceHealth resource type</span></span>

<span data-ttu-id="cf1d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf1d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf1d5-105">表示设备的运行状况，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="cf1d5-105">Represents a device's health, including any errors.</span></span>

## <a name="properties"></a><span data-ttu-id="cf1d5-106">属性</span><span class="sxs-lookup"><span data-stu-id="cf1d5-106">Properties</span></span>
| <span data-ttu-id="cf1d5-107">属性</span><span class="sxs-lookup"><span data-stu-id="cf1d5-107">Property</span></span>     | <span data-ttu-id="cf1d5-108">类型</span><span class="sxs-lookup"><span data-stu-id="cf1d5-108">Type</span></span>        | <span data-ttu-id="cf1d5-109">说明</span><span class="sxs-lookup"><span data-stu-id="cf1d5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cf1d5-110">lastConnectionTime</span><span class="sxs-lookup"><span data-stu-id="cf1d5-110">lastConnectionTime</span></span>|<span data-ttu-id="cf1d5-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf1d5-111">DateTimeOffset</span></span>|<span data-ttu-id="cf1d5-112">上次连接设备的时间。</span><span class="sxs-lookup"><span data-stu-id="cf1d5-112">The last time the device was connected.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf1d5-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf1d5-113">JSON representation</span></span>

<span data-ttu-id="cf1d5-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf1d5-114">The following is a JSON representation of the resource.</span></span>

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