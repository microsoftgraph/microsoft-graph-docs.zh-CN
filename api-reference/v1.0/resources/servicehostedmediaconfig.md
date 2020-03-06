---
title: serviceHostedMediaConfig 资源类型
description: ServiceHostedMediaConfig 类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 7f43d529e2fc18ddf67876737c07a66c606db560
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533752"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="b6603-103">serviceHostedMediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6603-103">serviceHostedMediaConfig resource type</span></span>

<span data-ttu-id="b6603-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6603-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b6603-105">远程承载的媒体。</span><span class="sxs-lookup"><span data-stu-id="b6603-105">The media that's hosted remotely.</span></span> <span data-ttu-id="b6603-106">这是从[mediaConfig](mediaconfig.md)继承的。</span><span class="sxs-lookup"><span data-stu-id="b6603-106">This is inherited from [mediaConfig](mediaconfig.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b6603-107">属性</span><span class="sxs-lookup"><span data-stu-id="b6603-107">Properties</span></span>

| <span data-ttu-id="b6603-108">属性</span><span class="sxs-lookup"><span data-stu-id="b6603-108">Property</span></span>                    | <span data-ttu-id="b6603-109">类型</span><span class="sxs-lookup"><span data-stu-id="b6603-109">Type</span></span>                                                        | <span data-ttu-id="b6603-110">说明</span><span class="sxs-lookup"><span data-stu-id="b6603-110">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="b6603-111">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="b6603-111">preFetchMedia</span></span>               | <span data-ttu-id="b6603-112">[mediaInfo](mediainfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="b6603-112">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="b6603-113">预回迁的介质列表。</span><span class="sxs-lookup"><span data-stu-id="b6603-113">The list of media to pre-fetch.</span></span>                   |


## <a name="json-representation"></a><span data-ttu-id="b6603-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6603-114">JSON representation</span></span>

<span data-ttu-id="b6603-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6603-115">The following is a JSON representation of the resource.</span></span>

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
