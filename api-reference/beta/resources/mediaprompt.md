---
title: mediaPrompt 资源类型
description: MediaPrompt 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1def44fbf2208f40ff432e943e9d6768718258c9
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006660"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="1e894-103">mediaPrompt 资源类型</span><span class="sxs-lookup"><span data-stu-id="1e894-103">mediaPrompt resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e894-104">MediaPrompt 类型。</span><span class="sxs-lookup"><span data-stu-id="1e894-104">The mediaPrompt type.</span></span>

## <a name="properties"></a><span data-ttu-id="1e894-105">属性</span><span class="sxs-lookup"><span data-stu-id="1e894-105">Properties</span></span>

| <span data-ttu-id="1e894-106">属性</span><span class="sxs-lookup"><span data-stu-id="1e894-106">Property</span></span>    | <span data-ttu-id="1e894-107">类型</span><span class="sxs-lookup"><span data-stu-id="1e894-107">Type</span></span>                      | <span data-ttu-id="1e894-108">说明</span><span class="sxs-lookup"><span data-stu-id="1e894-108">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="1e894-109">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="1e894-109">mediaInfo</span></span>   | [<span data-ttu-id="1e894-110">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="1e894-110">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="1e894-111">媒体信息</span><span class="sxs-lookup"><span data-stu-id="1e894-111">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="1e894-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1e894-112">JSON representation</span></span>

<span data-ttu-id="1e894-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e894-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

## <a name="example"></a><span data-ttu-id="1e894-114">示例</span><span class="sxs-lookup"><span data-stu-id="1e894-114">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->
```json
{
  "@odata.type": "#microsoft.graph.mediaPrompt",
  "mediaInfo": {
    "@odata.type": "#microsoft.graph.mediaInfo",
    "uri": "https://cdn.contoso.com/beep.wav",
    "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
