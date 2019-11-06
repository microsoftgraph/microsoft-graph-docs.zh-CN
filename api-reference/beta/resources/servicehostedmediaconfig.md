---
title: serviceHostedMediaConfig 资源类型
description: ServiceHostedMediaConfig 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: edefba3e415a50322022e4549fbecbd37da6d1da
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006541"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="20393-103">serviceHostedMediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="20393-103">serviceHostedMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20393-104">ServiceHostedMediaConfig 类型。</span><span class="sxs-lookup"><span data-stu-id="20393-104">The serviceHostedMediaConfig type.</span></span>

## <a name="properties"></a><span data-ttu-id="20393-105">属性</span><span class="sxs-lookup"><span data-stu-id="20393-105">Properties</span></span>

| <span data-ttu-id="20393-106">属性</span><span class="sxs-lookup"><span data-stu-id="20393-106">Property</span></span>                    | <span data-ttu-id="20393-107">类型</span><span class="sxs-lookup"><span data-stu-id="20393-107">Type</span></span>                                                        | <span data-ttu-id="20393-108">说明</span><span class="sxs-lookup"><span data-stu-id="20393-108">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="20393-109">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="20393-109">preFetchMedia</span></span>               | <span data-ttu-id="20393-110">[mediaInfo](mediainfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="20393-110">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="20393-111">预回迁的介质列表。</span><span class="sxs-lookup"><span data-stu-id="20393-111">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="20393-112">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="20393-112">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="20393-113">布尔</span><span class="sxs-lookup"><span data-stu-id="20393-113">Boolean</span></span>                                                     | <span data-ttu-id="20393-114">从默认的音频组中删除自参与者。</span><span class="sxs-lookup"><span data-stu-id="20393-114">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="20393-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20393-115">JSON representation</span></span>

<span data-ttu-id="20393-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20393-116">The following is a JSON representation of the resource.</span></span>

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
  "preFetchMedia": [ { "@odata.type": "microsoft.graph.mediaInfo" } ],
  "removeFromDefaultAudioGroup": true
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
