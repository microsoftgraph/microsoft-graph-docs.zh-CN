---
title: mediaInfo 资源类型
description: 在提示操作中使用的媒体信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b7e2b5fb0e00a7b173e1e14962b614fcca5382f5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971741"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="73196-103">mediaInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="73196-103">mediaInfo resource type</span></span>

<span data-ttu-id="73196-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73196-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73196-105">在提示操作中使用的媒体信息。</span><span class="sxs-lookup"><span data-stu-id="73196-105">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="73196-106">属性</span><span class="sxs-lookup"><span data-stu-id="73196-106">Properties</span></span>
| <span data-ttu-id="73196-107">属性</span><span class="sxs-lookup"><span data-stu-id="73196-107">Property</span></span>       | <span data-ttu-id="73196-108">类型</span><span class="sxs-lookup"><span data-stu-id="73196-108">Type</span></span>    | <span data-ttu-id="73196-109">说明</span><span class="sxs-lookup"><span data-stu-id="73196-109">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="73196-110">resourceId</span><span class="sxs-lookup"><span data-stu-id="73196-110">resourceId</span></span>     | <span data-ttu-id="73196-111">String</span><span class="sxs-lookup"><span data-stu-id="73196-111">String</span></span>  | <span data-ttu-id="73196-112">可选，用于唯一标识资源。</span><span class="sxs-lookup"><span data-stu-id="73196-112">Optional, used to uniquely identity the resource.</span></span> <span data-ttu-id="73196-113">如果传递了提示 uri，则会将此 resourceId 作为密钥进行缓存。</span><span class="sxs-lookup"><span data-stu-id="73196-113">If passed the prompt uri will be cached against this resourceId as key.</span></span> |
| <span data-ttu-id="73196-114">url</span><span class="sxs-lookup"><span data-stu-id="73196-114">uri</span></span>            | <span data-ttu-id="73196-115">String</span><span class="sxs-lookup"><span data-stu-id="73196-115">String</span></span>  | <span data-ttu-id="73196-116">要播放的提示的路径。</span><span class="sxs-lookup"><span data-stu-id="73196-116">Path to the prompt to be played.</span></span> <span data-ttu-id="73196-117">目前仅支持 ( .wav) 格式、单通道、16位样本和 16000 (16KHz) 采样速率。</span><span class="sxs-lookup"><span data-stu-id="73196-117">Currently only Wave file (.wav) format, single-channel, 16-bit samples with a 16,000 (16KHz) sampling rate is only supported.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="73196-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73196-118">JSON representation</span></span>

<span data-ttu-id="73196-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73196-119">The following is a JSON representation of the resource.</span></span>

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


