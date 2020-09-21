---
title: mediaInfo 资源类型
description: 在提示操作中使用的媒体信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8e2f5a0d59f06449d122f4ca2db582afa4da9c39
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965524"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="51b5f-103">mediaInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="51b5f-103">mediaInfo resource type</span></span>

<span data-ttu-id="51b5f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51b5f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="51b5f-105">在提示操作中使用的媒体信息。</span><span class="sxs-lookup"><span data-stu-id="51b5f-105">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="51b5f-106">属性</span><span class="sxs-lookup"><span data-stu-id="51b5f-106">Properties</span></span>
| <span data-ttu-id="51b5f-107">属性</span><span class="sxs-lookup"><span data-stu-id="51b5f-107">Property</span></span>       | <span data-ttu-id="51b5f-108">类型</span><span class="sxs-lookup"><span data-stu-id="51b5f-108">Type</span></span>    | <span data-ttu-id="51b5f-109">说明</span><span class="sxs-lookup"><span data-stu-id="51b5f-109">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="51b5f-110">resourceId</span><span class="sxs-lookup"><span data-stu-id="51b5f-110">resourceId</span></span>     | <span data-ttu-id="51b5f-111">String</span><span class="sxs-lookup"><span data-stu-id="51b5f-111">String</span></span>  | <span data-ttu-id="51b5f-112">可选。</span><span class="sxs-lookup"><span data-stu-id="51b5f-112">Optional.</span></span> <span data-ttu-id="51b5f-113">用于唯一标识资源。</span><span class="sxs-lookup"><span data-stu-id="51b5f-113">Used to uniquely identity the resource.</span></span> <span data-ttu-id="51b5f-114">如果传入，则会将提示 uri 作为密钥缓存在此 resourceId 中。</span><span class="sxs-lookup"><span data-stu-id="51b5f-114">If passed in, the prompt uri will be cached against this resourceId as a key.</span></span> |
| <span data-ttu-id="51b5f-115">url</span><span class="sxs-lookup"><span data-stu-id="51b5f-115">uri</span></span>            | <span data-ttu-id="51b5f-116">String</span><span class="sxs-lookup"><span data-stu-id="51b5f-116">String</span></span>  | <span data-ttu-id="51b5f-117">将播放的提示的路径。</span><span class="sxs-lookup"><span data-stu-id="51b5f-117">Path to the prompt that will be played.</span></span> <span data-ttu-id="51b5f-118">目前仅支持 ( .wav) 格式、单通道、16位样本以及 16000 (16KHz) 采样速率。</span><span class="sxs-lookup"><span data-stu-id="51b5f-118">Currently supports only Wave file (.wav) format, single-channel, 16-bit samples with a 16,000 (16KHz) sampling rate.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="51b5f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51b5f-119">JSON representation</span></span>

<span data-ttu-id="51b5f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51b5f-120">The following is a JSON representation of the resource.</span></span>

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

