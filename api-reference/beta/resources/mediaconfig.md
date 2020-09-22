---
title: mediaConfig 资源类型
description: 包含用于连接到呼叫的媒体配置的抽象基类。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 05f93ff0776795d988b66ad84c98af1d5f5bede2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971753"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="aceb5-103">mediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="aceb5-103">mediaConfig resource type</span></span>

<span data-ttu-id="aceb5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aceb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aceb5-105">包含用于连接到呼叫的媒体配置的抽象基类。</span><span class="sxs-lookup"><span data-stu-id="aceb5-105">An abstract base class that contains the media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="aceb5-106">属性</span><span class="sxs-lookup"><span data-stu-id="aceb5-106">Properties</span></span>

| <span data-ttu-id="aceb5-107">属性</span><span class="sxs-lookup"><span data-stu-id="aceb5-107">Property</span></span>       | <span data-ttu-id="aceb5-108">类型</span><span class="sxs-lookup"><span data-stu-id="aceb5-108">Type</span></span>    | <span data-ttu-id="aceb5-109">说明</span><span class="sxs-lookup"><span data-stu-id="aceb5-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aceb5-110">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="aceb5-110">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="aceb5-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="aceb5-111">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="aceb5-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aceb5-112">JSON representation</span></span>

<span data-ttu-id="aceb5-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aceb5-113">The following is a JSON representation of the resource.</span></span>

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


