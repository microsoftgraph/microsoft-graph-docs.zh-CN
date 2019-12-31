---
title: mediaInfo 资源类型
description: 在提示操作中使用的媒体信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d17117880cf736870d2728a9666af689a4296d04
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913294"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="3c51a-103">mediaInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c51a-103">mediaInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c51a-104">在提示操作中使用的媒体信息。</span><span class="sxs-lookup"><span data-stu-id="3c51a-104">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="3c51a-105">属性</span><span class="sxs-lookup"><span data-stu-id="3c51a-105">Properties</span></span>
| <span data-ttu-id="3c51a-106">属性</span><span class="sxs-lookup"><span data-stu-id="3c51a-106">Property</span></span>       | <span data-ttu-id="3c51a-107">类型</span><span class="sxs-lookup"><span data-stu-id="3c51a-107">Type</span></span>    | <span data-ttu-id="3c51a-108">说明</span><span class="sxs-lookup"><span data-stu-id="3c51a-108">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="3c51a-109">resourceId</span><span class="sxs-lookup"><span data-stu-id="3c51a-109">resourceId</span></span>     | <span data-ttu-id="3c51a-110">String</span><span class="sxs-lookup"><span data-stu-id="3c51a-110">String</span></span>  | <span data-ttu-id="3c51a-111">可选，用于唯一标识资源。</span><span class="sxs-lookup"><span data-stu-id="3c51a-111">Optional, used to uniquely identity the resource.</span></span> <span data-ttu-id="3c51a-112">如果传递了提示 uri，则会将此 resourceId 作为密钥进行缓存。</span><span class="sxs-lookup"><span data-stu-id="3c51a-112">If passed the prompt uri will be cached against this resourceId as key.</span></span> |
| <span data-ttu-id="3c51a-113">url</span><span class="sxs-lookup"><span data-stu-id="3c51a-113">uri</span></span>            | <span data-ttu-id="3c51a-114">String</span><span class="sxs-lookup"><span data-stu-id="3c51a-114">String</span></span>  | <span data-ttu-id="3c51a-115">要播放的提示的路径。</span><span class="sxs-lookup"><span data-stu-id="3c51a-115">Path to the prompt to be played.</span></span> <span data-ttu-id="3c51a-116">目前仅支持带有16000（16KHz）采样速率的波形文件（.wav）格式的单通道、16位样本。</span><span class="sxs-lookup"><span data-stu-id="3c51a-116">Currently only Wave file (.wav) format, single-channel, 16-bit samples with a 16,000 (16KHz) sampling rate is only supported.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="3c51a-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c51a-117">JSON representation</span></span>

<span data-ttu-id="3c51a-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c51a-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
