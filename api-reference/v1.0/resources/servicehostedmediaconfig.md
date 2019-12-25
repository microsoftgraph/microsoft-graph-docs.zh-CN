---
title: serviceHostedMediaConfig 资源类型
description: ServiceHostedMediaConfig 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 590eef4c572695188e609133f5bc852fd90c51f7
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865765"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="49489-103">serviceHostedMediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="49489-103">serviceHostedMediaConfig resource type</span></span>

<span data-ttu-id="49489-104">远程承载的媒体。</span><span class="sxs-lookup"><span data-stu-id="49489-104">The media that's hosted remotely.</span></span> <span data-ttu-id="49489-105">这是从[mediaConfig](mediaconfig.md)继承的。</span><span class="sxs-lookup"><span data-stu-id="49489-105">This is inherited from [mediaConfig](mediaconfig.md).</span></span>

## <a name="properties"></a><span data-ttu-id="49489-106">属性</span><span class="sxs-lookup"><span data-stu-id="49489-106">Properties</span></span>

| <span data-ttu-id="49489-107">属性</span><span class="sxs-lookup"><span data-stu-id="49489-107">Property</span></span>                    | <span data-ttu-id="49489-108">类型</span><span class="sxs-lookup"><span data-stu-id="49489-108">Type</span></span>                                                        | <span data-ttu-id="49489-109">说明</span><span class="sxs-lookup"><span data-stu-id="49489-109">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="49489-110">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="49489-110">preFetchMedia</span></span>               | <span data-ttu-id="49489-111">[mediaInfo](mediainfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="49489-111">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="49489-112">预回迁的介质列表。</span><span class="sxs-lookup"><span data-stu-id="49489-112">The list of media to pre-fetch.</span></span>                   |


## <a name="json-representation"></a><span data-ttu-id="49489-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49489-113">JSON representation</span></span>

<span data-ttu-id="49489-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49489-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "preFetchMedia"
  ],
  "baseType": "microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [ { "@odata.type": "microsoft.graph.mediaInfo" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "serviceHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
