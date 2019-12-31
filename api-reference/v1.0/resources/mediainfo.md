---
title: mediaInfo 资源类型
description: 在提示操作中使用的媒体信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 20134131dba64ad48effa1c95e5d81ab81102805
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913203"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="cf4cd-103">mediaInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf4cd-103">mediaInfo resource type</span></span>

<span data-ttu-id="cf4cd-104">在提示操作中使用的媒体信息。</span><span class="sxs-lookup"><span data-stu-id="cf4cd-104">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="cf4cd-105">属性</span><span class="sxs-lookup"><span data-stu-id="cf4cd-105">Properties</span></span>
| <span data-ttu-id="cf4cd-106">属性</span><span class="sxs-lookup"><span data-stu-id="cf4cd-106">Property</span></span>       | <span data-ttu-id="cf4cd-107">类型</span><span class="sxs-lookup"><span data-stu-id="cf4cd-107">Type</span></span>    | <span data-ttu-id="cf4cd-108">说明</span><span class="sxs-lookup"><span data-stu-id="cf4cd-108">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="cf4cd-109">resourceId</span><span class="sxs-lookup"><span data-stu-id="cf4cd-109">resourceId</span></span>     | <span data-ttu-id="cf4cd-110">String</span><span class="sxs-lookup"><span data-stu-id="cf4cd-110">String</span></span>  | <span data-ttu-id="cf4cd-111">可选。</span><span class="sxs-lookup"><span data-stu-id="cf4cd-111">Optional.</span></span> <span data-ttu-id="cf4cd-112">用于唯一标识资源。</span><span class="sxs-lookup"><span data-stu-id="cf4cd-112">Used to uniquely identity the resource.</span></span> <span data-ttu-id="cf4cd-113">如果传入，则会将提示 uri 作为密钥缓存在此 resourceId 中。</span><span class="sxs-lookup"><span data-stu-id="cf4cd-113">If passed in, the prompt uri will be cached against this resourceId as a key.</span></span> |
| <span data-ttu-id="cf4cd-114">url</span><span class="sxs-lookup"><span data-stu-id="cf4cd-114">uri</span></span>            | <span data-ttu-id="cf4cd-115">String</span><span class="sxs-lookup"><span data-stu-id="cf4cd-115">String</span></span>  | <span data-ttu-id="cf4cd-116">将播放的提示的路径。</span><span class="sxs-lookup"><span data-stu-id="cf4cd-116">Path to the prompt that will be played.</span></span> <span data-ttu-id="cf4cd-117">目前仅支持带有16000（16KHz）采样速率的波形文件（.wav）格式、单通道、16位样本。</span><span class="sxs-lookup"><span data-stu-id="cf4cd-117">Currently supports only Wave file (.wav) format, single-channel, 16-bit samples with a 16,000 (16KHz) sampling rate.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="cf4cd-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf4cd-118">JSON representation</span></span>

<span data-ttu-id="cf4cd-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf4cd-119">The following is a JSON representation of the resource.</span></span>

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
