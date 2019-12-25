---
title: mediaInfo 资源类型
description: 在提示操作中使用的媒体信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9d9b8f4709d3379afda8e30fec2b7db64a474a0e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865779"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="f8bdf-103">mediaInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="f8bdf-103">mediaInfo resource type</span></span>

<span data-ttu-id="f8bdf-104">在提示操作中使用的媒体信息。</span><span class="sxs-lookup"><span data-stu-id="f8bdf-104">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="f8bdf-105">属性</span><span class="sxs-lookup"><span data-stu-id="f8bdf-105">Properties</span></span>
| <span data-ttu-id="f8bdf-106">属性</span><span class="sxs-lookup"><span data-stu-id="f8bdf-106">Property</span></span>       | <span data-ttu-id="f8bdf-107">类型</span><span class="sxs-lookup"><span data-stu-id="f8bdf-107">Type</span></span>    | <span data-ttu-id="f8bdf-108">说明</span><span class="sxs-lookup"><span data-stu-id="f8bdf-108">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="f8bdf-109">resourceId</span><span class="sxs-lookup"><span data-stu-id="f8bdf-109">resourceId</span></span>     | <span data-ttu-id="f8bdf-110">String</span><span class="sxs-lookup"><span data-stu-id="f8bdf-110">String</span></span>  | <span data-ttu-id="f8bdf-111">可选。</span><span class="sxs-lookup"><span data-stu-id="f8bdf-111">Optional.</span></span> <span data-ttu-id="f8bdf-112">用于唯一标识资源。</span><span class="sxs-lookup"><span data-stu-id="f8bdf-112">Used to uniquely identity the resource.</span></span> <span data-ttu-id="f8bdf-113">如果传入，则会将提示 uri 作为密钥缓存在此 resourceId 中。</span><span class="sxs-lookup"><span data-stu-id="f8bdf-113">If passed in, the prompt uri will be cached against this resourceId as a key.</span></span> |
| <span data-ttu-id="f8bdf-114">url</span><span class="sxs-lookup"><span data-stu-id="f8bdf-114">uri</span></span>            | <span data-ttu-id="f8bdf-115">String</span><span class="sxs-lookup"><span data-stu-id="f8bdf-115">String</span></span>  | <span data-ttu-id="f8bdf-116">将播放的提示的路径。</span><span class="sxs-lookup"><span data-stu-id="f8bdf-116">Path to the prompt that will be played.</span></span> <span data-ttu-id="f8bdf-117">目前仅支持带有16000（16KHz）采样速率的波形文件（.wav）格式、单通道、16位样本。</span><span class="sxs-lookup"><span data-stu-id="f8bdf-117">Currently supports only Wave file (.wav) format, single-channel, 16-bit samples with a 16,000 (16KHz) sampling rate.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f8bdf-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8bdf-118">JSON representation</span></span>

<span data-ttu-id="f8bdf-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8bdf-119">The following is a JSON representation of the resource.</span></span>

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
