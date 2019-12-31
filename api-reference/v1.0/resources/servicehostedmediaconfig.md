---
title: serviceHostedMediaConfig 资源类型
description: ServiceHostedMediaConfig 类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 35d5754071aa388e300042b9977fd759a38a6b74
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912949"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="8865a-103">serviceHostedMediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="8865a-103">serviceHostedMediaConfig resource type</span></span>

<span data-ttu-id="8865a-104">远程承载的媒体。</span><span class="sxs-lookup"><span data-stu-id="8865a-104">The media that's hosted remotely.</span></span> <span data-ttu-id="8865a-105">这是从[mediaConfig](mediaconfig.md)继承的。</span><span class="sxs-lookup"><span data-stu-id="8865a-105">This is inherited from [mediaConfig](mediaconfig.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8865a-106">属性</span><span class="sxs-lookup"><span data-stu-id="8865a-106">Properties</span></span>

| <span data-ttu-id="8865a-107">属性</span><span class="sxs-lookup"><span data-stu-id="8865a-107">Property</span></span>                    | <span data-ttu-id="8865a-108">类型</span><span class="sxs-lookup"><span data-stu-id="8865a-108">Type</span></span>                                                        | <span data-ttu-id="8865a-109">说明</span><span class="sxs-lookup"><span data-stu-id="8865a-109">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="8865a-110">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="8865a-110">preFetchMedia</span></span>               | <span data-ttu-id="8865a-111">[mediaInfo](mediainfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="8865a-111">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="8865a-112">预回迁的介质列表。</span><span class="sxs-lookup"><span data-stu-id="8865a-112">The list of media to pre-fetch.</span></span>                   |


## <a name="json-representation"></a><span data-ttu-id="8865a-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8865a-113">JSON representation</span></span>

<span data-ttu-id="8865a-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8865a-114">The following is a JSON representation of the resource.</span></span>

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
