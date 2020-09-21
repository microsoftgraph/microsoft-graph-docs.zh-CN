---
title: mediaPrompt 资源类型
description: 此资源类型包含有关要播放的音频文件和其他其他设置的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 37329364ccfcb4b70de04ebfe8344ea407ce2bc7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965517"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="4a66b-103">mediaPrompt 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a66b-103">mediaPrompt resource type</span></span>

<span data-ttu-id="4a66b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a66b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4a66b-105">此资源类型包含有关要播放的音频文件和其他其他设置的信息。</span><span class="sxs-lookup"><span data-stu-id="4a66b-105">This resource type contains information about the audio file to be played and other additional settings.</span></span>

## <a name="properties"></a><span data-ttu-id="4a66b-106">属性</span><span class="sxs-lookup"><span data-stu-id="4a66b-106">Properties</span></span>

| <span data-ttu-id="4a66b-107">属性</span><span class="sxs-lookup"><span data-stu-id="4a66b-107">Property</span></span>    | <span data-ttu-id="4a66b-108">类型</span><span class="sxs-lookup"><span data-stu-id="4a66b-108">Type</span></span>                      | <span data-ttu-id="4a66b-109">说明</span><span class="sxs-lookup"><span data-stu-id="4a66b-109">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="4a66b-110">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="4a66b-110">mediaInfo</span></span>   | [<span data-ttu-id="4a66b-111">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="4a66b-111">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="4a66b-112">媒体信息</span><span class="sxs-lookup"><span data-stu-id="4a66b-112">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="4a66b-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a66b-113">JSON representation</span></span>

<span data-ttu-id="4a66b-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a66b-114">The following is a JSON representation of the resource.</span></span>

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

