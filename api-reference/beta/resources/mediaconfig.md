---
title: mediaConfig 资源类型
description: 包含用于连接到呼叫的媒体配置的抽象基类。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0f47ac0986107af16640208d64190da6138805d5
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866712"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="13a0c-103">mediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="13a0c-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13a0c-104">包含用于连接到呼叫的媒体配置的抽象基类。</span><span class="sxs-lookup"><span data-stu-id="13a0c-104">An abstract base class that contains the media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="13a0c-105">属性</span><span class="sxs-lookup"><span data-stu-id="13a0c-105">Properties</span></span>

| <span data-ttu-id="13a0c-106">属性</span><span class="sxs-lookup"><span data-stu-id="13a0c-106">Property</span></span>       | <span data-ttu-id="13a0c-107">类型</span><span class="sxs-lookup"><span data-stu-id="13a0c-107">Type</span></span>    | <span data-ttu-id="13a0c-108">说明</span><span class="sxs-lookup"><span data-stu-id="13a0c-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="13a0c-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="13a0c-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="13a0c-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="13a0c-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="13a0c-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13a0c-111">JSON representation</span></span>

<span data-ttu-id="13a0c-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13a0c-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
   ],
  "abstract": true,
  "@odata.type": "microsoft.graph.mediaConfig"
}-->
```json
{
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
